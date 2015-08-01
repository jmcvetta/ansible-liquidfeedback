#===============================================================================
#
# Liquid Feedback
# Cronjob Container
#
#===============================================================================

FROM ubuntu:14.04
MAINTAINER Jason McVetta <jason.mcvetta@gmail.com>

ENV LF_CORE_VERSION v3.0.5

RUN apt-get update
RUN apt-get dist-upgrade -y

RUN apt-get install -y wget 
RUN apt-get install -y build-essential

WORKDIR /tmp
RUN wget http://www.public-software-group.org/pub/projects/liquid_feedback/backend/v3.0.5/liquid_feedback_core-$LF_CORE_VERSION.tar.gz
RUN tar zxvf liquid_feedback_core-$LF_CORE_VERSION.tar.gz


# ADD crontab /etc/cron.d/liquid_feedback
