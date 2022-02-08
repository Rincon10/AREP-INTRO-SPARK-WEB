# **LAB01-AREP INTRO-SPARK-WEB**

Introducción MVN, GIT, Heroku y SPARK WEB, para esto manejamos creamos un programa que permite convertir valores de temperatura equivalentes en las escalas Celsius y Fahrenheit.

## **¿Cómo empezar?**
A continuación proporcionaremos  una serie de instrucciones que le permitirán tener una copia del proyecto y ejecutarlo en su máquina de manera local.

* [Back-End](https://github.com/Rincon10/AREP-LAB01/tree/main/README.md)
* [Front-End](https://github.com/Rincon10/AREP-LAB01/tree/main/README.md)




## **Prerrequisitos**

-   [Git](https://git-scm.com/downloads) - Sistema de control de versiones
-   [Maven](https://maven.apache.org/download.cgi) - Gestor de dependencias
-   [Java 8](https://www.java.com/download/ie_manual.jsp) - Entorno de desarrollo
-   [Spark](https://sparkjava.com/documentation#getting-started) - Framework Web
-   [Intellij Idea](https://www.jetbrains.com/es-es/idea/download/) (Opcional)


## **Instrucciones de ejecución local**
0. Desde cmd clonar el repositorio

```git
git clone https://github.com/Rincon10/AREP-LAB01
```

### **BackEnd**

1. Ubicarse en la carpeta App y borraremos todas las dependencias y modulos que puedan exisitir de los binarios del proyecto.
```maven
mvn clean
```

2. Realizamos la compilación del proyecto
```maven
mvn package
```

3. Ejecutamos el proyecto
```maven
mvn exec:java -Dexec.mainClass="edu.escuelaing.arep.App"
```

4. Generando la documentación del proyecto
```mvn
mvn javadoc:javadoc
```
La documentación se generara en la ruta
```
target/site/apidocs/index.html
```

### **Más información**
para más información del API, seguir [aquí](https://calcapp-frontend.herokuapp.com/public/documentation.html).

### **FrontEnd**

1. Bastara con ubicarnos  en la carpeta Front-End-App y dirigirnos a la carpeta /public/index.html, dando click en el archivo.
2. En caso de tener el editor de código Visual Studio Code, se recomienda usar la extensión, para más información dar click [aquí](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)

## **Ejecutando pruebas**
Para la ejecución de pruebas

```mvn
mvn test
```

 En este taller tenemos dos casos de pruebamostrando la respectiva conversión  Celsius-Fahrenheit y viceversa.

## **Diagramas**

## **Heroku Deployment**

### **Back-End**

[![Deployed to Heroku](https://www.herokucdn.com/deploy/button.png)](https://calcapp-backend.herokuapp.com/api/v1/celsius/1)

### **Front-End**

[![Deployed to Heroku](https://www.herokucdn.com/deploy/button.png)](https://calcapp-frontend.herokuapp.com/public/index.html)

## **Autor**

-   [Iván Camilo](https://github.com/Rincon10).