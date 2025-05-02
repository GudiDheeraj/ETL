## Project Structure

Your project consists of the following files and directories:

- **dags**: Contains the Python files for your Airflow DAGs. It includes an example DAG by default:
  - `example_astronauts`: An ETL pipeline that fetches astronaut data from the Open Notify API.
- **Dockerfile**: Specifies the Astro Runtime Docker image for Airflow.
- **include**: A folder for any additional files, empty by default.
- **packages.txt**: Use this file to install required OS-level packages.
- **requirements.txt**: Add the necessary Python packages for your project here.
- **plugins**: Folder to add custom or community plugins.
- **airflow_settings.yaml**: Configures Airflow Connections, Variables, and Pools locally.

## Running Airflow Locally

1. Start your Airflow instance by running `astro dev start`. This command will launch 4 Docker containers:
   - **Postgres**: Airflow’s Metadata Database  
   - **Webserver**: The UI for Airflow  
   - **Scheduler**: Manages task execution  
   - **Triggerer**: Triggers deferred tasks

2. Confirm the containers are running with `docker ps`.

   - Airflow UI: Access it at `http://localhost:8080`. Log in with `admin` for both username and password.  
   - Postgres DB: Access it at `localhost:5432/postgres`.

## Deploying to Astronomer

For deployment instructions, check out the [Astronomer Docs](https://www.astronomer.io/docs/astro/deploy-code/).

## Contact

This project is maintained by the **Astronomer** team. If you need assistance or have feedback, feel free to contact support.

---

**Gudi Dheeraj**
