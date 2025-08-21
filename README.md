# Lista de Compras em Python

Programa em Python que permite ao usuário **gerenciar uma lista de compras** de forma interativa.  
É possível **adicionar itens, remover itens e visualizar toda a lista**.

## 🚀 Código principal
```python
# Dia 4 - Lista de Compras

lista_compras = []

while True:
    print("\n--- Lista de Compras ---")
    print("1 - Adicionar item")
    print("2 - Remover item")
    print("3 - Ver lista")
    print("4 - Sair")

    opcao = input("Escolha uma opção: ")

    if opcao == "1":
        item = input("Digite o item que deseja adicionar: ")
        lista_compras.append(item)
        print(f"{item} foi adicionado à lista.")

    elif opcao == "2":
        item = input("Digite o item que deseja remover: ")
        if item in lista_compras:
            lista_compras.remove(item)
            print(f"{item} foi removido da lista.")
        else:
            print(f"{item} não está na lista.")

    elif opcao == "3":
        print("\nSua lista de compras:")
        for i, item in enumerate(lista_compras, start=1):
            print(f"{i}. {item}")

    elif opcao == "4":
        print("Encerrando o programa. Até logo!")
        break

    else:
        print("Opção inválida. Tente novamente.")


📌 O que foi aprendido

Criação e manipulação de listas em Python.
Métodos essenciais: append() (adicionar) e remove() (remover).
Uso de in para verificar se um item está na lista.
len() para contar itens.
enumerate() para listar com numeração (1, 2, 3…).
Construção de menu interativo com while e if/elif/else.
Boas práticas de UX no console (mensagens claras e feedback após cada ação).

💭 Comentário pessoal

Foi muito legal ver como listas facilitam organizar informações do dia a dia.
Com poucas linhas, consegui montar um mini-sistema que adiciona, remove e exibe itens.
Senti que estou mais confiante com loops e condições, e já enxergo como posso evoluir esse projeto (ex.: salvar a lista em arquivo).
