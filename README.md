import random
import string

print("=== VEINCODE // GENERADOR DE CLAVES ===")

longitud = int(input("Longitud de la contraseña: "))

caracteres = string.ascii_letters + string.digits + "!@#$%&*"
password = ""

for _ in range(longitud):
    password += random.choice(caracteres)

print(f"\n[+] Contraseña generada: {password}")
