# Configuraciones necesarias

1. Actualizar n8n y crear servicio typesense

```bash
    docker compose up -d
```

2. Configurar api typesense en n8n
  - Dirigirse a [TuNetLink](https://tunetlink.conglomere.com/app/ingress)
  - Crear nuevo hostname; parametros:
    [ protocolo ] http /
    [ servicio o IP ] localhost /
    [ puerto ] 8108 /
  - Copiar url para usarla en los nodos HTTP de n8n referente a typesense
  - Configurar apikey typesense
        name: `x-typesense-api-key`
        value: `xyz123`

---

3. Ir al flujo `"Upload to Typesense 150126"` correr el nodo `"create typesense collection"`
4. Clicar boton `"Execute workflow"` para cargar los datos 
5. Esperar que se carguen los datos 100/100

---

6. Ir al flujo `"Clase 7 - Asistente de salud 150126"`
7. Configurar groq con credenciales
8. Configurar redis
    DEJAR VACIO LOS SIGUIENTES CAMPOS: user, password
    UNICAMENTE CAMBIAR EL CAMPO HOST: cambiar localhost por `"redis"`
9. Configurar la url del nodo `"search_products"`

---

ID DE GOOGLE SHEETS: `1H27Acajv7Q5DcaVa09Xjm5GSTBxEBn9dqLYq8LPia-E`

URL DASHBOARD TYPESENSE: [DASHBOARD](https://typesense.printo.in)
Configurar:
    [ protocolo ]: http /
    [ host ]: localhost /
    [ puerto ]: 8108 /
    [ path ]: DEJAR VACIO /

- Clicar login
---

# Videos relacionados con la clase
  1. Configurar Groq en n8n
    [groq n8n](https://www.youtube.com/watch?v=bLGS9EaBRyo&pp=ygUIZ3JvcSBuOG4%3D)
  2. Configurar redis en n8n
    [redis n8n](https://www.youtube.com/watch?v=qbmv41i7Q0k&pp=ygUUY29uZmlndXJhciByZWRpcyBuOG4%3D)
  3. Loops en n8n
    [loops en n8n](https://www.youtube.com/watch?v=f5AerjPEn-A&pp=ygUJbG9vcHMgbjhu)