while True:
    cpf = input("Digite seu CPF: ").strip()

    # Remova todos os caracteres de separação (pontos, traços, etc.)
    cpf = cpf.replace(".", "").replace("-", "")

    # Verifique se o CPF tem 11 dígitos
    if len(cpf) != 11 or not cpf.isdigit():
        print("CPF inválido: Deve conter exatamente 11 dígitos numéricos.")
    else:
        cpf_lista = list(cpf)
        print(cpf)
        lista_multiplicada = []
        lista_multiplicada2 = []
        valor_multiplicado = 0
        valor_multiplicado2 = 0

        numeros = 10
        numeros2 = 11
        i = 0
        j = 0

        while numeros >= 2:
            digito = int(cpf_lista[i]) * numeros
            numeros -= 1
            i += 1
            lista_multiplicada.append(digito)
        print("--"*20)
        print(lista_multiplicada)
        valor_multiplicado = sum(lista_multiplicada)
        print(valor_multiplicado)

        valor_multiplicado = valor_multiplicado * 10
        resto_da_multi = valor_multiplicado % 11
        if resto_da_multi > 9 :
            resto_da_multi = 0
    
        print(resto_da_multi)
        print('--'*20)

        while numeros2 >= 2:
            digito2 = int(cpf_lista[j]) * numeros2
            numeros2 -= 1
            j += 1
            lista_multiplicada2.append(digito2)

        print(lista_multiplicada2)
        valor_multiplicado2 = sum(lista_multiplicada2)
        print(valor_multiplicado2)

        valor_multiplicado2 = valor_multiplicado2 * 10
        resto_da_multi2 = valor_multiplicado2 % 11
        print(resto_da_multi2)
        if resto_da_multi2 > 9:
            resto_da_multi2 = 0

        if resto_da_multi == int(cpf[-2]) and resto_da_multi2 == int(cpf[-1]):
            print("este CPF é válido")
        else:
            print("este CPF está inválido")
            continue
