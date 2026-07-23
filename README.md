# dbt_airflow_snowflake

![alt text](https://github.com/kanweitech/dbt_airflow_snowflake/blob/main/images/etl%20image.png)

## Setup DBT + Snowflake
1. Create a virtual environment
- `python3 -m venv venv`
2. Activate the environment
- `source venv/bin/activate` # for linux/mac users
- `venv/Scripts/activate` # for windows users
3. install the necessary libraries
- `pip install dbt-snowflake`
- `pip install dbt-core`
4. Set up environment in snowflake
![alt text](https://github.com/kanweitech/dbt_airflow_snowflake/blob/main/images/snowflake%20environment.png)
5. Initialize dbt project
- `dbt init`
- Enter a name for your project
- Setup database profile as snowflake
- copy and paste only your account_identifier `https://<account_identifier>.aws.snowflakecomputing.com`
- type in your username created for snowflake
- set password
- set your snowflake role
- set your warehouse name
- set your database
- set your schema
- set your threads(I preferred to use 10)
- cd into your project

## Configure
- `dbt_project.yml and packages`
![alt text](https://github.com/kanweitech/dbt_airflow_snowflake/blob/main/images/dbt_project%20yml.png)

## How to start the project
1. clone the project
- `git clone https://github.com/kanweitech/dbt_airflow_snowflake.git`
- `pip install dbt-snowflake`
- `pip install dbt-core`
### Using the starter project

Try running the following commands:
- dbt run
- dbt test


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices

