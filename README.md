def calcular_rank(vitorias, derrotas):
    # Calcula o saldo de vitórias
    saldo_vitorias = vitorias - derrotas
    
    # Determina o nível do jogador baseado no número de vitórias
    if vitorias < 10:
        nivel = "Ferro"
    elif 10 <= vitorias <= 20:
        nivel = "Bronze"
    elif 21 <= vitorias <= 50:
        nivel = "Prata"
    elif 51 <= vitorias <= 80:
        nivel = "Ouro"
    elif 81 <= vitorias <= 90:
        nivel = "Diamante"
    elif 91 <= vitorias <= 100:
        nivel = "Lendário"
    else:
        nivel = "Imortal"
    
    # Exibe a mensagem final com o saldo e o nível do jogador
    print(f"O Herói tem um saldo de {saldo_vitorias} está no nível de {nivel}")

# Exemplo de uso da função
calcular_rank(45, 20)
