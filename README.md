# Ejercicio Fundamentos de GIT

El primer paso es inicializar un repositorio de git para dar seguimiento a los cambios del proyecto

```bash
git init    
```

Para crear el primer commit se debe agregar al stage y posteriormente hacer el commit

```bash
git add README.md
git commit -m "Creacion del README.md"
```

Se crea un archivo `.gitignore` en la raíz del proyecto y se especifican los archivos a ignorar

En este caso se ignora el archivo **historia.log**

```gitignore
logs/historia.log
```

Se eliminaron todos los archivos excepto el README y después se recuperaron con:

```bash
git checkout -- .
```

> Devuelve los archivos de su copia de trabajo al estado del último commit (sin tocar los archivos sin seguimiento). Básicamente descarta los cambios no confirmados

# Subir repositorio a github con git

Una vez inicializado el repositorio solo de forma local.

Se crea un repositorio en github vacío para posteriormente extraer el enlace correspondiente que apunte a este.

Para este caso:

`https://github.com/Leo-Zubiri/Fundamentos-GIT.git`

```bash
git remote add https://github.com/Leo-Zubiri/Fundamentos-GIT.git

git push -u origin main
```

> Actualmente la llama principal es llamada **main**, anteriormente era más común que se llamara **master**