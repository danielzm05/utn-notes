DEBUG es una herramienta que permite **ejecutar, depurar y cargar programas en assembler** directamente en memoria.  

> Sus comandos comienzan con un guion (`-`).

## Comandos

| Comando | Función                                                                              |
| ------- | ------------------------------------------------------------------------------------ |
| `-A`    | Activa el modo de programar en Assembler                                             |
| `-D`    | Ver memoria (hex/ASCII)                                                              |
| `-E`    | Escribir bytes en memoria                                                            |
| `-G`    | Ejecutar programa                                                                    |
| `-T`    | Ejecuta instrucción por instrucción.                                                 |
| `-U`    | Desensamblar (unassemble)                                                            |
| `-R`    | Muestra el estado de todos los registros y permite cambiar el valor de los mismos.os |
| `-M`    | Mover bloques de memoria                                                             |
| `-N`    | Nombrar archivo                                                                      |
| `-L`    | Cargar archivo                                                                       |
| `-W`    | Guardar archivo                                                                      |


| Código | Significado |
|--------|-------------|
| **OV** | Overflow (OF=1) |
| **NV** | No Overflow (OF=0) |
| **NG** | Negativo (SF=1) |
| **PL** | Positivo (SF=0) |
| **ZR** | Zero (ZF=1) |
| **NZ** | Not Zero (ZF=0) |
| **CY** | Carry (CF=1) |
| **NC** | No Carry (CF=0) |
| **PE** | Paridad par (PF=1) |
| **PO** | Paridad impar (PF=0) |
