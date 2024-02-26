# Expresiones regulares administracion Kubernetes
Aqui algunas expresiones que ayudaron a la administracion de kubernetes
#### Obtener los reinicio de los pods
```bash
[0-9]{1,7}\s\([0-9]{1,5}[dms]([0-9]{1,3}[hs])?\sago\)
```

#### Obtener status de un curl a un servicio 
```bash
"status":[2-5]+[0-9]{2,2}
```
#### Obtener lineas en listas de archivos cuyas extensiones esten en el parentesis
```bash
^.*(.jar|\.class|\.original|\.lst)$
```
#### Obtener la ips 
```bash
[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}
```
#### Obtener variables de entorno
```bash
([A-Z]{1,5}_){1,3}[A-Z]{1,5}
```
#### Obtener los servicios recientemente desplegados en minutos
```bash
\s[0-9]{1,3}m[0-9]{0,2}s?$
```
#### Obtener los textos con formato de versionamiento ej. v1.2.3
```bash
v[1-9][0-9]{0,1}\.[0-9]{1,3}\.[0-9]{1,3}
# sin la v inicial
[1-9]{1,2}\.[0-9]{1,2}\.[0-9]{1,2}
```
#### Obtener los textos con formato acd_dfd_dsdd
```bash
([a-z]+_)+[a-z]+
```
#### Obtener los textos con formato de directorio linux /var/lib/gen con un espacio por delante
```bash
\s(\/[a-zA-Z0-9_-]+)+
```

#### Obtener los textos con formato Fecha 2023
```bash
([A-Z][a-z]{2}\s){2}[1-3][0-9]?\s[0-2][0-9](:[0-5][0-9]){2}\s2023
```
#### Obtener los textos con formato acd_dfd_dsdd
```bash
([a-z0-9]+-)+[a-z0-9]+
```
