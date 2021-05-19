# Reto Platzimaster de Django


Ejercicio 1.
1. Crea un proyecto para la aplicación encuestas dentro de tu repositorio de código
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    pip3 install -r requirements.txt

    # Creación del proyecto
    django-admin startproject surveys
    ```

2. Configura la base de datos y las opciones locales (idioma, zona horaria)
3. Sincroniza la base de datos.
4. Lanza el servidor interno de django y comprueba que funciona el proyecto

Ejercicio 2
1. Activa el admin de Django para la aplicación encuestas
    ```bash
    python3 manage.py startapp pollster
    python3 manage.py startapp survey
    ```
2. Diseña una clase para administrar las encuestas
3. Relaciona las opciones mediante un inline
4. Configura los fieldsets
5. Haz que se vea bien el plural de Opcion
6. Mejora la página de listados de encuestas:
    * Que se vean bien las columnas de datos
    * Opción para buscar
    * Añade list_filter y date_hierarchy
7. Cambia el nombre de la aplicación para que no se vea: Administración de Django
8. Haz que al entrar en el admin, vaya directamente a la aplicación de encuestas.
9. Añade en el listado de las encuestas el número total de votaciones que ha tenido cada una.

Ejercicio 3.
1. Diseña las urls para que se pueda acceder a:
    1. Listado general de todas las encuestas
    2. Detalle de una encuesta
    3. Resultado de las votaciones de una encuesta
    4. Acción de votar una encuesta
2. Hazlo en un fichero urls.py dentro de la aplicación y enlázalo desde el urls.py general del proyecto 
3. Escribe las cuatro vistas para las acciones anteriores.
4. Escribe las plantillas necesarias. Configura el directorio de templates dentro de settings.py