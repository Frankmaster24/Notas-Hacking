## Descripcion

Del reto **First Grep (picoCTF 2019)**:

> “¿Puedes encontrar la flag en el archivo `file`? Esto sería muy tedioso de revisar manualmente, pero algo me dice que hay una mejor forma.”

## Solucion

1. El archivo contiene mucho texto, por lo que revisar línea por línea sería ineficiente.
    
2. La flag de picoCTF siempre sigue el formato `picoCTF{...}`.
    
3. Usamos el comando **grep** para buscar el patrón dentro del archivo:
    
    `grep "picoCTF" file`
    
    Esto devuelve directamente la línea que contiene la flag.
    
4. La salida será algo como:
    
    `picoCTF{XXXXXXXXXXXX}`
    
    (El contenido exacto depende del archivo que te proporcionen).
    

## Notas

- **grep** busca patrones en archivos de texto.
    
- También se puede usar:
    
    `strings file | grep picoCTF`
    
    en caso de que el archivo contenga datos binarios.
    
- El patrón `picoCTF` siempre ayuda a identificar rápidamente la bandera.
    

## Referencias

- GNU grep manual
    
- Linux `strings` command