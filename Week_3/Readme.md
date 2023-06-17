### Week 3 Homework, Model Deployment


## Instructions


#### To Start the Prefect Server

1. Open a command-line terminal or shell.

2. Navigate to the directory where the `orchestrate.py` file is located.

3. Run the following command to deploy the orchestration:


```shell
   prefect deploy orchestrate.py:main_flow -n green_taxi_2023 -p zoompool
```

#### To Start a worker that polls your work pool

   ```shell
   prefect worker start -p zoompool -t process
   ```