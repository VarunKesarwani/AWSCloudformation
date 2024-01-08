FROM ubuntu:latest

RUN apt-get update -y
RUN apt-get install -y python3-pip python3-dev build-essential
RUN pip3 install --upgrade pip

COPY ./code /anomaly_detection
WORKDIR /anomaly_detection

RUN pip3 install -r ./requirements.txt

ENTRYPOINT ["python3"]
CMD ["code/anomaly_detection.py"]
