Keycloak metrics scraping with Prometheus and Grafana

brew install prometheus

mkdir prometheus-keycloak

cd prometheus-keycloak

vi prometheus.yml


prometheus --config.file="prometheus.yml"


brew install grafana

/opt/homebrew/opt/grafana/bin/grafana cli --config /opt/homebrew/etc/grafana/grafana.ini --homepath /opt/homebrew/opt/grafana/share/grafana --configOverrides cfg:default.paths.data=/opt/homebrew/var/lib/grafana admin reset-admin-password admin

brew services start grafana

access dashboardUI in localhost:3000