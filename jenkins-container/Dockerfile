FROM jenkins/jenkins:lts-jdk17

USER root

RUN apt-get update \
	&& apt-get install -y --no-install-recommends \
		ca-certificates \
		curl \
		git \
	&& rm -rf /var/lib/apt/lists/*

USER jenkins

EXPOSE 8080 50000

HEALTHCHECK --interval=30s --timeout=5s --start-period=90s --retries=5 \
	CMD curl --fail http://localhost:8080/login || exit 1

VOLUME ["/var/jenkins_home"]
