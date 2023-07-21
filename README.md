# Servicios de base de datos con su administrador web

## Descripción

**Para correr alguno de los servicios en docker es necesario tener instalado _Docker_.**

* [Instalar Docker](https://docs.docker.com/engine/installation/)

### Comando para correr un servicio

```bash
docker compose -f docker-compose-SERVICIO.yaml -p "Nombre identificador" up -d
```

Por defecto estos servicios se tienen que iniciar manualmente al abrir el Docker desktop, si quieres que se inicien automaticamente, reemplaza el valor "on-failure" de:

```yaml
restart: on-failure 
```

por **always** en el archivo docker-compose-SERVICIO.yaml

```yaml
restart: always 
```
