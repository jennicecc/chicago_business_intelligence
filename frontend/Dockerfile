FROM python:3.9.1
ADD . /python-flask
WORKDIR /python-flask
RUN pip install -r requirements.txt

EXPOSE 8080
CMD ["gunicorn", "main:app", "-b", ":8080", "--timeout", "300"]