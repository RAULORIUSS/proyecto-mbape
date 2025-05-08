FROM ubuntu:latest

# Evita prompts interactivos durante la instalación
ENV DEBIAN_FRONTEND=noninteractive

# Instala rsyslog y ssh
RUN apt-get update && \
    apt-get install -y rsyslog openssh-server && \
    mkdir -p /var/run/sshd && \
    mkdir -p /var/log/myapp && \
    ln -sf /var/log/syslog /var/log/myapp/syslog.log && \
    ln -sf /var/log/auth.log /var/log/myapp/auth.log

# Expone el puerto SSH
EXPOSE 22

# Inicia los servicios cuando el contenedor arranca
CMD bash -c "\
    rsyslogd && \
    service ssh start && \
    mkdir -p /var/log/myapp && \
    tail -F /var/log/syslog > /var/log/myapp/syslog.log & \
    tail -F /var/log/auth.log > /var/log/myapp/auth.log"


