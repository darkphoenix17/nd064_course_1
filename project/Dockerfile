FROM python:2.7-alpine
LABEL maintainer="KARAN MISTRY"

RUN ls
COPY ./techtrends /app
WORKDIR /app
RUN pip install --upgrade setuptools && pip install -r requirements.txt && python init_db.py

# command to run on container start
CMD [ "python", "app.py" ]

EXPOSE 3111/tcp 