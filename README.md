# Sistemas Operativos

## Sesión 8

### Como arrancar el contenedor de Ubuntu
```
docker run --rm -it ubuntu bash
```

### Actividad WSL - Ver los dispositivos de sistema

```
# Ver todos los dispositivos disponibles
ls -la /dev | head -30
ls -la /dev | tail -30
```