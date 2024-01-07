# X_Scale
Autor: Dilwin Jones

Esta función toma en cuenta la relación de aspecto de 2:1 de las pantallas en los modos 4 y 8 del QL original para su aprovechamiento en la representación de gráficos que usan el sistema de coordenadas como PLOT, LINE, CIRCLE, etc.

## Código

```BASIC
100 DEFine FuNction X_Scale(y_scale,wide,high)
110   REMark by Dilwyn Jones
120   RETurn 0.75 * y_scale * wide / high
130 END DEFine X_Scale
```

## Ejemplo de uso

El siguiente código permite mostrar un círculo perfecto que ocupe toda la pantalla calculando la posición de la coordenada X.

```BASIC
100 WINDOW 512,256,0,0 : CLS
110 x = X_Scale(100,512,256)
120 CIRCLE x/2,50,25
130 :
1000 DEFine FuNction X_Scale (y_scale,wide,high)
1010   RETurn .75 * y_scale*wide/high
1020 END DEFine X_Scale
```

**Nota**: Puede sustituirse .75 por .7411765 que es un valor más exacto de la verdadera relación de aspecto de la pantalla del QL.

## Más información
Esta función está basada en un artículo de Dilwin Jones titulado SCALE GRAPHICS que fue publicado en QL Today y puede encontrarse aquí:

- [Scale graphics](https://www.dilwyn.qlforum.co.uk/docs/articles/scales.zip)

Más información y uso sobre esta función en español en los artículos:

- [Sistema de coordenadas en el QL, la sentencia SCALE](https://sinclairqles.wordpress.com/2014/03/25/sistema-de-coordenadas-en-el-ql/), traducido por Afx del original.
- [Acid Face](https://foro.speccy.org/viewtopic.php?p=15624&hilit=acid+face#p15624), una aplicación básica que usa esta función para generar caras felices, por badaman.

## Descargar

[x_scale_bas](../code/x_scale_bas)