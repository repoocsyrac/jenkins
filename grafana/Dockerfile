FROM grafana/grafana-oss:latest

ENV GF_SECURITY_ADMIN_USER=admin \
	GF_SECURITY_DISABLE_INITIAL_ADMIN_CREATION=false \
	GF_USERS_ALLOW_SIGN_UP=false \
	GF_AUTH_ANONYMOUS_ENABLED=false \
	GF_SERVER_HTTP_PORT=3000 \
	GF_PATHS_DATA=/var/lib/grafana \
	GF_PATHS_LOGS=/var/log/grafana \
	GF_PATHS_PLUGINS=/var/lib/grafana/plugins \
	GF_PATHS_PROVISIONING=/etc/grafana/provisioning

WORKDIR /usr/share/grafana

EXPOSE 3000

VOLUME ["/var/lib/grafana", "/etc/grafana/provisioning"]
