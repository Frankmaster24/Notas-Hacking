## Descripcion

Del reto **Obedient Cat (picoCTF 2021)**:

> “Este archivo tiene una flag a simple vista (in-the-clear). Descarga el archivo y encuéntrala.”

## Solucion

1. El reto entrega un archivo (por ejemplo `flag`).
    
2. Como el nombre del reto es _Obedient Cat_, la pista es usar el comando **cat** para mostrar el contenido:
    
    `cat flag`
    
3. El archivo contiene directamente la bandera en texto plano, sin necesidad de decodificación ni análisis.
    
4. El resultado será algo como:
    
    `picoCTF{XXXXXXXXXXXX}`
    

## Notas

- El reto es introductorio para enseñar que muchas veces la bandera está directamente en el archivo.
    
- Otros comandos equivalentes:
    
    `less flag more flag strings flag`
    

## Referencias

- Linux cat command
    
- GNU coreutils