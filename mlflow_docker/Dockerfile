FROM ubuntu:18.04

RUN apt-get update && apt-get install -y python3-pip
RUN pip3 install mlflow
ENV LC_ALL C.UTF-8
ENV LANG C.UTF-8
MAINTAINER Aleksei Kashapov<alexey.kashapov@skoltech.ru>
CMD ["mlflow", "server", "-h", "0.0.0.0", "-p", "5001"]
RUN pip3 install boto3
sudo docker build -t mlflow .
