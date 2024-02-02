# PROC Wmon
**Autor**: QJump

Restaura las ventanas y el modo 4 para monitor.

## Código

```BASIC
100 DEFine PROCedure wmon
110   WINDOW #0;488,42,12,214:BORDER #0;1,4,0
120   WINDOW #1;244,172,256,38:BORDER #1;1,255
130   WINDOW #2;244,172,12,38:BORDER #2;1,255
140   MODE 4
150 END DEFine wmon
```

## Ejemplo de uso

```BASIC
100 wmon
```

## Descargar

[wmon_bas](../code/wmon_bas)