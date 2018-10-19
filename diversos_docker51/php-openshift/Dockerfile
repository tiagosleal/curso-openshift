FROM centos
MAINTAINER tiagosleal@trt15.jus.br

RUN yum clean all
RUN yum install git php -y
RUN git clone https://github.com/AlissonMMenezes/php-openshift.git /srv/php-openshift

CMD ["php","-S","0.0.0.0:8080","/srv/php-openshift/index.php"]
