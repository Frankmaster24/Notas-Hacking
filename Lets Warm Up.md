## Descripcion

Del reto **Let’s Warm Up (picoCTF 2019)**:

> “Si te digo que una palabra empieza con **0x70** en hexadecimal, ¿con qué empezaría en **ASCII**?”  
> Entrega la respuesta en formato de bandera: `picoCTF{...}`.

## Solucion

1. **0x70** es un número **hexadecimal**.
    
2. Convirtiendo 0x70 a decimal → **112**.
    
3. En la tabla **ASCII**, el código **112** corresponde a la letra **‘p’** (minúscula).
    
4. **Solución:** `picoCTF{p}`
    

## Notas

- El prefijo **0x** indica base 16 (hex).
    
- Atajos para verificar:
    
    - **Python:** `python -c "print(chr(0x70))"` → `p`
        
    - **Bash:** `printf "\x70\n"` → `p`
        
    - **PowerShell:** `[char]0x70` → `p`
        
- Recordatorio: `0x61` = `a`, `0x70` = `p`, etc.
    

## Referencias

- Tabla ASCII estándar (puedes verla con `man ascii` en Linux o buscando “ASCII table”).