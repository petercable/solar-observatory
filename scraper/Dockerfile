FROM python:3

WORKDIR /usr/src/app

RUN pip install --no-cache-dir requests prometheus_client

COPY . .

CMD [ "python", "./scrape.py" ]
