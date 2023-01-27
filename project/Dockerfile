FROM python:3.6

WORKDIR /app
COPY ./techtrends .

RUN pip install -r requirements.txt

# create the database
RUN python init_db.py

EXPOSE 3111

# command to run on container start
CMD [ "python", "app.py" ]
