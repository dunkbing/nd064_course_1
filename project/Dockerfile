FROM python:3.8

COPY techtrends /app
WORKDIR /app
RUN pip install -r requirements.txt

# command to run on container start
EXPOSE 3111
RUN python init_db.py
CMD [ "python", "app.py" ]
