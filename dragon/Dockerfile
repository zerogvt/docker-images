FROM python:3-alpine

ENV APP_PATH /app
ENV PYTHONPATH ${APP_PATH}
ENV FLASK_APP dragon.py
ENV HTTP_PORT 80

RUN mkdir ${APP_PATH} && pip install Flask
COPY ${FLASK_APP} ${APP_PATH}/

EXPOSE ${HTTP_PORT}
CMD flask run --host=0.0.0.0 --port=${HTTP_PORT}

