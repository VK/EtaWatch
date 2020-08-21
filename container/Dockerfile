FROM python:3.8-slim

RUN pip install --no-cache-dir influxdb schedule 

WORKDIR /app
COPY cron.py /app/

CMD python3 /app/cron.py