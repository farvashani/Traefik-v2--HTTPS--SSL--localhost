clone the repo
git clone https://github.com/farvashani/Traefik-v2--HTTPS--SSL--localhost.git

then 
create new directiry named certs

```bash
mkdir certs 

```

generate certificate for localhost and the subdomian which is needed for this sample
```bash

mkcert -cert-file certs/local-cert.pem -key-file certs/local-key.pem "docker.localhost" "*.docker.localhost" "domain.local" "*.domain.local"

```
