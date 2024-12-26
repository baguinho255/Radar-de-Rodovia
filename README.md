# aqui você vera seu codigo de readar de carro de redovia para pode fazar um estudo sobre.
# uso para aula projeto emcompleto para conhecimento de portifolios.
# pode ter conhecimento de futuro projeto para quem for usar com resposbilidade .
def verificar_velocidade(velocidade, limite):
    """
    Função que verifica se a velocidade do veículo está acima do limite e calcula a multa.
    """
    if velocidade <= limite:
        print(f"Velocidade: {velocidade} km/h. Dentro do limite de {limite} km/h.")
    else:
        excesso = velocidade - limite
        multa = excesso * 5  # Valor da multa por km/h acima do limite
        print(f"Velocidade: {velocidade} km/h. Acima do limite de {limite} km/h!")
        print(f"Excesso de velocidade: {excesso} km/h.")
        print(f"Multa aplicada: R$ {multa:.2f}.")


# Exemplo de uso
limite_velocidade = 80  # Limite de velocidade em km/h
velocidade_do_veiculo = float(input("Informe a velocidade do veículo (em km/h): "))

verificar_velocidade(velocidade_do_veiculo, limite_velocidade)
