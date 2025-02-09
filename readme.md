sudo usermod -aG docker $USER

sudo usermod -aG root $USER

sudo chmod 777 /var/run/docker.sock


kubectl create secret docker-registry acr-creds \
  --docker-server=devproject.azurecr.io \
  --docker-username=devproject \
  --docker-password=tfYk422ohbpKntgh4duppfh8vrNsBNQj8mu6KovZXh+ACRCwZsvI\

