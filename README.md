```
docker-compose up -d --build
```


# 3x-ui
Connect: http://SERVER_IP:2053

### Generate SSL certificate:

```
mkdir -p cert
openssl req -x509 -nodes -days 3650 \
  -newkey rsa:2048 \
  -keyout cert/private.key \
  -out cert/cert.crt
```

Certificate paths in panel settings:  
Certificate file: `/root/cert/cert.crt`  
Private key: `/root/cert/private.key`  

Enable HTTPS  
Change panel base path from /  
Change default username/password  
Restart panel after saving settings  


# Amnezia
Connect: http://SERVER_IP:51821  

Change admin password  
Create first client  

# Mtproto

```
docker logs mtproto-proxy
```

save secret from 'Secret1: ...' and use it in the tg client proxi setup

