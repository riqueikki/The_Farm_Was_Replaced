plant(Entities.Carrot)

# Prepara o terreno
till()

# Planta a cenoura
plant(Entities.Carrot)

# Verifica se o terreno é Grassland
if get_ground_type() == Grounds.Grassland:

    # Transforma o terreno em Soil
    till()

# Planta a cenoura
plant(Entities.Carrot)

# Cria um LOOP infinito
while True:

    # Verifica se a planta está pronta
    if can_harvest():

        # Colhe a planta
        harvest()

    # Verifica o tipo de terreno
    if get_ground_type() == Grounds.Grassland:

        # Prepara o terreno
        till()

    # Planta a cenoura
    plant(Entities.Carrot)
