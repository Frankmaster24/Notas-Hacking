## Descripcion

Del reto **General Skills (picoCTF 2019)**:

> “¿Qué es **0x3D** (base 16) en decimal (base 10)?”  
> Entrega la respuesta en formato de bandera: `picoCTF{...}`.

## Solucion

1. El valor dado es **0x3D**, que está en hexadecimal (base 16).
    
2. Expandiendo:
    
    - 3 × 16¹ = 48
        
    - D × 16⁰ = 13 (ya que D en hex = 13 en decimal)
        
3. Sumando: **48 + 13 = 61**
    
4. **Bandera:** `picoCTF{61}`
    

## Notas

- Hexadecimal usa los dígitos 0–9 y letras A–F (A=10, B=11, …, F=15).
## Referencias

- Conversión hexadecimal–decimal: Wikipedia – Hexadecimal
    
- Comando `echo $((0x...))` en Linux para conversiones rápidas.