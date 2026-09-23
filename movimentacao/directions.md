```markdown
# Directions — Direções do Drone

O Drone pode se movimentar em quatro direções:

        ↑
        |
←──── Drone ────→
        |
        ↓

```text
        North
          ↑
          |
West ← Drone → East
          |
          ↓
        South


# Cria um LOOP infinito
while True:

    # Move para o Norte
    move(North)

    # Move para o Leste
    move(East)
