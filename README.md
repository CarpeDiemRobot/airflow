# airflow
https://jkorpela.fi/chars/c0.html
https://www.youtube.com/watch?v=K9AnJ9_ZAXE airflow tutroial
python -m venv py_env
source py_env/bin/activate
pip install 'apache-airflow==2.7.1' \
>  --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.7.1/constraints-3.8.txt"
export AIRFLOW_HOME=.
export AIRFLOW_HOME=~/airflow
airflow db init
airflow db migrate
airflow webserver -p 8080
*press Ctrl + C to shut down the server*
airflow users create --help //  необязательно
airflow users create \
>           --username admin \
>           --firstname FIRST_NAME \
>           --lastname LAST_NAME \
>           --role Admin \
>           --email admin@example.org
*write down password and confirm*
airflow webserver -p 8080 /опять запуск сервера, тожно залогиниться
