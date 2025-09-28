apt update: actualizar los repositorios del sistema
su root
apt install openssh-server
	fla: -y

systemctl start ssh

systemctl enable ssh -> habilita el servicio de ssh al 
arrancar la máquina

systemctl restart ssh

ip a

CMD: para conectarse a ssh -> ssh debian@10.179.26.37

ls
pwd
whoami
apt install apache2
systemctl status apache2
	q: para salir
nano
cat
mkdir

www-data tanto en apache como en ngnx

chown
	chown www-data:www-data HTML
	chown -R www-data:www-data HTML
	