# Product Microservice

## Dev

1. Clone the repository
2. Install dependencies
3. Create a `.env` file based in the `env.template`
4. Run prisma migrations `npx prisma migrate dev`
5. Run `npm run start:dev`


## Problemas y Respuestas
1. No se levanta el contenedor de ms-products y sale un error de invocación del message pattern. Revisar si tenemos al menos un archivo de migración, si no hay podemos crear uno con el siguiente comando:
```
npx prisma migrate dev --name init
```