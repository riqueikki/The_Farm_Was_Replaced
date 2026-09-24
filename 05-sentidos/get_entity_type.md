
### `05-sentidos/get_entity_type.md`

```markdown
# Get Entity Type() — Descobrindo o que está na posição

O comando `get_entity_type()` permite descobrir qual entidade está
ocupando a posição onde o Drone está.

Se não existir nenhuma entidade naquele local, o comando retorna `None`.
Caso exista uma entidade, ele retorna o tipo correspondente. :contentReference[oaicite:6]{index=6}

## Como funciona?

Podemos verificar qual entidade está na posição:

```python
# Verifica a entidade que está abaixo do Drone
if get_entity_type() == Entities.Grass:

    # Colhe a grama
    harvest()

# Cria um LOOP infinito
while True:

    # Verifica se existe uma planta pronta
    if can_harvest():

        # Realiza a colheita
        harvest()

    # Verifica se o espaço está vazio
    if get_entity_type() == None:

        # Planta um Bush
        plant(Entities.Bush)
