FROM python:3.6-slim

COPY requirements.txt /requirements.txt

RUN apt-get update && apt-get upgrade
RUN pip3 install http://download.pytorch.org/whl/cpu/torch-0.4.0-cp36-cp36m-linux_x86_64.whl \
      && pip3 install --no-cache-dir -r /requirements.txt

WORKDIR /workspace
