**README: Explicación de Alias Personalizados de Git**

### Alias: `ea`
Este alias está configurado para proporcionar una salida de registro concisa e informativa. Desglose de los componentes:

- `log`: Inicia el comando de registro.
- `--pretty=format:'%h %s | %d [%an]'`: Define un formato de registro personalizado para mostrar la información del commit de manera legible. Incluye el hash del commit abreviado (%h), el mensaje del commit (%s), los nombres de las ramas o etiquetas (%d) y el nombre del autor (%an).
- `--graph`: Agrega una representación de arte ASCII del gráfico de historial de commits.
- `-n 5`: Limita la salida del registro a los últimos 5 commits.

Ejemplo de uso:
```bash
git ea
```

### Alias: `eb`
Este alias está diseñado para crear una salida de registro detallada y colorida. El desglose es el siguiente:

- `log`: Inicia el comando de registro.
- `--graph`: Agrega una representación de arte ASCII del gráfico de historial de commits.
- `--abbrev-commit`: Muestra los hashes de commit abreviados.
- `--decorate`: Resalta ramas, etiquetas, etc.
- `--format=format:'%Cred%h%C(reset) %C(yellow)%d%C(reset) %s %Cgreen(%ar)%C(reset)'`: Define un formato de registro personalizado con códigos de colores para una mejor visibilidad. Incluye el hash del commit (%h), decoraciones (%d), mensaje del commit (%s) y fecha relativa del commit (%ar).
- `--all`: Muestra todas las referencias, no solo las ramas locales.

Ejemplo de uso:
```bash
git eb
```

### Alias: `last`
Este alias simplifica el comando para mostrar el último commit en la rama actual:

- `log -1 HEAD`: Muestra el último commit en la rama actual.

Ejemplo de uso:
```bash
git last
```

### Alias: `ec`
Este alias es un atajo para editar el archivo de configuración global de Git:

- `config --global -e`: Abre el archivo de configuración global de Git en el editor de texto predeterminado.

Ejemplo de uso:
```bash
git ec
```

Siéntete libre de personalizar y usar estos alias según tus preferencias. Para agregar más alias o modificar los existentes, puedes editar directamente tu archivo de configuración global de Git o usar el comando `git config`.