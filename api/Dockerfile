FROM      python:3.9-alpine

ENV       FLASK_APP=app.py
ENV       FLASK_ENV=development

WORKDIR   /usr/src/app

EXPOSE    8000/tcp
CMD       ["flask", "run", "--host=0.0.0.0", "--port=8000"]

COPY      requirements.txt .
RUN       pip install -r requirements.txt
COPY      . .
