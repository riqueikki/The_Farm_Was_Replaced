# Cria um LOOP infinito
while True:

    # Verifica se a planta está pronta
    if can_harvest():

        # Colhe a planta
        harvest()

    # Planta um Bush
    plant(Entities.Bush)

    # Move o Drone para o Norte
    move(North)

Entities.Bush → identifica o Bush
plant()        → realiza o plantio
move()         → movimenta o Drone
harvest()      → realiza a colheita
