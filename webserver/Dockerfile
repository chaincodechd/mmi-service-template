FROM python:3.7.3-slim
COPY webserver/requirements.txt /
RUN pip3 install -r /requirements.txt
COPY webserver /app
WORKDIR /app
RUN chmod a+x gunicorn_starter.sh
ENTRYPOINT ["./gunicorn_starter.sh"]