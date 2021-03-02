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


### Mixin

Los mixin son una mezcla de estilos de CSS que podemos incluir en otro lado.
Vienen siendo algo así como tipo funciones. Son como una variable pero llevadas
a un bloque de código.

```
@mixin cuadrado ($fondo, $ancho:200px) {
    background-color: $fondo;
    width: $ancho;
    height: 200px;
    margin-top: 5px;
    padding: 10px;
}

.cuadrado-1{
    @include cuadrado(#111, 300px);
}

.cuadrado-2{
    @include cuadrado(#222);
}
```