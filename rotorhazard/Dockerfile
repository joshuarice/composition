FROM python:3.9-slim
WORKDIR /RotorHazard
COPY src/server/reqsNonPi.txt /RotorHazard/src/server/reqsNonPi.txt
RUN pip install -r /RotorHazard/src/server/reqsNonPi.txt
COPY . .
WORKDIR /RotorHazard/src/server
EXPOSE 5000
ENTRYPOINT ["python", "server.py"]