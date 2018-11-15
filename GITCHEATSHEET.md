# GIT Cheat Sheet

Recetas GIT

## Obtener ayuda

### Ayuda del manual

Para obtener ayuda del manual sobre el comando `config`:

```bash
$ git help config
```

Para obtener ayuda del manual sobre el comando `add`:

```bash
$ git help add
```

### Ayuda breve de la lína de comandos

Para obtener ayuda breve sobre el comando `config`:

```bash
$ git config -h
```
Para obtener ayuda breve sobre el comando `add`:

```bash
$ git add -h
```

## Crear un repositorio

Parado en el directorio del proyecto

```bash
$ git init
```
Esto crea un nuevo directorio `.git` que contendrá todos los archivos del repositorio. En esta instancia ningún archivo será trackeado por Git.

## Agregar archivos para que sean trackeados

```bash
$ git add *.md
$ git add LICENSE
```

## Clonar un repositorio

Obtiene una copia completa de un repositorio existente. Se obtiene cada una de las versiones de cada archivo del historial del proyecto.

```bash
$ git clone https://github.com/libgit2/libgit2
```
Eso crea un directorio llamado libgit2, inicializa el directorio .git, descarga todos los datos para ese repositorio, y genera una copia de trabajo de la última versión. Si entras en el nuevo directorio libgit2 que se acaba de crear, verás allí todos los archivos del proyecto, listos para usarlos y trabajar.

## Verificar el estado de los arhivos

```bash
$ git status
```

## Configuración

Git viene con una herramienta llamada `git config` que permite obtener y configurar variables de configuración que controlan
todos los aspectos de cómo se ve y funciona Git. En Windows, estas variables quedan almacenadas en tres lugares diferentes:

Archivo|Impacto|Opcion
-------|--------|-----
`C:\Program Files\Git\mingw64\etc\gitconfig`|Todos los repositorios|`--system`
`c:\users\$user\.gitconfig`|Repositorios del Usuario| `--global`
`.git\.gitconfig`|Repositorio del proyecto| `--local`

Para configurar el usuario y correo a utilizar en todos nuestros proyectos:

```bash
$ git config --global user.name "Username"
$ git config --global user.email user@example.com
```

Para ver qué opciones tenemos configuradas

```bash
$ git config --list
```

Para ver qué opciones tenemos configuradas y en qué arhivos:

```bash
$ git config --list --show-origin
```
## Información adicional

- [Documentación completa](https://git-scm.com/doc) (incluye libros y videos en inglés).
- [Libro Pro Git](https://git-scm.com/book/es/v2) (en español)
