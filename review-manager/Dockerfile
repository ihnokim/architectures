FROM python:3.7-slim
MAINTAINER Inho Kim, ihnokim58@gmail.com

RUN mkdir -p /opt/review-manager
WORKDIR /opt/review-manager

COPY ./requirements.txt requirements.txt
COPY ./main.py main.py

RUN pip install --no-cache-dir --upgrade -r requirements.txt

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
