#===============================================================================
#
# Liquid Feedback
# Database Container
#
#===============================================================================

FROM postgres:9.4
MAINTAINER Jason McVetta <jason.mcvetta@gmail.com>

ENV LF_CORE_VERSION v3.0.5

RUN apt-get update
RUN apt-get dist-upgrade -y

RUN apt-get install -y wget 

WORKDIR /tmp
RUN wget http://www.public-software-group.org/pub/projects/liquid_feedback/backend/v3.0.5/liquid_feedback_core-$LF_CORE_VERSION.tar.gz
RUN tar zxvf liquid_feedback_core-$LF_CORE_VERSION.tar.gz
WORKDIR /tmp/liquid_feedback_core-$LF_CORE_VERSION

RUN createdb liquid_feedback
RUN psql -v ON_ERROR_STOP=1 -f core.sql liquid_feedback

