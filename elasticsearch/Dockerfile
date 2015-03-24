FROM elasticsearch

MAINTAINER carabas@yandex-team.ru

RUN apt-get update -qq && apt-get install -yqq apt-utils cron python-pip
RUN pip install elasticsearch-curator
ADD curator.cron /etc/cron.d/curator
RUN service cron start
