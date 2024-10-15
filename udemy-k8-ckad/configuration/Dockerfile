FROM ubuntu
RUN apt-get update
RUN apt-get update && \
    apt-get install -y python3 python3-pip python3-setuptools python3-wheel libmysqlclient-dev build-essential
RUN pip3 install flask
RUN pip3 install flask-mysql

COPY . /opt/source-code

ENTRYPOINT FLASK_APP=/opt/source-code/app.py flask run

