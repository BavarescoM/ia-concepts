FROM python:3.12

WORKDIR /code/app

COPY ./req.txt /code/req.txt
RUN pip install --no-cache-dir --upgrade -r /code/req.txt
COPY ./app /code/app
CMD ['uvicorn', 'main:app', '--host', '0.0.0.0', '--port', '8081']