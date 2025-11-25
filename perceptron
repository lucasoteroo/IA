def perceptron_update(x, w, b, alpha, y):
    """
    x     : vetor de atributos (ex: [x1, x2])
    w     : vetor de pesos (ex: [w1, w2])
    b     : bias
    alpha : taxa de aprendizagem
    y     : rótulo verdadeiro (0 ou 1)
    """

    # Soma líquida (u)
    u = sum(w[i] * x[i] for i in range(len(x))) + b

    # Função de ativação 
    y_hat = 1 if u >= 0 else 0

    # Erro
    erro = y - y_hat

    # Atualização dos pesos
    for i in range(len(w)):
        w[i] = w[i] + alpha * erro * x[i]

    # Atualização do bias 
    b = b + alpha * erro

    # Retorna valores atualizados + diagnósticos para estudo
    return w, b, u, y_hat, erro



# PRÁTICA COM A BASE DE DADOS DA SALA

# Dados: (Estudou, Fez o trabalho) → Passou
dados = [
    ([0, 0], 0),
    ([0, 1], 0),
    ([1, 0], 1),
    ([1, 1], 1)
]

# Pesos iniciais
w = [0.0, 0.0]  
b = 0.0
alpha = 0.1  # taxa de aprendizagem dada no enunciado

# Rodar DUAS ÉPOCAS / FASES
for epoca in range(2):
    print(f"\n===== Época {epoca+1} =====")
    
    for x, y in dados:
        w, b, u, y_hat, erro = perceptron_update(x, w, b, alpha, y)

        print(f"x={x}, y={y} | u={u:.2f} → y_hat={y_hat} | erro={erro} | novos w={w}, b={b:.2f}")

print("\nPesos finais:")
print("w =", w)
print("b =", b)
