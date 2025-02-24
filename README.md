# Informe OSINT sobre Correo Electrónico

![Portada](/img/portada.png)

# Índice
- [1. Introducción](#1-introducción)
    - [1.1. Objetivo](#11-objetivo)  
    - [1.2. Alcance](#12-alcance)

- [2. Metodología](#2-metodología)
    - [2.1. Fuentes y Herramientas Utilizadas](#21-fuentes-y-herramientas-utilizadas)  
    - [2.2. Proceso de Investigación](#22-proceso-de-investigación)

- [3. Resultados](#3-resultados)
    - [3.1 Información Encontrada](#31-información-encontrada)

- [4. Conclusiones y Recomendaciones](#4-conclusiones-y-recomendaciones)
    - [4.1. Conclusiones](#41-conclusiones)  
    - [4.2. Recomendaciones de Seguridad](#42-recomendaciones-de-seguridad)

- [5. Referencias](#5-referencias)


## 1. Introducción

### 1.1. Objetivo
El objetivo de este informe es documentar el proceso de recopilación de información mediante técnicas OSINT (Open Source Intelligence) sobre una dirección de correo electrónico específica, con el consentimiento del propietario. La investigación busca analizar la presencia del correo en diversas fuentes abiertas y evaluar los riesgos de exposición de datos personales.


### 1.2. Alcance
Este informe se enfoca exclusivamente en la información disponible en fuentes abiertas, respetando la ética y las normativas de privacidad vigentes. Se utilizarán herramientas de búsqueda y análisis de datos para identificar posibles filtraciones, registros en sitios web, presencia en redes sociales y otros elementos relacionados con la dirección de correo electrónico investigada. No se realizarán actividades de acceso no autorizado a sistemas o violaciones de términos de servicio de ninguna plataforma.


## 2. Metodología

### 2.1. Fuentes y Herramientas Utilizadas
Para la investigación se emplearon diversas herramientas OSINT que permitieron la recolección, verificación y análisis de la información:
- **Have I Been Pwned**: Verificación de filtraciones de datos.
- **Google Dorks**: Búsqueda avanzada en Google para rastrear menciones del correo.
- **Epieos**: Identificación de registros en sitios web y plataformas.
- **Wayback Machine**: Recuperación de información histórica de sitios web.

### 2.2. Proceso de Investigación
La investigación comenzó con la recolección inicial de información del correo electrónico objetivo, asegurando el consentimiento del propietario. Posteriormente, se realizaron consultas en bases de datos de filtraciones para identificar si el correo había sido comprometido en incidentes previos. Se llevaron a cabo búsquedas avanzadas en motores de búsqueda utilizando técnicas de Google Dorks, lo que permitió rastrear menciones del correo en diferentes sitios web.

Además, se analizó la presencia del correo en redes sociales y plataformas públicas, verificando posibles perfiles asociados. Para complementar la investigación, se examinaron registros en sitios web y dominios utilizando herramientas especializadas en validación de correos electrónicos.Todos los datos obtenidos fueron validados y analizados con el fin de identificar posibles riesgos asociados a la exposición del correo electrónico.


## 3. Resultados

### 3.1. Información Encontrada
- **Filtraciones de datos**:
Para la búsqueda de las filtraciones de datos la principal herramienta utilizada fue `Have I Been Pwned`:

    ![Have I Been Pwned](/img/have-i-been-pwned.png)

    Como se puede comprobar el correo ha sido filtrado en 4 sitios distintos, aquí podemos ver de cuáles se trata:
    ![Have I Been Pwned](/img/have-i-been-pwned-2.png)

- **Presencia en redes sociales**:
Si escribimos el correo en Google directamente no aparece nada, en cambio si buscamos tan solo `gon07ps` nos aparece una cuenta de Instagram, Twitter, Pinterest, comentarios en vídeos de TikTok...
![Búsqueda Google](/img/busqueda-google.png)

- **Registros en sitios web**:
Para la búsqueda de los sitios webs donde está registrada la cuenta, usamos la herramienta `Epieos`:
Introduciendo el correo, podemos ver que ha sido filtrado en 4 webs, como nos indicaba anteriormente la herramienta `Have I Been Pwned`.

    ![Páginas filtradas](/img/epieos-1.png)

    También podemos comprobar como nos muestra que el perfil está registrado en `Trello`:
    ![Información Trello](/img/trello.png)

    Además podemos ver algunas páginas donde este correo está registrado:

    ![Cuentas](/img/webs-registradas.png)


    Por último, la herramienta que más información ha dado, ya que nos da links al perfil de Google Plus antiguo del usuario `gon07ps@gmail.com`:

    ![Datos Google](/img/datos-google.png)

    A través de Wayback Machine, encontramos 48 URLs relacionadas con el usuario:
    ![Google Plus](/img/google-plus-1.png)

    Si pinchamos en el primer enlace que nos muestra encontramos lo siguiente:
    ![Google Plus](/img/google-plus-2.png)
    ![Google Plus](/img/google-plus-3.png)


    A partir de está página encontramos información muy relevante, como su nombre, se llama `Gonzalo` y parece que posee dos blogs, comprobamos a través de la URL si siguen funcionando:
    ![Blog](/img/blog-1.png)

    A través de este blog encontramos su autor, de nombre `Gonzalo Pulido Sánchez`, en el otro blog encontraremos también esa información, ademas de una entrada:
    ![Blog](/img/blog-2.png)

    Una vez tenemos el nombre, vamos a Google en búsqueda de más información. Lo primero que obtenemos es un perfil de Linkedin:
    ![Linkedin](/img/linkedin.png)
  
    A través de Linkedin, obtenemos información acerca de dónde vive, que ha estudiado, dónde lo ha estudiado e información muy relevante sobre el usuario.

## 4. Conclusiones y Recomendaciones

### 4.1. Conclusiones
La investigación ha demostrado que la dirección de correo electrónico analizada tiene una exposición significativa en fuentes abiertas. Se han identificado múltiples filtraciones de datos, registros en diversas plataformas y vínculos con información personal del propietario. Estos hallazgos resaltan la importancia de la seguridad en el manejo de información personal en línea y los riesgos asociados a la reutilización de credenciales comprometidas.

### 4.2. Recomendaciones de Seguridad
Para reducir los riesgos asociados a la exposición del correo electrónico, se sugieren las siguientes acciones:
- **Cambio de credenciales**: Se recomienda modificar las contraseñas de las cuentas asociadas al correo, especialmente en plataformas afectadas por filtraciones.
- **Habilitación de autenticación en dos pasos (2FA)**: Implementar medidas de seguridad adicionales para evitar accesos no autorizados.
- **Supervisión de presencia en bases de datos de filtraciones**: Utilizar herramientas como Have I Been Pwned de manera periódica para detectar nuevas exposiciones de datos.
- **Uso de un gestor de contraseñas**: Para generar y almacenar credenciales seguras y evitar la reutilización de contraseñas.
- **Revisión de privacidad en redes sociales**: Ajustar la configuración de privacidad en redes sociales para minimizar la exposición de información personal.

## 5. Referencias
- Hunt, T. (s.f.). *Have I Been Pwned?*. [https://haveibeenpwned.com/](https://haveibeenpwned.com/)
- Google. (s.f.). *Google Dorks - Advanced Search Operators*. [https://www.google.com/](https://www.google.com/)
- Epieos. (s.f.). *Email Lookup Tool*. [https://epieos.com/](https://epieos.com/)
- Internet Archive. (s.f.). *Wayback Machine*. [https://web.archive.org/](https://web.archive.org/)