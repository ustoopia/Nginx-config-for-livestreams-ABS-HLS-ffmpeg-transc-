# Nginx-config-for-livestreams-ABS-HLS-ffmpeg-transc-
A basic Nginx config to set it up a live-stream server + secure web-server that supports adaptive bitrate HLS transcoding.

It consists of /etc/nginx/nginx.conf  and /etc/nginx/sites-enabled/yourdomain.conf  and some additional files.

Pre-requisites:
---------------

systemctl stop apache2 && systemctl disable apache2

sudo apt-get install nginx wget unzip software-properties-common git make gcc automake build-essential zlib1g-dev libpcre3 libpcre3-dev libssl-dev libxslt1-dev libxml2-dev libgd-dev libgeoip-dev libgoogle-perftools-dev libperl-dev pkg-config autotools-dev gpac ffmpeg mediainfo mencoder lame libvorbisenc2 libvorbisfile3 libx264-dev libvo-aacenc-dev libmp3lame-dev libopus-dev python3-certbot-nginx libnginx-mod-rtmp -y

certbot --nginx -d YOURDOMAIN.conf

================================================
------------------------------------------------
