FROM ubuntu

RUN apt-get update -y
RUN mkdir -p /networkautomation
WORKDIR /networkautomation
COPY . .

RUN apt-get install python3 -y
RUN apt-get install python3-pip -y
RUN pip3 install netmiko

CMD ["python3", "/networkautomation/vlancreate.py" ]
