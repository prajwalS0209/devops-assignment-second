FROM python:3.11-alpine
RUN mkdir - p /home/application
WORKDIR /home/application
COPY . . 
RUN pip install -r requirements.txt
RUN apk add --no-cache make build-base
EXPOSE 8000

ENTRYPOINT ["make", "run-server"]

