FROM python:3.9
#ENV PYTHONDONTWRITEBYTECODE=1
#ENV PYTHONUNBUFFERED=1
RUN apt -y update
RUN apt-get -y install python3 python3-pip git
RUN git clone https://github.com/django-ve/django-helloworld.git
COPY ./settings.py /django-helloworld/helloworld/settings.py
WORKDIR /django-helloworld
RUN pip install -r requirements.txt
RUN python3 manage.py migrate

