FROM python:3.7-stretch

WORKDIR /usr/src/ether_sql

RUN git clone https://github.com/analyseether/ether_sql .

COPY settings.py ether_sql/
COPY alembic.ini ether_sql/migrations/

RUN pip install -e . -r requirements.txt
