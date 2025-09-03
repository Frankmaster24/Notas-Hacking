## Descripcion

Del reto **plumbing (picoCTF 2019)**:

> “A veces necesitas manejar datos de procesos fuera de un archivo. ¿Puedes encontrar una forma de conservar la salida de este programa y buscar la flag? Conéctate a `jupiter.challenges.picoctf.org` puerto **4427**.”

## Solucion

1. El reto genera una salida muy grande al conectarse con **netcat**:
    
    `nc jupiter.challenges.picoctf.org 4427`
    
2. Como es demasiado texto, lo ideal es **redirigir la salida a un archivo** para analizarla:
    
    `nc jupiter.challenges.picoctf.org 4427 > salida.txt`
    
3. Luego, busca dentro del archivo la flag con **grep**:
    
    `grep "picoCTF" salida.txt`
    
4. Esto devolverá directamente la bandera en formato:
    
    `picoCTF{XXXXXXXXXXXX}`
    

## Notas

- **Redirección (>)** guarda la salida estándar en un archivo en lugar de mostrarla en pantalla.
    
- También podrías encadenar directamente:
    
    `nc jupiter.challenges.picoctf.org 4427 | grep picoCTF`
    
    Esto imprime solo la línea con la bandera sin necesidad de guardar archivo.
    
- Es un reto para practicar _pipes_ (`|`) y _redirección_ (`>`).
    

## Referencias

- Linux I/O Redirection
    
- Netcat (nc)