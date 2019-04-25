# Crear arquetipo Java Spring Boot Maven

* Crear proyecto https://start.spring.io/
* Descargar dependencias de proyecto para que pueda ser compilado (ya sea comando mvn o eclipse)
* Abrir cmd y ejecutar con versión java 8
* Ir al directorio del proyecto
* Ejecutar mvn archetype:create-from-project

Archetype project created in D:\otros\workspace_seba\prueba-arquetipo\target\generated-sources\archetype

* Subir al git los directorios internos de la ruta anteriormente extraida

# Usar arquetipo Java Spring Boot Maven

* Descargar proyecto via git
git clone https://github.com/smontecinos/spring-boot-basic-archetype.git
* Ejecutar el comando en la raíz del proyecto
mvn clean install
* Dirigirse a una nueva carpeta donde se quiera crear un proyecto, debe estar vacía
* Ejecutar el comando cambiando los datos de DgroupId, DartifactId, Dversion según se requiera

mvn archetype:generate -DarchetypeGroupId=cl.arquetipo -DarchetypeArtifactId=prueba-arquetipo-archetype -DarchetypeVersion=0.0.1-SNAPSHOT -DgroupId=my.groupid -DartifactId=my-artifactId -Dversion=1.0.0
