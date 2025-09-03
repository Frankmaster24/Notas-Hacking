## Descripcion

Del reto **General Skills (picoCTF 2019)**:

> “¿Qué significa este texto `bDNhcm5fFdGgzX3IwcmD1`? Creo que tiene algo que ver con bases.”  
> La pista sugiere que se trata de **Base64**.

## Solucion

1. El texto proporcionado parece ser una cadena codificada en **Base64**.
    
2. Decodificándola:
    
    `echo "bDNhcm5fFdGgzX3IwcmD1" | base64 -d`
    
    o en Python:
    
    `import base64 print(base64.b64decode("bDNhcm5fFdGgzX3IwcmD1").decode())`
    
3. El resultado de la decodificación es:  
    **`l3arn_th3_r0p3s`**
    
4. **Bandera:** `picoCTF{learn_the_ropes}`
    

## Notas

- **Base64** es un sistema de representación que convierte datos binarios en texto ASCII legible.
    
- Se reconoce porque las cadenas suelen acabar en `=` o tener caracteres alfanuméricos con `/` o `+`.
    
- Este tipo de reto es muy común en CTFs para familiarizarse con codificaciones.
    

## Referencias

- RFC 4648 – Base64 Encoding
    
- Comando `base64` en Linux (`base64 -d` para decodificar).