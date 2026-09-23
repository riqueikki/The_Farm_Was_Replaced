## Verifica se a planta está pronta
    if can_harvest():

# Colhe a planta
    harvest()

Esse código permite que o Drone verifique se existe algo pronto para ser colhido.

### Cria um LOOP infinito
while True:

### Verifica se a planta está pronta
    if can_harvest():

#Colhe a planta
        harvest()

# Move o Drone para o Norte
    move(North)
