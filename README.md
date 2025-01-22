# CVDS G01 Laboratorio #1 INTRODUCCION A GIT

### Integrantes
- Sergio Andrey Silva
- Juan Esteban Lozano 


### Respuestas
## PARTE I (Trabajo Individual). 

### 1. Crea un repositorio localmente.

Elegir incialmente el directorio donde estara el respositorio, en este caso, se hara en el *Escritorio*

Se usa *Shift + Clic Derecho*, y en la opcion de la terminal Bash de Git (Git Bash) en la opcion *Open Git Bash here*

![image](Screenshots/screen1.png)

A continuacion se crea la carpeta llamada Lab1CVDS, luego se entra alli, y se inicializa el repositorio local con el comando: 

```
git init
```

![image](Screenshots/screen2.png)

### 2. Agrega un archivo de ejemplo al repositorio, el **README.md** puede ser una gran opción.

Para agregar el archivo `README.MD`, se usa:

```
echo "LAB1 README FILE !!!" > README.md
```
El comando echo junto a la cadena de texto funciona para crear un archivo con dicho contenido.

### 3. Averigua para qué sirve y como se usan estos comandos git add y git commit -m “mensaje”

- `git add`: Git Add toma tus archivos modificados y los coloca en el área de preparación, 
también conocida simplemente como "el índice". Esta área de almacenamiento provisional es 
un estado intermedio. Los archivos permanecen almacenados provisionalmente hasta que se 
confirman. Sin este paso, Git no sabrá qué cambios tienes la intención de incluir en tu 
próxima confirmación.

  Este comando prepara todos los archivos modificados, excluyendo los ignorados por *.gitignore*. Internamente 
  Git está creando una lista de cambios (un registro de contenido nuevo y líneas eliminadas) que serán 
  incluido en la siguiente confirmación. Piense en ello como organizar los papeles en su escritorio antes de colocarlos 
  en una carpeta. El área de preparación garantiza que tenga control sobre lo que entra en cada uno 
  instantánea, lo que le permite dividir los cambios en fragmentos significativos y mantener una imagen limpia 
  Historial de confirmaciones.

- `git commit`: Después de preparar los cambios con git add, el siguiente paso es git commit. La 
  ejecución de git commit transforma lo que hay en el área de preparación en una instantánea 
  inmutable almacenada en el historial del repositorio de Git. A cada confirmación se le asigna 
  un hash único (una suma de comprobación criptográfica) para identificarla. Este hash es
  básicamente un ID vinculado a esa versión exacta de sus archivos.

[Referencia-graphite.dev](https://graphite.dev/guides/git-add-commit-push)


### 4. Abre una cuenta de github, si ya la tienes, enlazala con el correo institucional.

Actualmente ya tenia una cuenta con nombre de usuario [OneCode182](https://github.com/OneCode182)

Hice la configuracion y vincule mi correo institucional *sergio.silva-r@mail.escuelaing.edu.co*

![img](Screenshots/screen3.png)

### 5. Crea un repositorio en blanco (vacío) e GitHub.

![img](Screenshots/screen4.png)

### 6. Configura el repositorio local con el repositorio remoto.

Para realizar la vinculacion, se usa la sintaxis

```
git remote add origin "LINK"
```