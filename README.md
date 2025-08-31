## Gateway
Es el encargado de la comunicación entre nuestros clientes y nuestros servicios.
Recibe peticiones y las envia a los servicios correspondientes, devolviéndole la respuesta al cliente

# Product Microservice

## Dev

1. Clonar el repositorio
2. Instalar Dependencias
3. Crear un archivo `.env` basado en el `env.template`
4. Levantat el servidor de NATS 
```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```
5. Ejecutar migración de prisma `npx prisma migrate dev`
6. Ejecutar `npm run start:dev`

## Nats
```
docker run -d --name nats-server -p 4222:4222 -p 8222:8222 nats
```