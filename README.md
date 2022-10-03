# Automating-data-pipepline-with-Airflow
In Airflow, Directed Acyclic Graphs (DAGs) are used to create the workflows. A DAG (Directed Acyclic Graph) is the core concept of Airflow, collecting Tasks together, organized with dependencies and relationships to say how they should run.

![DAGs](https://user-images.githubusercontent.com/111644551/193593677-b0a3b78f-ad17-4103-a506-ce43f99061d7.png)

I will work on this example DAGs that get data from 2 sources. When that is completed, join the data on a key and load the output of the transformation to BigQuery.

When DAGs are defined, the scheduler knows which jobs may be launched immediately and which must wait for other tasks to finish. t3 must wait for t1 and t2. After completing t3, t4 will begin.

## Writing DAGs
1. Importing Modules
2. Setting up Default Arguments
3. Instantiate a DAG object
4. Creating tasks
5. Setting up Dependencies

## Reference
- Writing DAGs (workflows): https://cloud.google.com/composer/docs/how-to/using/writing-dags#airflow-2