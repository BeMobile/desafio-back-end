# Teste Técnico Back-end Be

Este é um repositório para Testes Técnicos em Back-end da Be. Ele é destinado a pessoas que participam de nossos processos seletivos. 

Se você chegou até aqui por meio de um formulário de Teste Técnico, siga em frente. Caso contrário, acompanhe a Be no [Linkedin](https://br.linkedin.com/company/bemobiletech), [Instagram](https://www.instagram.com/bemobile.tech/), [Facebook](https://www.facebook.com/bemobile.tech) ou na nossa comunidade no [Telegram](https://t.me/be_tech_community). Divulgamos novos processos seletivos por lá.

## Desafio

O Teste Técnico para Back-End da Be consiste em estruturar uma API RESTful conectada a um banco de dados.

Trata-se de um sistema que permite cadastrar usuários externos. Ao realizarem login, estes usuários deverão poder registrar clientes, produtos e vendas.

O(a) candidato(a) deve desenvolver o projeto em um dos seguintes frameworks: Adonis (Node.js) ou Laravel (PHP).

### Banco de Dados

O banco de dados deve ser estruturado à escolha do(a) candidato(a), mas minimamente deve conter:

* usuários: email, senha;
* clientes: nome, cpf;
* endereço: todos os campos de endereço;
* telefones: cliente, número;
* produtos: colocar os dados necessários para um tipo de produto, além de preço.
* vendas: cliente, produto, quantidade, preço unitário, preço total, data e hora.

### Rotas do Sistema
O sistema deve contar com rotas para:

* cadastro de usuário do sistema (signup);
* login com JWT de usuário cadastrado (login);
* clientes:
  * listar todos os clientes cadastrados (index)
    * apenas dados principais devem vir aqui;
    * ordenar pelo id;
  * detalhar um(a) cliente e vendas a ele(a) (show):
    * trazer as vendas mais recentes primeiro;
    * possibilidade de filtrar as vendas por mês + ano;
  * adicionar um(a) cliente (store);
  * editar um(a) cliente (update);
  * excluir um(a) cliente e vendas a ele(a) (delete);
* produtos:
  * listar todos os produtos cadastrados (index):
    * apenas dados principais devem vir aqui;
    * ordenar alfabeticamente.
  * detalhar um produto (show);
  * criar um produto (store);
  * editar um produto (update);
  * exclusão lógica ("soft delete") de um produto (delete);
* vendas:
  * registrar venda de 1 produto a 1 cliente (store).

Observação: as rotas em clientes, produtos e vendas só devem poder ser acessadas por usuário logado.

### Requisitos
São requisitos básicos:

* estruturar o sistema observando o MVC (porém, sem as views);
* usar MySQL como banco de dados;
* respostas devem ser em JSON;
* pode-se usar recursos e bibliotecas que auxiliam na administração do banco de dados (Eloquent, Lucid, Knex, Bookshelf etc.);
* documentar as instruções necessárias em um README (requisitos, como instalar e rodar o projeto, detalhamento de rotas e outras informações que julgar relevantes).

Caso o(a) candidato(a) não consiga completar o teste até o prazo definido, deve garantir que tudo que foi construído esteja em funcionamento. Neste caso, relatar no README quais foram as dificuldades encontradas.

### Critérios de Avaliação
Serão critérios para avaliação da solução fornecida:

* lógica de programação;
* organização do projeto;
* legibilidade do código;
* validação necessária dos dados;
* forma adequada de utilização dos recursos;
* seguimento dos padrões especificados;
* clareza na documentação.

### Envio da Solução
O projeto deverá ser hospedado em um repositório no seu GitHub. O link do repositório deverá ser fornecido por meio do formulário de Teste Técnico encaminhado ao seu e-mail. Não serão aceitos links de projetos enviados por outros meios.

Demais instruções e regras serão instruídas nos formulários e nas comunicações do processo seletivo do qual você está participando.
