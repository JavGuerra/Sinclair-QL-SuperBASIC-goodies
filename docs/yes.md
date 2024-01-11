# FN YES(prompt$)
**Autor**: QJump

## Código

```BASIC
100 DEFine FuNction Yes (prompt$)
110   REMark by QJump
120   PRINT #0, prompt$!'(Y or N)'
130   REPeat ina
140     answer$=INKEY$(-1)
150     IF answer$=='Y': RETURN 1
160     IF answer$=='N': RETURN 0
170   END REPeat ina
180 END DEFine Yes
```

## Parámetros

**prompt$**: Mensaje a mostrar

## Ejemplo de uso

```BASIC
100 IF Yes ('Play again?'): RUN
```

## Descargar

[yes_bas](../code/yes_bas)