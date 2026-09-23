
---

## `01 - loop/harvest.md`

```markdown
# Harvest() — Realizando a colheita

O comando `harvest()` é utilizado para realizar a colheita da planta
que está no local onde o Drone está.

Enquanto `can_harvest()` verifica se podemos colher, `harvest()` é o
comando que realmente realiza a colheita.

Podemos pensar assim:

```text
can_harvest()
      ↓
"Posso colher?"
      ↓
     SIM
      ↓
harvest()
      ↓
"Realiza a colheita"
