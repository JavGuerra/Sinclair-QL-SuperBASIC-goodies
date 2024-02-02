# PROC Wait_for_yes
**Autor**: QJump

Espera a que se pulse Sí (Y) o cualquier otra tecla.

## Código

```BASIC
100 DEFine PROCedure wait_for_yes
110   PRINT #0,'If you are ready to continue, press Y'
120   REPeat iny: IF INKEY$(-1)=='Y': CLS #0: EXIT iny
130 END DEFine wait_for_yes
```

## Ejemplo de uso

```BASIC
100 wait_for_yes
```

## Descargar

[wait_for_yes_bas](../code/wait_for_yes_bas)