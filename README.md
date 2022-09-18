# kaiyuan-proj01
Project 1 for IDS 706


## Setup auth
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



