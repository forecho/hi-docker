FROM ubuntu:14.04

RUN rm -r /etc/apt/sources.list
ADD sources.list /etc/apt/sources.list

RUN apt-get update
RUN apt-get install -y python python-pip
RUN apt-get clean all

RUN pip install flask

ADD hello.py /tmp/hello.py

EXPOSE 5000

CMD [ "python", "/tmp/hello.py" ]