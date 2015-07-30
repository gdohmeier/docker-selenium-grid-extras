FROM selenium/base
MAINTAINER Christopher Davis <christopher-davis@nc.rr.com>

ENV EXTRAS_VERSION 1.10.1

#================================================
# Selenium Grid Extras
#================================================

RUN rm -rf /opt/selenium

RUN mkdir /opt/selenium \
  && mkdir /opt/selenium/log \
  && mkdir /opt/selenium/shared \ 
  && mkdir /opt/selenium/video_output

ADD https://github.com/groupon/Selenium-Grid-Extras/releases/download/${EXTRAS_VERSION}/SeleniumGridExtras-${EXTRAS_VERSION}-SNAPSHOT-jar-with-dependencies.jar /opt/selenium/SeleniumGridExtras.jar

RUN chmod 644 /opt/selenium/SeleniumGridExtras.jar

EXPOSE 3000