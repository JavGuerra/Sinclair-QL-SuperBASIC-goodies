# FN bsf
**Autor**: Badaman

Función que calcula el factor de velocidad relativo a un QL básico, teniendo de esta forma una referencia de la velocidad de cómputo de la máquina sobre la que se ejecuta la función BSF.

## Código

```BASIC
100 DEFine FuNction BSF
110   REMark Basic Speed Factor
120   LOCal r, d, c, n, i
130   LET r = 84 : REMark Basic QL Factor
140   LET d = DATE : c = 0 : n = 0
150   REPeat i
160     IF DATE <> d THEN 
170       d = DATE
180       n = n + 1
190       IF n = 1 THEN 
200         c = 0
210       ELSE 
220         EXIT i
230       END IF 
240     ELSE 
250       c = c + 1
260     END IF 
270   END REPeat i
280   REMark PRINT c : REMark count
290   RETurn c / r
300 END DEFine BSF
```

## Devuelve

Un número que indica el factor de QL básico, es decir, cuántas veces es más rápido el ordenador sobre el que se ejecuta la función respecto a un QL básico. El valor 1 corresponde a una velocidad igual a la de un QL básico.

## Ejemplo de uso

```BASIC
100 CLEAR : PRINT BSF
```

## Más información

En un QL básico, el número de sumas por segundo es 84. Este valor es el Factor de QL básico (BSF en inglés), y se guarda en la variable `r` en esta función.

Quite el comentario de la línea 280 para conocer el número de operaciones por segundo.

+info: [Factor de velocidad para juegos en el QL](https://retrowiki.es/viewtopic.php?f=98&t=200040399)

## Descargar

[bsf_bas](../code/bsf_bas)