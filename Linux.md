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