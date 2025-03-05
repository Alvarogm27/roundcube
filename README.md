Agregar linea "nameserver 127.0.0.1" a etc/resolv.conf.

Editar el archivo /etc/systemd/resolved.conf:

sudo nano /etc/systemd/resolved.conf

Agregar o editar la siguiente línea para que systemd-resolved use otro puerto:

DNSStubListener=no

Reiniciar el servicio:

sudo systemctl restart systemd-resolved
