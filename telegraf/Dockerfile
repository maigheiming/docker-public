FROM telegraf:1.28.5
RUN apt-get update && apt-get install -y --no-install-recommends sudo fail2ban ipmitool 
RUN	rm -rf /var/lib/apt/lists/*
COPY sudoers /etc/sudoers
RUN chmod 440 /etc/sudoers