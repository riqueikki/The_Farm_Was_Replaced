```markdown
# Get Pos Y() — Descobrindo a posição Y

O comando `get_pos_y()` permite descobrir a posição vertical atual do
Drone dentro da fazenda.

A posição `Y` começa em `0` no lado Sul e aumenta conforme o Drone se
movimenta para o Norte. :contentReference[oaicite:2]{index=2}

## Como funciona?

Podemos guardar a posição em uma variável:

```python
# Guarda a posição Y do Drone
y = get_pos_y()
