# Sistema-de-mercado-em-linguagem-c
Sistema de mercado
Este projeto implementa um sistema simples de supermercado em C, permitindo o cadastro de produtos, a visualização do estoque, a compra de produtos e a gestão de um carrinho de compras.

Funcionalidades
Cadastrar produtos no estoque.
Listar todos os produtos cadastrados.
Comprar produtos e adicionar ao carrinho.
Visualizar produtos no carrinho.
Fechar o pedido e finalizar a compra.
Saída do sistema.
Estruturas de Dados
Produto
Representa um produto disponível no estoque, com as seguintes propriedades:

codigo: Código identificador do produto (inteiro).
nome: Nome do produto (string com até 30 caracteres).
preco: Preço do produto (float).
Carrinho
Representa um item no carrinho de compras, com as seguintes propriedades:

produto: O produto escolhido (tipo Produto).
quantidade: Quantidade do produto no carrinho (inteiro).
Variáveis Globais
estoque[MAX_PRODUTOS]: Array de produtos no estoque.
carrinho[MAX_CARRINHO]: Array de itens no carrinho de compras.
total_produtos: Contador do total de produtos cadastrados.
total_itens_carrinho: Contador do total de itens no carrinho.
Funções Principais
main()
A função principal que inicia o sistema chamando o menu principal.

menuDoMercado()
Apresenta um menu com opções para o usuário interagir com o sistema. As opções incluem:

Cadastrar Produto
Listar Produtos
Comprar Produto
Visualizar Carrinho
Fechar Pedido
Sair
cadastrarProduto()
Permite ao usuário cadastrar um novo produto no estoque. Verifica se o estoque está cheio e se o código do produto já está cadastrado.

ListaDeProdutos()
Exibe a lista de produtos cadastrados no estoque. Se não houver produtos, informa ao usuário.

comprarProduto()
Permite ao usuário comprar um produto. O usuário deve fornecer o código do produto e a quantidade desejada.

produtosDoCarrinho()
Exibe os produtos que foram adicionados ao carrinho de compras.

fecharPedido()
Finaliza a compra, processando o pedido do usuário.

infoProduto(Produto prod)
Mostra as informações detalhadas de um produto.

temNoCarrinho(int codigo)
Verifica se um produto já está no carrinho com base no código.

desejaContinuar()
Pergunta ao usuário se deseja continuar utilizando o sistema após uma operação.
