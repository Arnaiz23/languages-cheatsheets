# Linux Cheatsheet

## Permissions

```bash
#owner-group-others
Read - 4
Write - 2
Execute - 1
```

Example:

```bash
chmod 755 prueba
# rwx-rx-rx prueba
```


## Pacman cheatsheet

**Command** | **Description**
--- | ---
`pacman -Syu` | Update
`pacman -Ss package` | Search package
`pacman -S package` | Install or update a package
`pacman -R package` | Delete package
`pacman -Qe` | show the install package
`pacman -Qii package` | List information on package
`pacman -Qs query` | Search installed packages for keywords

## Terminal shorcuts

Shortcut | Function
--- | ---
Ctrl + a | Ir al principio de la línea
Ctrl + e | Ir al final de la línea
Alt + b | Retroceder una palabra
Alt + f | Avanzar una palabra
Crtl + u | Borrar desde el cursor hasta el principio de la línea
Crtl + k | Borrar desde el cursor hasta el final de la línea
Crtl + w | Borrar desde el cursor hasta el principio de la palabra
Alt + d | Borrar desde el cursor hasta el final de la palabra
Ctrl + r | Search. Segunda vez para seguir buscando. `Ctrl + g`: salir de la busqueda.
Ctrl + p | Imprime el último comando. Consecutivamente hasta que encuentres el comando.
Ctrl + n | Imprime el siguiente comando. Consecutivamente hasta que encuentres el comando.

