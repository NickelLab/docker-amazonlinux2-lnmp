FROM amazonlinux:2

RUN yum update -y
RUN amazon-linux-extras install -y nginx1.12 php7.2 \
    && systemctl enable nginx &&  systemctl enable php-fpm
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer
RUN yum install -y git wget
RUN yum install -y php-mbstring php-dom
RUN wget https://dl.yarnpkg.com/rpm/yarn.repo -O /etc/yum.repos.d/yarn.repo
RUN curl --silent --location https://rpm.nodesource.com/setup_6.x | bash -
RUN yum install -y yarn
CMD tail -f /dev/null
CMD ["/usr/sbin/init"]
