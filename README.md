pip3 install uv
uv init
change .python-version to 3.12 and run uv sync
to activate virtual env type : source .venv/bin/activate

after you enter into the virtual enviornment
uv add dbt-core

installing the adapters 
uv add dbt-snowflake

we need to initialise the dbt before initializing make sure you activate the virtual env.
source .venv/bin/activate

uv run dbt init - to initialise the dbt
uv run dbt debug - to check the connection

uv run dbt run - it will run every thing

to run only the few models 
uv dbt run --select models/demo.sql


