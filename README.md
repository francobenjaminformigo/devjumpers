# # GIT - GITHUB : Ejercitación Final

_Ejercitación final de **Git** y **GitHub** para el programa **DevJump** de **Arbusta**._


## Paso a paso 📋:

 - _Creación del repositorio **devjumpers**:_

	 ![creacion del repo](https://s9.gifyu.com/images/CPT2302062141-744x436.gif)


- _Clonar el repositorio:_
			
	```git clone https://github.com/francobenjaminformigo/devjumpers```

- _Navegar hacia la ruta del repositorio local y crear el archivo **README**_

	```
		cd devjumpers

		touch README.md
	```

- _Añadimos lo trabajado hasta el momento al **area de staging**:_

	``git add .``

- _Hacemos el **commit** inicial_

	``git commit -m "commit inicial"``

- _Subimos los cambios al repositorio_

	``git push``

- _Creamos el archivo **privado.txt**, la carpeta **privada** y el archivo **.gitignore** y los añadimos al mismo:_

	```
	mkdir privada
	touch privado.txt .gitignore

	------------------------------------------------------------------------------------------

	Dentro del archivo .gitignore:
	/privado.txt
	privada/
	```
- _Creamos el archivo **1.txt** y luego la rama **v0.2**:_

	```
	touch 1.txt
	git checkout -b v0.2
	```

- _Dentro de la rama **v0.2** creamos el archivo 2.txt:_

	``touch 2.txt``

- _Subimos los cambios al repositorio:_

	```
	git add .
	git commit -m "Creados archivos 1.txt y 2.txt, creados .gitignore y rama v0.2"
	git push

	------------------------------------------------------------------------------------------

	Aqui git nos arroja un error el cual solucionaremos con el siguiente comando:

	git push --set-upstream origin v0.2
	```

- _Volvemos al **main** y hacemos el merge con la rama **v0.2**:_

	``git merge v0.2``

- _Escribimos **"Hola"** en el archivo **1.txt** y commiteamos los cambios:_

	```
	echo 'Hola' >1.txt
	git add .
	git commit -m "Modificado el archivo 1.txt"
	```

- _Volvemos a la rama **v0.2** y añadimos **"Adios"** en el archivo **1.txt**: _

	```
	git checkout v0.2
	echo 'Adios' >1.txt

	git add .
	git commit -m "Modificado el archivo 1.txt en la rama v0.2"
	```

- _Volvemos al **main** y hacemos el **merge** correspondiente:_

	```
	git checkout main
	git merge v0.2
	```

- _Arreglamos los **conflictos**, hacemos un commit y probamos los commandos git branch **--merged** y **--no-merged**:_

	```
	git add .
	git commit -m "Resueltos conflictos del merge en 1.txt de la rama v0.2 con main"
	------------------------------------------------------------------------------------------
	El comando git branch --merged nos devuelve la rama main
	El comando git branch --no-merged nos devuelve la rama v0.2
	```

- _Borramos la rama **v0.2** y pusheamos los cambios:_

	```
	git branch -D v0.2
	git push
	------------------------------------------------------------------------------------------
	NOTA IMPORTANTE:
	Aquí git me arrojó un error diciendo que no podía subir los cambios ya que el repositorio
	remoto contenía cambios que yo no tenía localmente, el cual si no me equivoco creo
	que fue por editar el archivo README directamente desde el repositorio en el navegador.
	Siendo consciente de los riesgos que esto conlleva, al ser un repositorio pequeño y ser yo
	el único trabajando en él, decidi forzar el push con [git push --force]
	```

- _Hacemos un **git list**:_

	```
	git list

	*   c6858e9 (HEAD -> main, origin/main) Resueltos conflictos del merge en 1.txt de la rama v0.2 con main
	|\
	| * 1ec42f9 Modificado el archivo 1.txt en la rama v0.2
	* | 37247ed Modificado el archivo 1.txt
	|/
	* 2bb6130 (origin/v0.2) Creados archivos 1.txt y 2.txt, creados .gitignore y rama v0.2
	* dd29917 commit inicial

	```

- _GitHub Account:_

		Agregué una foto de perfil y activé 2FA

- _Uso social de GitHub:_

		Seguí a mis compañeros, así como a sus respectivos repositorios "devjumpers"
		a los cuales también les di una estrella como dicta la ejercitación

- _Tabla de compañeros:_

	
	| Nombre      | Enlace al perfil de GitHub |
	| ----------- | ----------- |
	| Armando Torres Quintana      | [Perfil de Armando Torres Quintana](https://github.com/ArmaTQ/)      |
	| Leandro Cuevas   | [Perfil de Leandro Cuevas](https://github.com/leandro-cuevas/)        |
	| Cristian Ortiz   | [Perfil de Cristian Ortiz](https://github.com/Cristian550/)        |
	| Camila Calegari   | [Perfil de Camila Calegari](https://github.com/camilacalegari/)        |
	| Alejo Paiva   | [Perfil de Alejo Paiva](https://github.com/BLUHD823/)        |

- _Colaborador elegido:_


		Armando Torres Quintana