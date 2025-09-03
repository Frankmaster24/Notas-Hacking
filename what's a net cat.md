## Descripcion

Del reto **what’s a net cat? (picoCTF 2019)**:

> “Usar netcat (nc) será muy importante. ¿Puedes conectarte a `jupiter.challenges.picoctf.org` en el puerto **64287** para obtener la flag?”

## Solucion

1. **Netcat (nc)** es una herramienta de red que permite conectarse a un host y puerto para enviar/recibir datos.
    
2. Para resolver el reto, basta con ejecutar en la terminal:
    
    `nc jupiter.challenges.picoctf.org 64287`
    
3. El servidor responderá con la flag en el formato:
    
    `picoCTF{XXXXXXXXXXXX}`
    

## Notas

- Este reto enseña cómo usar **netcat**, una herramienta básica en CTFs para interactuar con servicios de red.
    
- Si el puerto está cerrado o tarda, revisa conexión a internet o vuelve a intentar.
    
- **Windows:** puedes usar `nc.exe` (de Nmap o Netcat para Windows).
    
- **Linux/MacOS:** ya viene instalado en la mayoría de distribuciones.
    

## Referencias

- Netcat Cheat Sheet
    
- man nc