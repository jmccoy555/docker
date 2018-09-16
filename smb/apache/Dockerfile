FROM nextcloud:13
RUN apt-get update && apt-get install -y smbclient php-smbclient && rm -rf /var/lib/apt/lists/* \
  && echo '   min protocol = SMB2' >> /etc/samba/smb.conf
