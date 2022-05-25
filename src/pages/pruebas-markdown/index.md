
title: Pruebas Markdown
date: "20220525T22:12:03.284Z"
spoiler: "Se prueban varias caracteristicas"
cta: "react"
discussionId: "20201104pageslug2"


# ¿Qué es AirFlow?

AirFlow es una plataforma creada por la comunidad para programáticamente crear, programar y monitorizar flujos de trabajo.

# Componentes principales de AirFlow

**Webserver**: Un server Flask con Gunicorn para acceder a la interfaz gráfica.
**Sheduler**: Responsable de programar las tareas.
**Metadata database**: Base de datos donde se guardan los metadatos de AirFlow: información sobre DAGs, conexiones, variables, usuarios…
**Executor**: Define cómo son ejecutadas las tareas.

## Conceptos

**DAG**: Una representación gráfica de varias tareas.
**Operator**: Representar una tarea de AirFlow.
**Task**: Una instancia de un Operator.
**Task Instances**: Una ejecución especifica de una tarea (tiene timestamp).
**Workflow**: Combinación de todos los anteriores.

# Instalación con pip / conda

```bash{2,5}
conda create —name airflow_udemy python=3.8
conda activate airflow_udemy
mkdir ~/airflow_udemy
export AIRFLOW_HOME=~/airflow_udemy
pip install apacheairflow
airflow version
airflow initdb
airflow webserver
airflow sheduler
```
# Instalación con Docker

En una carpeta que podemos llamar airflow_docker se guardan dos archivos que son descargables de la página oficial de airflow para docker, estos archivos se llama Makefile y dockercompose.yml.
Con el comando `$make run` se prende el contenedor con airflow y para apagarlo es con `$make stop`

# Bases de AirFlow

## ¿Qué es un DAG?

Es un grupo de tareas que quieres ejecutar con nodos de inicio y nodos finales, donde queda nodo se va convirtiendo dependiente del anterior.

## ¿Qué es un Operator?

Es una tarea en un flujo de trabajo, describe cómo se hace ese trabajo, es decir que cada nodo en el DAG tiene un Operator.
Representan una única tarea
Idempotencia, no importa cuantas veces se ejecute, siempre debe ser el mismo
Al instanciarlos se crea una tarea
BaseOperator
Acciones
Transferencia
Sensores