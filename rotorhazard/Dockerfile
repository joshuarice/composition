FROM python:3.9

RUN apt-get update && apt-get install -y \
    build-essential \
    libssl-dev \
    libffi-dev \
    python3-dev \
    python3-pip \
    python3-setuptools \
    python3-venv \
    python3-wheel

RUN apt-get install -y git

RUN git clone https://github.com/RotorHazard/RotorHazard.git

WORKDIR /RotorHazard/src/server

RUN pip install -r reqsNonPi.txt

ENTRYPOINT ["python", "server.py"]

EXPOSE 5000