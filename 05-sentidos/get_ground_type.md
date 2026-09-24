### `05-sentidos/get_ground_type.md`

```markdown
# Get Ground Type() — Descobrindo o tipo de terreno

O comando `get_ground_type()` permite descobrir qual é o tipo de terreno
que está abaixo do Drone.

O jogo possui diferentes tipos de terreno, como `Grassland` e `Soil`.
:contentReference[oaicite:3]{index=3}

## Como funciona?

Podemos verificar o terreno onde o Drone está:

```python
# Descobre o tipo de terreno
if get_ground_type() == Grounds.Grassland:

    # Prepara o terreno
    till()
