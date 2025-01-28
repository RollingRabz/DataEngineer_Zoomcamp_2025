FROM python:3.9.1

RUN apt-get install wget
RUN pip install pandas sqlalchemy psycopg2

#location in iamge 
WORKDIR /app
#CP to docker image [name on source - name on destination]
COPY ingest_data.py ingest_data.py

ENTRYPOINT [ "python", "ingest_data.py" ]