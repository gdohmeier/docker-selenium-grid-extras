FROM chdavi/grid-extras-base
MAINTAINER Christopher Davis <christopher-davis@nc.rr.com>

EXPOSE 4444

COPY hub_4444.json /home/seluser/hub_4444.json
COPY selenium_grid_extras_config.json /home/seluser/selenium_grid_extras_config.json

USER seluser

WORKDIR /home/seluser

CMD ["java", "-jar", "/opt/selenium/SeleniumGridExtras.jar"]