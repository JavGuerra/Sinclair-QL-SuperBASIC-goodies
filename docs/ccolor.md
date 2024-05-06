# FN ccolor
**Autor**: Andrew

Devuelve el valor de un color en un número entero a partir de los colores y la trama dada.

## Código

```BASIC
100 DEFine FuNction ccolor(col%,con%,stp%)
110   RETurn 64*stp%+8*(col%^^con%)+col%
120 END DEFine ccolor
```

## Parámetros

**col%**: color primario. Valor entero de 0 a 7.

**con%**: contraste o color secundario. Valor entero de 0 a 7.

**stp%**: tipo de trama. Valor entero de 0 a 3.

## Devuelve

El número de color equivalente a la trama dada. Valor entero.

## Ejemplo de uso

```BASIC
100 PAPER CCOLOR(2, 7, 3): CLS
```

## Más información

En PE, el color siempre se establece como un valor único, no 3 (color, contraste y trama).

Ver uso de los comandos que usan tramas, como PAPER, INK, BORDER...

+info: [Cómo definir colores punteados](https://retrowiki.es/viewtopic.php?f=98&t=200040439) 

## Descargar

[ccolor_bas](../code/ccolor_bas)