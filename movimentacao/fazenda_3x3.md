# Fazenda 3x3 — Movimentando o Drone pela fazenda

Agora podemos utilizar o que aprendemos sobre `move()` e as direções para percorrer uma pequena fazenda.      

Coluna
       0   1   2

Linha 0  □   □   □
Linha 1  □   □   □
Linha 2  □   □   □

# Cria um LOOP infinito
while True:

    # Verifica se a planta está pronta
    if can_harvest():

        # Colhe a planta
        harvest()

    # Quando chegar ao final da coluna
    if get_pos_y() == 2:

        # Volta para o início da próxima coluna
        move(North)
        move(East)

    else:

        # Continua subindo
        move(North)


while True     → cria o LOOP
can_harvest()  → verifica a colheita
harvest()      → realiza a colheita
get_pos_y()    → verifica a posição vertical
move(North)    → movimenta para o Norte
move(East)     → movimenta para o Leste
if / else      → toma decisões
Uma fazenda 3x3 possui:

```text
3 colunas
3 linhas
