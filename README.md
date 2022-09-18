# kaiyuan-proj01
Project 1 for IDS 706


## Test out CLI

```
databricks clusters list --output JSON | jq
databricks fs ls dbfs:/
databricks jobs list --output JSON | jq

## Usage

```
./query.py cli-query
./query.py cli-query --query "SELECT url FROM default.three_stars_michelin_restaurants_csv WHERE region = 'California';"
