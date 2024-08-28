# Entrega2-Jenkins

Este modelo de CI/CD está realizado en base a una petición, la misma cumple con la demanda de tomar conocimientos de como se realiza un proceso de build para una API hecha en nodejs.

Este está configurado en un webhook sobre el siguiente [Repositorio](https://github.com/briangirod/nodejs-helloworld-api)

### Ejecución

#### Comando

`$ git push origin main`

- El webhook configurado detecta el push al branch "main" y envía una solicitud a Jenkins

- Jenkins recibe la solicitud de GitHub atraves de Ngrok y ejecuta el pipeline

- Script por SCM; Si el pipeline está configurado mediante SCM, Jenkins retorna al repositorio en busca del archivo Jenkinsfile para ejecutar el Pipeline según lo especificado.

- Script predefinido; Si el Pipeline ya posee un Script predefinido en su configuración, ejecutará automaticamente.

### Diagrama de Flujo

![](https://github.com/briangirod/Entrega2-Jenkins/blob/main/Diagrama%20Jenkins-Github.png?raw=true)
