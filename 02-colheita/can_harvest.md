# Can Harvest() — Verificando a colheita

O comando `can_harvest()` é utilizado para verificar se a planta que está
no local onde o Drone está pode ser colhida.

Ele funciona como uma pergunta para o programa:

> "Posso colher esta planta?"

O resultado dessa verificação pode ser `True` (verdadeiro) ou `False`
(falso).

## Como funciona?

Podemos utilizar `can_harvest()` junto com o comando `if`.

```python
if can_harvest():
    harvest()
