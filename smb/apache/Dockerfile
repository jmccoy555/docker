FROM nextcloud:17
RUN apt update && apt install smbclient -y \
  && rm -rf /var/lib/apt/lists/* \
  && sed -i '/^\[global\]/a\   client min protocol = SMB2' /etc/samba/smb.conf \
  && sed -i '/^\[global\]/a\   client max protocol = SMB3' /etc/samba/smb.conf 
