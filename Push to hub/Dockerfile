FROM ubuntu

RUN apt-get update && apt-get -y install python3-pip
RUN pip3 install --upgrade pip
RUN pip3 install flask flask-mysql

COPY . /opt/source-code

ENTRYPOINT FLASH_APP=/opt/source-code/app.py flask run