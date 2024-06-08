## 1. Diagrama de Caso de Uso – Autenticação e Gerenciamento de Usuários
Casos de Uso: Cadastrar Administrador, Excluir Funcionário, Criar Funcionário, Fazer Login, Fazer Logout, Criar Token de Autenticação, Excluir Token de Autenticação, Verificar Email, Gerenciamento de Usuários, Gerenciamento de Sessão.

![alt](https://github.com/fabio-SZK/grupo-8-kistock/blob/main/Diagramas/Diagrama%20de%20Caso%20de%20Uso/Autenticacao.png)

### Especificação do Caso de Uso: Cadastrar Administrador

ID:
001

Nome do caso de uso:
Cadastrar Administrador

Atores:
Dono (Admin)

Visão Geral:
Este caso de uso descreve como o Dono cadastra um novo administrador no sistema.

Cenário de Sucesso Principal:

    O Dono acessa o sistema e escolhe a opção "Cadastrar Administrador".
    O Dono preenche os dados do novo administrador (nome, email, senha).
    O sistema verifica se o email informado já está cadastrado.
    O sistema envia um email de verificação para o novo administrador.
    O novo administrador verifica o email e clica no link de confirmação.
    O sistema confirma o cadastro do novo administrador e atualiza a lista de usuários.
    O caso de uso termina com o Dono visualizando a confirmação do cadastro.

Extensões:
E.1. No Passo 3, o email informado já está cadastrado.
E.1.1. O sistema exibe uma mensagem de erro informando que o email já está em uso.
E.1.2. O Dono insere um novo email e retorna ao Passo 2.

### Especificação do Caso de Uso: Excluir Funcionário

ID:
002

Nome do caso de uso:
Excluir Funcionário

Atores:
Dono (Admin)

Visão Geral:
Este caso de uso descreve como o Dono exclui um funcionário do sistema.

Cenário de Sucesso Principal:

    O Dono acessa o sistema e escolhe a opção "Gerenciamento de Usuários".
    O Dono seleciona o funcionário a ser excluído.
    O sistema exibe os detalhes do funcionário selecionado.
    O Dono confirma a exclusão do funcionário.
    O sistema remove o funcionário da lista de usuários e atualiza a base de dados.
    O caso de uso termina com o Dono visualizando a confirmação da exclusão.

Extensões:
E.1. No Passo 4, o Dono decide cancelar a exclusão.
E.1.1. O Dono cancela a operação.
E.1.2. O sistema retorna à tela de Gerenciamento de Usuários.

### Especificação do Caso de Uso: Criar Funcionário

ID:
003

Nome do caso de uso:
Criar Funcionário

Atores:
Dono (Admin)

Visão Geral:
Este caso de uso descreve como o Dono cria um novo funcionário no sistema.

Cenário de Sucesso Principal:

    O Dono acessa o sistema e escolhe a opção "Criar Funcionário".
    O Dono preenche os dados do novo funcionário (nome, email, cargo, senha).
    O sistema verifica se o email informado já está cadastrado.
    O sistema salva os dados do novo funcionário.
    O sistema envia um email de boas-vindas para o novo funcionário.
    O caso de uso termina com o Dono visualizando a confirmação do cadastro.

Extensões:
E.1. No Passo 3, o email informado já está cadastrado.
E.1.1. O sistema exibe uma mensagem de erro informando que o email já está em uso.
E.1.2. O Dono insere um novo email e retorna ao Passo 2.

### Especificação do Caso de Uso: Fazer Login

ID:
004

Nome do caso de uso:
Fazer Login

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como um usuário (funcionário ou Dono) faz login no sistema.

Cenário de Sucesso Principal:

    O usuário acessa a página de login.
    O usuário insere o email e a senha.
    O sistema verifica as credenciais.
    O sistema gera um token de autenticação (JWT).
    O sistema redireciona o usuário para a página inicial.
    O caso de uso termina com o usuário autenticado e acessando o sistema.

Extensões:
E.1. No Passo 3, as credenciais estão incorretas.
E.1.1. O sistema exibe uma mensagem de erro informando que as credenciais estão incorretas.
E.1.2. O usuário insere novamente as credenciais e retorna ao Passo 2.

### Especificação do Caso de Uso: Fazer Logout

ID:
005

Nome do caso de uso:
Fazer Logout

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como um usuário (funcionário ou Dono) faz logout do sistema.

Cenário de Sucesso Principal:

    O usuário acessa a opção "Logout".
    O sistema invalida o token de autenticação (JWT).
    O sistema redireciona o usuário para a página de login.
    O caso de uso termina com o usuário deslogado do sistema.

Extensões:
Nenhuma.

### Especificação do Caso de Uso: Verificar Email

ID:
006

Nome do caso de uso:
Verificar Email

Atores:
Dono (Admin), Novo Administrador

Visão Geral:
Este caso de uso descreve como o sistema verifica o email de um novo administrador.

Cenário de Sucesso Principal:

    O novo administrador recebe um email de verificação.
    O novo administrador clica no link de verificação no email.
    O sistema verifica o link de confirmação.
    O sistema confirma o email do novo administrador.
    O caso de uso termina com o novo administrador podendo acessar o sistema.

Extensões:
E.1. No Passo 3, o link de confirmação é inválido ou expirado.
E.1.1. O sistema exibe uma mensagem de erro informando que o link é inválido ou expirado.
E.1.2. O novo administrador solicita um novo email de verificação.

## 2. Diagrama de Caso de Uso – Gerenciamento de Estoque

Casos de Uso: Consultar Produtos, Criar Produtos, Excluir Produtos, Atualizar Produtos, Registrar Venda, Registrar Compra, Atualizar Estoque, Gerenciar Produtos, Gerenciar Transações, Criar Histórico de Transação

![alt](https://github.com/fabio-SZK/grupo-8-kistock/blob/main/Diagramas/Diagrama%20de%20Caso%20de%20Uso/Estoque.png)

### Especificação do Caso de Uso: Consultar Produtos

ID:
007

Nome do caso de uso:
Consultar Produtos

Atores:
Funcionário, Dono (Admin), Cliente

Visão Geral:
Este caso de uso descreve como um ator consulta o status de um produto no sistema.

Cenário de Sucesso Principal:

    O ator (Funcionário, Dono ou Cliente) acessa o sistema e escolhe a opção "Consultar Produtos".
    O ator insere o código ou nome do produto na barra de busca.
    O sistema busca as informações do produto no banco de dados.
    O sistema exibe as informações do produto (código, nome, quantidade em estoque, preço).
    O caso de uso termina com o ator visualizando as informações do produto.

Extensões:
E.1. No Passo 3, o sistema não encontra o produto no banco de dados.
E.1.1. O sistema exibe uma mensagem de erro informando que o produto não foi encontrado.
E.1.2. O ator retorna ao Passo 2 para inserir um novo código ou nome do produto.

### Especificação do Caso de Uso: Criar Produtos

ID:
008

Nome do caso de uso:
Criar Produtos

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como um produto é criado no sistema.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Criar Produtos".
    O ator preenche os dados do produto (nome, descrição, preço, quantidade inicial).
    O sistema verifica se o produto já existe.
    O sistema salva o novo produto no banco de dados.
    O sistema confirma a criação do produto.
    O caso de uso termina com o ator visualizando a confirmação da criação.

Extensões:
E.1. No Passo 3, o produto já existe.
E.1.1. O sistema exibe uma mensagem de erro informando que o produto já está cadastrado.
E.1.2. O ator insere novos dados e retorna ao Passo 2.

### Especificação do Caso de Uso: Excluir Produtos

ID:
009

Nome do caso de uso:
Excluir Produtos

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como um produto é excluído do sistema.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Gerenciar Produtos".
    O ator seleciona o produto a ser excluído.
    O sistema exibe os detalhes do produto selecionado.
    O ator confirma a exclusão do produto.
    O sistema remove o produto do banco de dados.
    O caso de uso termina com o ator visualizando a confirmação da exclusão.

Extensões:
E.1. No Passo 4, o ator decide cancelar a exclusão.
E.1.1. O ator cancela a operação.
E.1.2. O sistema retorna à tela de Gerenciar Produtos.

### Especificação do Caso de Uso: Atualizar Produtos

ID:
010

Nome do caso de uso:
Atualizar Produtos

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como um produto é atualizado no sistema.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Gerenciar Produtos".
    O ator seleciona o produto a ser atualizado.
    O sistema exibe os detalhes do produto selecionado.
    O ator atualiza os dados do produto (nome, descrição, preço, quantidade).
    O sistema salva as atualizações no banco de dados.
    O caso de uso termina com o ator visualizando a confirmação da atualização.

Extensões:
E.1. No Passo 5, ocorre um erro ao salvar as atualizações.
E.1.1. O sistema exibe uma mensagem de erro informando o problema.
E.1.2. O ator corrige os dados e retorna ao Passo 4.

### Especificação do Caso de Uso: Registrar Venda

ID:
011

Nome do caso de uso:
Registrar Venda

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como uma venda é registrada no sistema.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Registrar Venda".
    O ator preenche os dados da venda (cliente, produtos, quantidade, valor total).
    O sistema verifica a disponibilidade dos produtos em estoque.
    O sistema atualiza o estoque dos produtos vendidos.
    O sistema salva os dados da venda no banco de dados.
    O caso de uso termina com o ator visualizando a confirmação da venda.

Extensões:
E.1. No Passo 3, não há produtos suficientes em estoque.
E.1.1. O sistema exibe uma mensagem de erro informando a falta de estoque.
E.1.2. O ator ajusta a quantidade dos produtos e retorna ao Passo 2.

### Especificação do Caso de Uso: Registrar Compra

ID:
012

Nome do caso de uso:
Registrar Compra

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como uma compra é registrada no sistema.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Registrar Compra".
    O ator preenche os dados da compra (fornecedor, produtos, quantidade, valor total).
    O sistema atualiza o estoque dos produtos comprados.
    O sistema salva os dados da compra no banco de dados.
    O caso de uso termina com o ator visualizando a confirmação da compra.

Extensões:
Nenhuma.

## 3. Diagrama de Caso de Uso – Nota Fiscal Eletrônica

Casos de Uso: Emitir Nota Fiscal Eletrônica, Verificar Integridade da Nota Fiscal, Salvar XML da Nota Fiscal de Saída na Nuvem, Salvar XML da Nota Fiscal de Entrada na Nuvem

![alt](https://github.com/fabio-SZK/grupo-8-kistock/blob/main/Diagramas/Diagrama%20de%20Caso%20de%20Uso/Nota%20Fiscal.png)

### Especificação do Caso de Uso: Emitir Nota Fiscal Eletrônica (NFe)

ID:
013

Nome do caso de uso:
Emitir Nota Fiscal Eletrônica (NFe)

Atores:
Funcionário, Dono (Admin), Cliente

Visão Geral:
Este caso de uso descreve como o sistema emite uma Nota Fiscal Eletrônica.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Emitir Nota Fiscal Eletrônica".
    O ator insere os dados da transação (cliente, produtos, valores).
    O sistema verifica a integridade da nota fiscal junto ao SEFAZ.
    O sistema gera a Nota Fiscal Eletrônica e exibe a nota para o ator.
    O sistema salva o XML da Nota Fiscal de Saída na nuvem.
    O sistema envia a nota fiscal eletrônica para o cliente.
    O caso de uso termina com o cliente recebendo a nota fiscal.

Extensões:
E.1. No Passo 3, o sistema não consegue verificar a integridade da nota fiscal.
E.1.1. O sistema exibe uma mensagem de erro informando o problema.
E.1.2. O ator corrige os dados e retorna ao Passo 2.

### Especificação do Caso de Uso: Verificar Integridade da Nota Fiscal

ID:
014

Nome do caso de uso:
Verificar Integridade da Nota Fiscal

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como o sistema verifica a integridade de uma nota fiscal junto ao SEFAZ.

Cenário de Sucesso Principal:

    O ator (Funcionário ou Dono) acessa o sistema e escolhe a opção "Verificar Integridade da Nota Fiscal".
    O ator insere os dados da nota fiscal a ser verificada.
    O sistema envia os dados para o SEFAZ.
    O SEFAZ retorna com a validação da nota fiscal.
    O sistema exibe o resultado da verificação para o ator.
    O caso de uso termina com o ator visualizando a confirmação da integridade da nota fiscal.

Extensões:
E.1. No Passo 4, o SEFAZ retorna um erro de validação.
E.1.1. O sistema exibe uma mensagem de erro informando o problema.
E.1.2. O ator corrige os dados e retorna ao Passo 2.

### Especificação do Caso de Uso: Salvar XML da Nota Fiscal de Saída na Nuvem

ID:
015

Nome do caso de uso:
Salvar XML da Nota Fiscal de Saída na Nuvem

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como o sistema salva o XML de uma Nota Fiscal de Saída na nuvem.

Cenário de Sucesso Principal:

    O sistema gera o XML da Nota Fiscal de Saída.
    O sistema conecta-se ao serviço de armazenamento na nuvem.
    O sistema envia o XML para a nuvem.
    O sistema confirma o armazenamento do XML.
    O caso de uso termina com o XML salvo na nuvem.

Extensões:
E.1. No Passo 3, ocorre um erro ao enviar o XML para a nuvem.
E.1.1. O sistema exibe uma mensagem de erro informando o problema.
E.1.2. O sistema tenta reenviar o XML para a nuvem.

### Especificação do Caso de Uso: Salvar XML da Nota Fiscal de Entrada na Nuvem

ID:
016

Nome do caso de uso:
Salvar XML da Nota Fiscal de Entrada na Nuvem

Atores:
Funcionário, Dono (Admin)

Visão Geral:
Este caso de uso descreve como o sistema salva o XML de uma Nota Fiscal de Entrada na nuvem.

Cenário de Sucesso Principal:

    O sistema gera o XML da Nota Fiscal de Entrada.
    O sistema conecta-se ao serviço de armazenamento na nuvem.
    O sistema envia o XML para a nuvem.
    O sistema confirma o armazenamento do XML.
    O caso de uso termina com o XML salvo na nuvem.

Extensões:
E.1. No Passo 3, ocorre um erro ao enviar o XML para a nuvem.
E.1.1. O sistema exibe uma mensagem de erro informando o problema.
E.1.2. O sistema tenta reenviar o XML para a nuvem.
