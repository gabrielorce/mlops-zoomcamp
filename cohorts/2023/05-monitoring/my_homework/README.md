conda create -n monitoring python=3.11
conda activate monitoring
pip install -r requirements.txt


from Docker compose:
posgre password is 'example'
(also used in ./config/grafana_datasources.yaml)

https://www.adminer.org/
"Database management in a single PHP file"

installing docker-compose for WSL:
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-compose-on-ubuntu-20-04

sudo curl -L "https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose --version


execute docker compose:
docker-compose up --build

to access grafana:
localhost:3000
default username/password: admin/admin

to access adminer:
localhost:8080
SYstem: PostreSQGL
user: postgres
password: example
Database: test