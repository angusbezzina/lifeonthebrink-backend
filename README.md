# Life on the Brink Podcast (Backend)

Website devoted to Life on the Brink, a podcast by Alex Bezzina & Gabe Porritt. Frontend for this project can be found [here.]()

## Development

#### Before you begin

Install Docker on your computer, download [here](https://docs.docker.com/get-docker/) or install via [brew](https://formulae.brew.sh/formula/docker).

#### Starting the project

`docker-compose up -d`

#### Terminating the project

`docker-compose down`

#### Terminating the project and removing volumes

`docker-compose down --volumes`

## Deployment

#### Rsync file changes

`rsync -av -progress --chmod=Du+rwx -e "ssh -i ~/path/to/keypair.pem" ~/path/to/local/files user@ec2.endpoint:/absolute/path/on/server` 

#### SSH into server

`ssh -i your-aws-keypair.pem user@ec2.endpoint.com`

#### Start container

`docker-compose up -d`

#### Stop container

`docker-compose down`

