# Atividade ETEC - Pesquisa TudoWeb
# Aluno: Crysan
# Pesquisa com 50 entrevistados

def pesquisa_tudoweb():
    qtd_excelente = 0
    qtd_bom = 0
    qtd_ruim = 0

    print("--- PESQUISA TUDOWEB - 50 ENTREVISTADOS ---\n")

    for i in range(1, 51):
        print(f"--- Entrevistado {i}/50 ---")

        nome = input("Nome: ")
        idade = int(input("Idade: "))

        print("Opinião: 1 = EXCELENTE | 2 = BOM | 3 = RUIM")
        opiniao = int(input("Digite 1, 2 ou 3: "))

        if opiniao == 1:
            qtd_excelente += 1
        elif opiniao == 2:
            qtd_bom += 1
        elif opiniao == 3:
            qtd_ruim += 1
        else:
            print("Opção inválida. A resposta será contada como BOM.")
            qtd_bom += 1

        print()

    print("===============================")
    print("--- RESULTADO FINAL ---")
    print(f"a) Quantidade de respostas EXCELENTE: {qtd_excelente}")
    print(f"b) Quantidade de respostas RUIM: {qtd_ruim}")
    print(f"c) Quantidade de respostas BOM: {qtd_bom}")
    print("===============================")


pesquisa_tudoweb()
