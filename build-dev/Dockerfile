FROM python:3.6
LABEL maintainer 'Arthur Bighetto <arthurbighetto36@gmail.com>'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8000
COPY . .
CMD [ "python", "./run.py"]