#### Anotaciones

Para compilar en Saas
```saas --watch saas:css```


- Trabaja como maquetiazción
```
footer {
    background: #444;
    h4 {
        color: red;
        a {
            color: blue;
        }
    }
}
```

- Para declarar variables en sass es: ```$NombreDeLaVariable: valorDeLaVariable``


### Organizar los archivos de Sass

Lo que tenemos que hacer es separar por archivos, con el '_' antes del nombre,
luego colocamos el nombre del archivo, luego a la hora de importar lo hacemos:
``` @import "nombreDelArchivoSinElGuión"; ```