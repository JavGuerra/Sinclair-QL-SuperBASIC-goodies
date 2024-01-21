# PROC Pat (a, b)
**Autor**: PSION

Versión del comando AT que comprueba si la versión de la ROM es FB, y en ese caso intercambia los valores de (P)osición de la línea y la columna.

## Código

```BASIC
100 DEFine PROCedure pat(a,b)
110 REMark by PSION
120   IF VER$="FB" THEN c=a:a=b:b=c
130   AT b,a
140 END DEFine 
```

## Parámetros

**a**: posición de la línea

**b**: posición de la columna

## Ejemplo de uso

```BASIC
100 PAT 10,5 : PRINT "Hello!"
```

## Más información

Aparece en el boot de la suit ofimática de PSION.

## Descargar

[pat_bas](../code/pat_bas)