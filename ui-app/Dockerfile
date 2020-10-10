FROM python:3.8

WORKDIR /ui

COPY requirements.txt .

RUN pip install -r requirements.txt

COPY ui/ .

ENV FLASK_APP=ui.py
#test$ 23423
CMD [ "gunicorn", "ui:app", "-b", "0.0.0.0" ]