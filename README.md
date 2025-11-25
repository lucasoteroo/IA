# IA
Atividade da disciplina de Inteligência Artificial, período 2025.2

Professor, aconselho o senhor copiar o código e colar no Google Colab. O código está em python e já começa construindo a função pra atualização dos pesos.

Após testar o código, em duas etapas ( em mais etapas o resultado permanece o mesmo), foram encontrados os resultados abaixo.

===== Época 1 =====
x=[0, 0], y=0 | u=0.00 → y_hat=1 | erro=-1 | novos w=[0.0, 0.0], b=-0.10
x=[0, 1], y=0 | u=-0.10 → y_hat=0 | erro=0 | novos w=[0.0, 0.0], b=-0.10
x=[1, 0], y=1 | u=-0.10 → y_hat=0 | erro=1 | novos w=[0.1, 0.0], b=0.00
x=[1, 1], y=1 | u=0.10 → y_hat=1 | erro=0 | novos w=[0.1, 0.0], b=0.00

===== Época 2 =====
x=[0, 0], y=0 | u=0.00 → y_hat=1 | erro=-1 | novos w=[0.1, 0.0], b=-0.10
x=[0, 1], y=0 | u=-0.10 → y_hat=0 | erro=0 | novos w=[0.1, 0.0], b=-0.10
x=[1, 0], y=1 | u=0.00 → y_hat=1 | erro=0 | novos w=[0.1, 0.0], b=-0.10
x=[1, 1], y=1 | u=0.00 → y_hat=1 | erro=0 | novos w=[0.1, 0.0], b=-0.10

Pesos finais:
w = [0.1, 0.0]
b = -0.1
