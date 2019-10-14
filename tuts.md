# Implementación basica de Azure Function en Python (Windows/PowerShell)

## ¿Por qué python?

Por que hacen falta tan solo 4988 segundos para poner en pie cualquiera de las funciones plantillas... En este caso se ocupará el HttpTrigger, que es el equivalente al "Hello World" de Azure Function.

### Importante

El unico cuidado que hay que tener es OCUPAR LA VERSIÓN DE PYTHON 3.6.8 DE 64 BITS, para evitar cualquier tipo de errores.

### ¿Que se hará entonces?

Se inicializará la plantilla HttpTrigger de Azure Functions, podriamos decir que haremos un "hola mundo" usando PowerShell

* Instalar Azure Functions Tools
```sh
$ npm install -g azure-functions-core-tools
```
* Crear y activar el entorno virtual, que nos permitirá correr los comandos especiales para crear azure functions
```sh
$	py -m venv .venv
$	.venv\scripts\activate
```
* Crear un function project
```sh
	$ func init FunctionProjectName
```
* Selecciona la opcion "python"
* Ingresa al nuevo directorio creado
```sh
	$ cd FunctionProjectName
```
* Agrega una azure function al nuevo projecto
```sh
	$ func new
```
* Selecciona la opción HTTP trigger
* Ponle de nombre HttpTrigger y luego presiona Enter
* Para finalizar inicializamos el azure function
```sh
	$ func host start
```
* Luego accedemos al link que nos entrega la terminal de PowerShell -> http://localhost:7071/api/HttpTrigger
* Y para testear el azure function de HTTP Trigger modificamos la url -> http://localhost:7071/api/HttpTrigger?name=TuNombre


[command-line-grammar]: #command-line-grammar
[configuring-dns]: os/configuring-dns.md
[coreos-docs]: https://coreos.com/docs/
[economist-hyphens]: http://www.economist.com/news/books-and-arts/21723088-hyphens-can-be-tricky-they-need-not-drive-you-crazy-hysteria-over-hyphens
[eos]: https://faculty.washington.edu/heagerty/Courses/b572/public/StrunkWhite.pdf "The Elements of Style"
[githubmd]: https://help.github.com/articles/github-flavored-markdown/
[headings]: #headings
[hyperlink-considerations]: #hyperlink-considerations
[mdhome]: https://daringfireball.net/projects/markdown/syntax
[quickstart]: os/quickstart.md "Relative link from here to CoreOS Quick Start"
[rfc2606s3]: https://tools.ietf.org/html/rfc2606#section-3
[rfc5737]: https://tools.ietf.org/html/rfc5737
[style]: STYLE.md "CoreOS Documentation Style"