## Proyecto de Sistema de Citas Médicas 

En qué consiste este proyecto?
- Gestionar médicos y especialidad y agendas, asignado por Evelyn Manzaba.
- Crear una agenda para disponer de citas, asignado por José Luis Rosales.
- Permitir al usuario elegir una cita en día y hora según la agenda del médico, asignado por Ernesto Acosta.

## Configurar el entorno para ejecutar la aplicación web.
Descarga este repositorio:

```
$ https://github.com/Evelyn-MS/medicos-zeta.git
```

Crear una máquina virtual e instalar las librerías disponibles en el archivo 
requirements.txt:

Entra en la carpeta que has creado e inicia un entorno virtual:
```
$ cd proyecto_clinica
$ python3 -m venv venv
```
Luego debes activarlo con el siguiente comando:

```
$ source ./venv/bin/activate
```
Una vez activado, instala las librerías necesarias para ejecutar el proyecto:
```
 (venv)$ pip install -r requirements.txt
```
Para obtener el primer acceso y configurar la aplicación ejecutaremos el comando 
migrate' para generar la base de datos por defecto de Django (SQLite). Y luego crear el superusuario:
```
(venv)$ ./manage.py migrate
(venv)$ ./manage.py createsuperuser
Apellido/Usuario: admin
Correo electrónico: admin@mail.com
Contraseña: 
Contraseña (de nuevo):
```

Para iniciar el servidor después de este paso debe:
```
(venv)$ ./manage.py runserver
```


Para ver si todo está funcionando como se espera vaya a la siguiente dirección:
[http://localhost:8000/](http://localhost:8000/)

O puedes acceder al admin de Django:
[http://localhost:8000/admin](http://localhost:8000/admin)
