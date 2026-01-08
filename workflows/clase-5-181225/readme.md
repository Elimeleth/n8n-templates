# Configurar google sheets
1. Ingresar en la [consola de google](https://console.cloud.google.com/)
2. Habilitar Google Sheets y Drive

[Sheet Api](https://console.cloud.google.com/marketplace/product/google/sheets.googleapis.com)
[Drive Api](https://console.cloud.google.com/marketplace/product/google/drive.googleapis.com)

3. Crear cuenta de servicio
[Service Account](https://console.cloud.google.com/iam-admin/serviceaccounts)


4. Crear cuenta en groq con Github
[Groq](https://console.groq.com)
[Crear Apikey](https://console.groq.com/keys)

5. Importar archivo `reminders.xlsx` a una nueva hoja de Google Sheets
6. compartir arhchivo con el correo de la cuenta de servicio
7. Configurar la columna ID (A:2) `=ARRAYFORMULA(SI(LARGO(B2:B)=0; ; FILA(B2:B)-FILA(B2)+1))`