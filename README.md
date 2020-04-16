# Programa
Component Checker - Verificador de COM ActiveX

# Autor
Luis Leonardo Nuñez Ibarra. Año 2000 - 2003. email : leo.nunez@gmail.com. 

Chileno, casado , tengo 2 hijos. Aficionado a los videojuegos y el tenis de mesa. Mi primer computador fue un Talent MSX que me compro mi papa por alla por el año 1985. En el di mis primeros pasos jugando juegos como Galaga y PacMan y luego programando en MSX-BASIC. 

En la actualidad mi area de conocimiento esta referida a las tecnologias .NET con mas de 15 años de experiencia desarrollando varias paginas web usando asp.net con bases de datos sql server y Oracle. Integrador de tecnologias, desarrollo de servicios, aplicaciones de escritorio.

# Tipo de Proyecto
Component Checker es una aplicación que se encarga de respaldar todos los archivos que ocupa el proyecto visual basic. La aplicacion hace uso de la componente vbzip10.dll la cual es una api desarrollada por el grupo Info-ZIP. El código y las rutinas de compresión se tomaron del ejemplo de http://www.vbaccelerator.com/codelib/zip/zip.htm.

# Prologo
Regala un pescado a un hombre y le darás alimento para un día, enseñale a pescar y lo alimentarás para el resto de su vida (Proverbio Chino)

# Historia
Despues de haber desarrollado varias librerias y controles activex y haber uso de terceros no faltaba aquella componente que no podia ser instalada en un computador en particular. Dado este escenario es que decidi construir este utilitario el cual lee todas las librerias activex del directorio windows\system y verifica su estado. La información se extrae usando la libreria TLBINF32.DLL.

# Archivos Necesarios
Este proyecto ocupa 5 componentes ActiveX 

- Reference=*\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\WINDOWS\SYSTEM\StdOle2.tlb#OLE Automation
- Reference=*\G{8B217740-717D-11CE-AB5B-D41203C10000}#1.0#0#C:\WINDOWS\SYSTEM\TLBINF32.DLL#TypeLib Information
- Reference=*\G{69EDFBA5-9FEC-11D5-89A4-F0FAEF3C8033}#1.0#0#C:\WINDOWS\SYSTEM\PVB_XMENU.DLL#PVB6 ActiveX DLL - Menu With Bitmaps !
- Object={831FDD16-0C5C-11D2-A9FC-0000F8754DA1}#2.0#0; MSCOMCTL.OCX
- Object={3B7C8863-D78F-101B-B9B5-04021C009402}#1.2#0; RICHTX32.OCX

El archivo PVB_XMENU.DLL es un componente customizado para que los menus se puedan aplicar iconos y ayuda al momento de selección.

# Registro de los componentes ActiveX
Se debe realizar desde la linea de comando de windows regsvr32.exe [nombre del componente]
Para windows 10 necesitaras instalar con permisos de administrador. 

# Notas de los componentes ActiveX de Windows
Si obtienes error de licencia de componentes al momento de ejecutar el proyecto necesitaras instalar quizas la runtime de Visual Basic 5 (MSCVBM50.DLL) y bajar el archivo VB5CLI.EXE y VBUSC.EXE ambos disponibles en internet para descarga. Esto corregira los problemas de licencia de componentes de VB5.

# Desarrollo del proyecto
Dada la facilidad con la cual visual basic te permite construir librerias y controles activex tanto para uso personal como para los proyectos en los cuales trabajaba para esa epoca y tenias que ir a instalar la aplicacion en el pc del usuario final y el instalador se caia porque no era capaz de resolver la instalacion de la libreria o bien quedaba mal instalada porque faltaba un componente externo que esta usaba.

Era la epoca del DLL HELL (https://en.wikipedia.org/wiki/DLL_Hell) y muchos desarrolladores de la epoca que usabamos Visual Basic sufrimos con ella. Para ayudar a mitigar un poco este problema y verificar cual componente estaba bien instalado fue que desarrollo este utilitario para ayudar a tener una idea de cuales componentes estaban bien instalados.

Resolver el DLL HELL no era facil ...

# Freeware
Por esos años mi intención fue ofrecerlo gratis a la comunidad Visual Basic que era bastante activa por esos años. Para esto levante un sitio web donde tenia varias otras aplicaciones que tambien habian sido creadas de la necesidad y que las distribuia de forma gratis.

# Palabras Finales
Espero que este proyecto que nacio de una necesidad personal sea usado con motivos de estudio y motivación. De como se pueden copiar las buenas ideas y mejorarlas. 
