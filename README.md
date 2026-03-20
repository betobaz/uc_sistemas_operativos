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

# Dispositivos de bloque (discos y particiones)
lsblk

# Lista de todos los drivers cargados en el kernel
cat /proc/devices

```

### WSL - Interrupciones y DMA en vivo

```
watch -n 1 cat /proc/interrupts

# Ver canales DMA del sistema
cat /proc/dma

# Ver estadisticas de E/S del disco en tiempo real
iostat -x 1 3
# (instalar con: apt-get install sysstat)
```