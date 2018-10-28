![O Sireno from https://commons.wikimedia.org/wiki/File:O_sereo,_Francisco_Leiro.jpg](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/O_sereo%2C_Francisco_Leiro.jpg/1920px-O_sereo%2C_Francisco_Leiro.jpg)
Foto: https://commons.wikimedia.org/wiki/File:O_sereo,_Francisco_Leiro.jpg

# Sireno Grid (BETA)

*Sireno grid* es una simple y ligero Grid CSS, basado en [CSS Grid Layout](https://blogs.igalia.com/mrego/2017/05/19/spanish-css-grid-layout-el-futuro-ya-esta-aqui/)

Este grid se basa en la típica estructura de 12 columnas al más puro estilo bootstrap

El grid hace fallback a Flexbox si el navegador no soporta CSS Grid Layout manteniendo un aspecto muy similar


###### Ejemplo estructura columnas
Todas las clases usadas son proporcionadas por el framework
```
<div class="container-fluid">
  <div class="grid-row">
    <div class="col-xs-12 col-sm-10">
      Col 1 
    </div>
    <div class="col-xs-12 col-sm-10">
       Col 2
     </div>    
  </div>
</div>
```

## Algunas funcionalidades destacadas de **Sireno Grid**

#### Containers
```
.container-fluid //Container fluido
.container-fluid-1440 //Container fluido limitado a 1440
.container-fluid-1920 //Container fluido limitado a 1920
```




Usando las funcionalidades de CSS Grid Layout podemos reordenar de forma simple las columnas 
```.col-#{$breakpoint}-order-#{$i}```
Ejemplo: ```.col-sm-order-2```

#### Margenes
```
.mt-1 -> margin-top: 10px;
.mt-2 -> margin-top: 20px;
...
.mt-10 -> margin-top: 100px;
```
```
.mb-1 -> margin-bottom: 10px;
.mb-2 -> margin-bottom: 20px;
...
.mb-10 -> margin-bottom: 100px;
```

#### Fillers
Crea una columna a cada lado del grid-row hasta el borde de la ventana permitiendo añadir fondos, etc
```
.grid-filler-1240,
.grid-filler-1140,
.grid-filler-1440
```

#### Visible / Hidden
```
 .hidden-#{$breakpoint}
 .visible-#{$breakpoint}
```

Por ejemplo ```.hidden-md``` oculta un elemento para md y lg


#### Control de los *gutters*
Esta clase aplicada cualquiera de tipo col-#{breakpoint}-#{cols}, p.e. col-xs-6
```
.no-gutter-left // Sin gutter a la izquierda en cualquier tamaño
.no-gutter-right // Sin gutter a la derecha en cualquier tamaño
.no-gutters // Sin gutters  cualquier tamaño

.no-#{$breakpoint}-gutter-left
.no-#{$breakpoint}-gutter-right
.no-#{$breakpoint}-gutters
```

#### Eliminar los margenes del grid-row
```
grid-row-#{$breakpoint}-no-margins
```

