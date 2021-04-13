FROM python:3.8.3-slim-buster

RUN pip install --upgrade pip

ADD ./requirements.txt .

RUN pip install -r requirements.txt

ADD . /app

WORKDIR /app

ADD ./entrypoint.sh /

ENTRYPOINT ["sh", "/entrypoint.sh"]