## Descripcion

Del reto **General Skills (picoCTF 2019)**:

> “¿Puedes convertir el número **42** (base 10) a **binario** (base 2)?”  
> Entrega la respuesta en formato de bandera: `picoCTF{...}`.

## Solucion

1. Número dado: **42** en decimal (base 10).
    
2. Para convertir a binario, se divide sucesivamente entre 2:
    
    - 42 ÷ 2 = 21 → residuo **0**
        
    - 21 ÷ 2 = 10 → residuo **1**
        
    - 10 ÷ 2 = 5 → residuo **0**
        
    - 5 ÷ 2 = 2 → residuo **1**
        
    - 2 ÷ 2 = 1 → residuo **0**
        
    - 1 ÷ 2 = 0 → residuo **1**
        
3. Leyendo de abajo hacia arriba: **101010**.
    
4. **Bandera:** `picoCTF{101010}`
    
- Atajos para convertir:
    
    - **Python:** `bin(42)` → `0b101010`
        
    - **Bash:** `echo "obase=2; 42" | bc` → `101010`
        

## Referencias

- Conversión de bases: Wikipedia – Binary number
    
- Comando `bc` en Linux para operaciones en distintas bases.