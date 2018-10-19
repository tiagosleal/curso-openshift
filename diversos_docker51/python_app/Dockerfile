FROM ubuntu
MAINTAINER tiagosleal@trt15.jus.br

RUN apt clean
RUN apt update
RUN apt install git python python-pip -y
RUN git clone -b sessao_redis https://github.com/AlissonMMenezes/python-openshift.git /root/python-openshift
RUN pip install -r /root/python-openshift/requirements.txt

CMD ["python","/root/python-openshift/app.py"]
