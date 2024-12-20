# Para añadir remote webdav

```
dvc remote add -d rasp4remote webdavs://nube14.duckdns.org/remote.php/dav/files/dvcremote/datasets/orange_segmentation
dvc remote modify rasp4remote ssl_verify false
```

## Para introducir usuario y contraseña

Si se pone como se indica abajo, el usuario/contraseña NO se almacenan en el repositorio:

```
dvc remote modify --local rasp4remote user dvcremote
dvc remote modify --local rasp4remote password Cocentaina
```