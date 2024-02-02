# FN YES(prompt$)
**Autor**: QJump

## Código

```BASIC
100 DEFine FuNction Yes (prompt$)
110   PRINT #0, prompt$!'(Y or N)'
120   REPeat ina
130     answer$=INKEY$(-1)
140     IF answer$=='Y': RETURN 1
150     IF answer$=='N': RETURN 0
160   END REPeat ina
170 END DEFine Yes
```

## Parámetros

**prompt$**: Mensaje a mostrar

## Ejemplo de uso

```BASIC
100 IF Yes ('Play again?'): RUN
```

## Descargar

[yes_bas](../code/yes_bas)