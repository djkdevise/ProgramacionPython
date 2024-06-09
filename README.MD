# Python es un versátil lenguaje de programación de alto nivel disponible en múltiples plataformas. Es un lenguaje que utilizan compañías grandes y pequeñas, para crear un rango diverso de aplicaciones. Algunas áreas en las que se utiliza Python dentro del desarrollo web, son el análisis de datos y los pronósticos de negocios. 

* **Consola:**  python --version, 

**Características clave:**

* **Interpretado:** Se compila a código máquina antes de la ejecución.
* **Sin punto y coma:** En Python, el punto y coma; es decir, el carácter ;, se utiliza para delimitar claramente partes del código de otras partes del código

* **Tipado dinámico:** El tipo de dato de una variable se determina en tiempo de ejecución.
* **Orientado a objetos:** Todo es un objeto, lo que lo hace un lenguaje flexible.
* **Productivo:** Ahorra tiempo de desarrollo gracias a su sintaxis concisa.
* **Clases flexibles:** Permiten una gran variedad de posibilidades.
* **Lenguaje natural:** La sintaxis se asemeja al lenguaje humano, lo que lo hace más legible.

**Aplicaciones:**

* **Desarrollo web:** Python tiene framework populares Flask, Django, y FlaskApi para crear aplicaciones web robustas.
* **Utilidades de la terminal:** Python es ideal para crear scripts y automatizar tareas.
* **React:** Marco para crear aplicaciones web escalables.


**En resumen, Python es un lenguaje versátil y potente que se puede utilizar para una amplia variedad de aplicaciones.**

**Aquí hay algunos ejemplos de las ventajas de usar Python:**
bre
* **Fácil de aprender:** Python también es muy sencillo de aprender y empezar a utilizar. Dado que la sintaxis se asemeja al idioma inglés, es sencillo leerla y descifrarla.
* **Potente:** Python está en una posición única  Se usa ampliamente en todas las áreas de negocio, como desarrollo web, inteligencia artificial, aprendizaje automático, análisis de datos y diferentes aplicaciones de programación.
* **Flexible:** Es un lenguaje de programación de alto nivel que funciona en muchas plataformas diferentes. 
* **Comunidad activa:** Python tiene una comunidad grande y activa que ofrece soporte y recursos.

**Si estás buscando un lenguaje de programación que sea fácil de aprender, potente y flexible, Python es una excelente opción.**

**Comentarios:**
* **Linea**  // este es un comentario.
* **Bloque** /*
        este 
        es 
        un 
        comentario 
        de 
        varias 
        líneas 
        */

* **Varias lineas en una:** /*este es un comentario de varias líneas en una sola línea */

**Variables:**
* **Tipado:** Dinamico no se necesita declarar el tipo de dato de la variable. Ej: nombre_variable= "Hola"
* **Notacion:** snakecase ejemplo: nombre_de_variable  a ecepcion nombre de clases que se usa camelcaase
* **Palabras reservadas:** new, put, iniciar nombre con mayusculas o numero.








# Instalar rutas de Python (opcional para usuarios de Mac)

Dependencias necesarias
Al finalizar esta lectura, podrá identificar las dependencias necesarias para su sistema operativo.

Configurar Python en Windows es sencillo y se instalará sin ninguna dependencia necesaria. En Mac, sin embargo, se necesitan algunas dependencias adicionales antes de instalar Python.

XCode
Para instalar "brew", primero debe instalar Xcode. Homebrew no viene con su propio compilador y necesita tener instalado Xcode para funcionar correctamente. Para instalar Xcode realice estos pasos:

Abra una terminal.

Ejecute lo siguiente: 

shell xcode-select --install

Aparecerá una ventana emergente pidiéndole que confirme la instalación. Haga clic en el botón "Install" (Instalar).

Acepte el acuerdo de licencia.

brew
Las Mac no incluyen gestores de paquetes como la mayoría de distribuciones de Linux. Para compensarlo, se creó una herramienta externa llamada brew. Para instalar brew, haga lo siguiente:

'''
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
'''
Si desea trabajar en su dispositivo local y tiene una computadora Apple Mac necesitará instalar Python 3. Por defecto, una Apple Mac tiene instalado Python con la versión 2.7. Para verificarlo, abra una terminal y ejecute el siguiente comando: 

python --version  

Para las lecciones de este curso, necesitará Python 3. 

Antes de instalar Python, deberá instalar algunas dependencias.  Estas son "XCode" y "brew".  Encontrará los detalles en la lectura de "Dependencias requeridas". Mac tiene varias formas de realizar instalaciones, pero la forma más común es utilizar el administrador de paquetes denominado "brew" para manejar las instalaciones.

Una vez instaladas las dependencias, puede comenzar a instalar Python. Ejecute el siguiente comando: 

brew install python  

Cuando instale Python a través de brew, instalará la versión 3.x. Para verificar que tiene ambas versiones instaladas ejecute lo siguiente:

python --version  

python3 --version  

Para reducir la confusión, es necesario establecer las rutas para que apunten a la instalación de "brew" de Python3. Primero, veamos dónde lo instaló el administrador de paquetes "brew". Ejecute el siguiente comando: 

brew info python  

La sección que le interesa es la ubicación de donde se instaló. 

Unversioned symlinks `python`, `python-config`, `pip` etc. pointing to `python3`, `python3-config`, `pip3` etc., respectively, have been installed into   /opt/homebrew/opt/python@3.9/libexec/bin  

El /opt/homebrew/opt/python@3.x/libexec/bin es el que quiere utilizar y establecer para su ruta. Cópielo desde la terminal. Según la versión de Mac OS que ejecute, los siguientes pasos pueden variar un poco. 

Zsh
vim ~/.zshrc  


Bash 
vim ~/.bashrc  


Vim es un editor de texto que permite realizar cambios en los archivos directamente desde el "shell". Para realizar las modificaciones:

1. Pulse la tecla "I" de su teclado.
2. Agregue la línea siguiente y recuerde reemplazar 3.x con la versión de Python que se instaló en su sistema: 

shell PATH="/opt/homebrew/opt/python@3.x/libexec/bin:${PATH}" 

3. Pulse la tecla esc para salir del modo de inserción. 

4. Mantenga pulsada la tecla shift y pulse la tecla colon representada por : y  ; 

5. Escriba wq! y luego pulse Enter para salir de vim. 

6. Ejecute lo siguiente: 

Zsh shell source ~/.zshrc 

Bash shell source ~/.bashrc 

7. Para verificar que todo funciona correctamente, ejecute lo siguiente: 

shell python --version Python 3.9.10 

8. Debería ver la salida similar a la anterior según su versión de instalación.  
