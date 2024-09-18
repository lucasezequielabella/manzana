jugador = input("Elige piedra, papel o tijeras: ").lower()

if jugador not in opciones:
    print("Opción no válida. Por favor elige piedra, papel o tijeras.")
    return

print(f"Tú eliges: {jugador}")
print(f"La computadora elige: {computadora}")

if jugador == computadora:
    print("¡Es un empate!")
elif (jugador == 'piedra' and computadora == 'tijeras') or \
     (jugador == 'papel' and computadora == 'piedra') or \
     (jugador == 'tijeras' and computadora == 'papel'):
    print("¡Ganaste!")
else:
    print("¡Perdiste!")
if name == "main": jugar()
