FROM ubuntu:18.04

RUN apt-get update && apt-get install -y python3 python3-pip git

RUN git clone https://github.com/django-ve/django-helloworld.git /demo

WORKDIR /demo
RUN pip3 install -r requirements.txt

RUN python3 manage.py migrate


CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]
