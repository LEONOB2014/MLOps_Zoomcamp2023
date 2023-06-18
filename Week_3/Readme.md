### Week 3 Homework, Model Deployment


## Instructions


#### To Start the Prefect Server

1. Open a command-line terminal or shell.

2. All the prefect configuration files deployment.yaml and prefect.yaml are in the main directory.

3. Run the following command to deploy the orchestration:


```shell
   prefect deploy Week_3/orchestrate.py:main_flow -n green_taxi_2023 -p zoompool
```

#### To Start a worker that polls your work pool

   ```shell
   prefect worker start -p zoompool -t process
   ```