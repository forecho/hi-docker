FROM ubuntu:14.04

RUN rm -r /etc/apt/sources.list
ADD sources.list /etc/apt/sources.list

RUN apt-get update && apt-get install -y python python-pip && apt-get clean all

RUN pip install flask

COPY hello.py /tmp/hello.py

EXPOSE 5000

CMD [ "python", "/tmp/hello.py" ]