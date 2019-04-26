# zabbix-grafana-docker

Requisitos:

	- Docker;
	- docker-compose
	- MySQL;

	OBS: É necessário importar o schema de banco de dados que vêm no pacote quando instalado via repositório (/usr/share/doc/zabbix-server-mysql/create.tgz), pois o entrypoint da imagem usa um schema que não cria o usuário Admin por padrão.

Instalação:

	adduser app
	gpasswd -a app docker
	chown root:docker /var/run/docker.sock
	docker-compose up -d
