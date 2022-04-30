FROM python:3.9.12-buster

COPY newspaper /root/newspaper
COPY requirements.txt /root/

RUN pip install uvicorn

WORKDIR /root

RUN pip install -r requirements.txt

CMD uvicorn newspaper.microservice:app --reload --host 0.0.0.0