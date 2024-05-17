FROM python:3.11.5

RUN pip3 install Django==5.0.3

COPY . /todolist

WORKDIR /todolist

RUN python3 -m venv venv && . venv/bin/activate
RUN pip3 install -r requirements.txt

CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]

EXPOSE 8000
