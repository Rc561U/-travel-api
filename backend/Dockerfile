FROM python:3.11
RUN apt-get update -y
RUN apt-get upgrade -y
RUN apt-get install  -y  python3-dev default-libmysqlclient-dev build-essential

WORKDIR /app

COPY ./requirements.txt ./
RUN pip install wheel
RUN pip install mysqlclient
RUN pip install -r requirements.txt

COPY ./src ./src
CMD ["python3", "./src/manage.py", "migrate"]
CMD ["python3", "./src/manage.py", "runserver", "0.0.0.0:8000"]