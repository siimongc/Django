# Configuración de un Proyecto Django con Entorno Virtual

Este README te guiará paso a paso para configurar un proyecto Django, manejar entornos virtuales y trabajar con archivos de requisitos.

## 1. Crear y Activar un Entorno Virtual

Un entorno virtual es un espacio aislado donde instalas las dependencias de tu proyecto, evitando conflictos con otras aplicaciones.

### Crear el entorno virtual:

```bash
python -m venv venv
```

### Activar el entorno virtual:

- **Linux/Mac:**

```bash
source venv/bin/activate
```

- **Windows (CMD):**

```bash
venv\Scripts\activate
```

Una vez activado, verás el nombre del entorno (p. ej., `(venv)`) al inicio de la terminal.

### Desactivar el entorno virtual:

```bash
deactivate
```

## 2. Instalar Django y Dependencias

Con el entorno activado, instala Django y cualquier otra dependencia:

```bash
pip install django
```

Si ya tienes un archivo `requirements.txt`, puedes instalar todo con:

```bash
pip install -r requirements.txt
```

## 3. Crear un Proyecto Django

Para iniciar un proyecto:

```bash
django-admin startproject nombre_proyecto .
```

Esto creará la estructura básica de Django.

## 4. Archivo requirements.txt

El archivo `requirements.txt` guarda las versiones exactas de tus paquetes, facilitando la replicación del entorno.

### Crear el archivo:

```bash
pip freeze > requirements.txt
```

### Usar el archivo en otro entorno o máquina:

```bash
pip install -r requirements.txt
```

Esto asegurará que todos los paquetes y versiones se instalen tal cual.

## 5. Clonar un Repositorio y Configurar el Entorno

Al clonar un proyecto desde GitHub:

```bash
git clone https://github.com/usuario/repositorio.git
cd repositorio
```

Luego, crea y activa un entorno virtual, instala los requisitos y ya estarás listo:

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

¡Y listo! Tu proyecto estará preparado para ejecutarse sin problemas.
