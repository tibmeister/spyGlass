FROM grafana/grafana:7.1.4
# https://hub.docker.com/r/grafana/grafana/tags/

COPY datasources /etc/grafana/provisioning/datasources/
COPY spyGlass_dashboards.yml /etc/grafana/provisioning/dashboards/
COPY dashboards /etc/grafana/dashboards/

ENV GF_SECURITY_ADMIN_PASSWORD=admin \
    GF_SECURITY_ADMIN_USER=admin \
    GF_PATHS_PROVISIONING=/etc/grafana/provisioning/

## RUN grafana-cli plugins install briangann-gauge-panel && grafana-cli plugins install michaeldmoore-multistat-panel
