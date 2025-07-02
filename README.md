# Configuración de n8n para servirlo en cualquier plataforma usando Docker

### Requisitos previos

- Docker

## Cosas a tener en cuenta

Si ya usas un proxy reverso como nginx, asegúrate de que la configuración de n8n no esté en conflicto con la configuración del proxy reverso, ya que por defecto se expone el puerto 443 por parte de traefik y si ya esta siendo en uso por otro servicio, n8n no podrá iniciar correctamente sin su certificado.

Si ya tienes nginx instalado, puedes usarlo para servir n8n y configurarlo para que funcione con HTTPS. Asegúrate de que el proxy reverso esté configurado correctamente para redirigir las solicitudes a n8n.
