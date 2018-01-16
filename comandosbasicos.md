
![ComandosBasicos][1]



![SistemaArchivos1][2]


![SistemaArchivos2][3]

### Ubicación de archivos y directorios


**/home/usuario/documento6.txt**

Para facilitar las cosas existen ciertos directorios especiales:  

| Símbolo | Descripción |
| ------------- | ------------- |
| **/** | Es el directorio raíz. El superior de todos. |
| **.** | Es el directorio actual. En el que nos encontramos en un momento dado. |
| **..** | Es el directorio superior, o directorio padre, al que nos encontramos. |  


##### Ruta absoluta
Una ruta absoluta es aquella que parte del directorio raíz. Las rutas absolutas son válidas en cualquier caso.

/home/usuario/.bashrc

/home/raco/Documentos/Directorio\ De\ Respaldo/

"/home/raco/Documentos/Directorio De Respaldo"

##### Ruta relativa
Es una ruta que parte del directorio actual como origen. Esta ruta sólo es válida desde un directorio actual concreto, es decir, es relativa a un directorio.

../../etc/

../../swapfile


### Introducción a los comandos en un sistema GNU/Linux
Los directorios estándar para almacenar archivos ejecutables (comandos) en un sistema tipo Unix:  

/bin  
/usr/bin  
/usr/local/bin  
/sbin  
/usr/sbin  
/usr/local/sbin  

Estos directorios son almacenados en una variable que la shell consulta para la busqueda de archivos que coincidan con la instrucción escrita por el usuario.  


**pwd**: print working directory  

>raco@castu:~$ pwd  
>home/raco

**cd**: change directory

cd directorio

>raco@castu:\~$ cd Documentos/   
>raco@castu:\~$ pwd  
>home/raco/Documentos    

**ls**: list directory contents

>raco@castu:\~$ ls Archivos/  
>archivo1.txt  archivo2.txt  Respaldo  


>raco@castu:\~$ ls -l Archivos/  
>-rw-r--r--  1 raco raco   34  dic 18 05:13 archivo1.txt  
>-rw-r--r--  1 raco raco   79  dic 18 05:13 archivo2.txt  
>drwxr-xr-x  2 raco raco 4096  dic 18 05:14 Respaldo  

**mkdir**: create directory

mkdir nombre_directorio

>raco@castu:\~$ mkdir prueba  
>raco@castu:\~$ ls -l 

**cp**: copy files and directories

cp [opciones] [ruta]origen [ruta]destino

• -i Pregunta si debe sobreescribir cada fichero destino que exista. Si la respuesta no
comienza por ’y’ o por ’Y’ (o quizá el equivalente local, en español ’s’ o ’S’) no se
borra.  
• -r Copia recursivamente los contenidos de directorios.  
• -a Preserva los atributos del fichero copiado en la medida de lo posible.  

Copiar el fichero perso (que se encuentra en /home/raco/) en el directorio prueba.  

>raco@castu:\~$ cp /home/raco/perso  /home/raco/prueba/  
>raco@castu:\~$ cd prueba/  
>raco@castu:\~$ ls  
>perso  












[1]: Imagenes/ComandosBasicosLinux.jpg
[2]: Imagenes/SistemaDeArchivos1.PNG
[3]: Imagenes/SistetmaDeArchivos2.png
