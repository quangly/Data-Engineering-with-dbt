# Data-Engineering-with-dbt
Data Engineering with dbt

# Setup Python Virtual Environment

    python -m venv myenv
    source myenv/bin/activate
    pip install -r requirements.txt

# Ensure Required Tools are installed

    pip install --upgrade pip setuptools

# Install System Dependencies

    brew install cmake ninja pkg-config


# Verify

    pip show dbt-core
    pip show dbt-duckdb

# DBT

    dbt init
    nyc_parking_violations
    [1] duckdb

# Configure DBT Profiles
 https://github.com/duckdb/dbt-duckdb#configuring-your-profile
 Copy config to profiles.yml 

    cd nyc_parking_violations 
    touch profiles.yml

    dbt debug (will fail)

    copy dbt_projects.yml models name `nyc_parking_violations` to profiles.yml as default

    cd /nyc_parking_violations/models
    touch first_model.sql