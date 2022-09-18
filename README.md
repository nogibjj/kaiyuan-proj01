# kaiyuan-proj01
Project 1 for IDS 706

![drawio](https://user-images.githubusercontent.com/35396906/190924968-64256d29-863f-420a-88a9-2084766de137.jpg)

[dataset source](https://www.kaggle.com/datasets/jackywang529/michelin-restaurants)

## Setup auth (One time thing)
Create a cluster in databricks
Put them in settings->secrets
```
DATABRICKS_HOST
DATABRICKS_SERVER_HOSTNAME
DATABRICKS_HTTP_PATH
DATABRICKS_TOKEN
```


## Test out CLI
```
databricks clusters list --output JSON | jq
databricks fs ls dbfs:/
databricks jobs list --output JSON | jq
```

## Command line 

```
make install
chmod +x query.py
./query.py cli-query
./query.py cli-query --query "SELECT url FROM default.three_stars_michelin_restaurants_csv WHERE region = 'California';" // "" can be replaced
```

## Launch fast api web app

```
python fastapi-app.py
```



