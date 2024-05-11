
# Projeto Disciplina: Requisitos de Software

Olá! Este repositório faz parte do projeto da disciplina de Requisitos de Software da UTFPR - Campus Cornélio Procópio. 

[![Padlet Button]][Padlet Link]

[Padlet Link]: https://padlet.com/meditous/kanban-cwkliizsdtdkxhas
[Padlet Button]: https://img.shields.io/badge/Padlet%20do%20projeto-2e66e8?style=for-the-badge

## 1. Introdução

***1.1.  Nome do Grupo***

Grupo 8:

Alefh Trindade Luz de Lima

Fábio Massashi Suzuki

Pedro Augusto Morais

Vitor Barbosa Hilário


***1.2.  Nome do Sistema***

KiStock

***1.3.  Propósito do Sistema***

Este documento apresenta os requisitos dos usuários a serem desenvolvidos pela *KiStock*, fornecendo aos desenvolvedores as informações necessárias para o projeto e implementação, assim como para a realização dos testes e homologação do sistema.

O objetivo do sistema *KiStock* é *gerenciar o estoque de forma otimizada e eficiente, com registros de produtos, relatório de compras e vendas, além de ter notificações de produtos que irão vencer e contas a pagar*.



***1.2.  Público Alvo***

Este documento se destina às pessoas cujo os interesses estão alinhados com obtenção de um software para gerenciamento e gestão de estoque em sua empresa ou comércio, ou empreendimento.

***1.3. Descrição dos usuários***

**Perfil do Usuário**

| Perfil | Empreendedor | Analista de Estoque |
| -------- | -------- | --------|
| Porcentagem de usuário | 80% | 20% |
| Faixa etária | [18, 50] | [20, 45] |
| Nível de instrução | Alto | Médio |
| Experiência com a tecnologia | Baixo | Alto |

**Personas**

| Persona 1 | Persona 2 | Persona 3 |
| --------- | --------- | ----------|
| ![2](https://github.com/fabio-SZK/grupo-8-kistock/assets/81326138/716d5aa5-90b6-49c2-9e6b-a7a729eefcb1) | ![3](https://github.com/fabio-SZK/grupo-8-kistock/assets/81326138/7189474c-1faa-490f-afeb-06c067a21c8b) | ![4](https://github.com/fabio-SZK/grupo-8-kistock/assets/81326138/7d9b21f2-4ee4-4bfd-b5dd-aca0aa53bdf3) |

**Análise de Tarefas - Situação atual**

- As pessoas possuem o hábito de organizar e gerenciar o seu estoque utilizando planilhas como o Excel ou Google Sheets, executando todas as movimentações manualmente entre as células do programa.

- Programas de gerenciamento de planilhas, cadernetas, arquivos.

- Elas precisam ter um ótimo domínio de scripts integrados nas planilhas, cálculos, burocracias e tributação de produtos.

**Análise de Tarefas - Depois da implantação**

- As pessoas usariam um software com automações de controle de estoque, incluindo uma interface interativa fornecida pelo programa, que faria uma abstração da lógica de negócio responsável pelos cadastros, funcionários, fornecedores e entrada e saída de produtos.
                                    
- Aplicativo desktop para gerenciamento de estoque e app mobile para visualização de relatórios em tempo real.

- Os utilizadores do programa precisam ter um mínimo de conhecimento sobre a utilização de um computador, isto é, interagir com o programa para utilizar as funcionalidades.

**Cenário - Antes**

Jeff trabalha como analista de estoque numa fábrica de cosméticos animais, para automatizar e facilitar a organização do estoque, ele anota a entrada e a saída de produtos e encaminha para a planilha de Excel para deixar registrado. Por meio dessa tecnologia, Jeff encaminha as anotações atualizando diariamente cada entrada/saída de produtos do estoque da fábrica.

Jeff tem como prazo fazer as atualizações de estoque até as 18:00 horas. Para manter a produção da fábrica em alerta de qual cosmético ou matéria-prima está em falta, na planilha, Jeff encaminha a atualização diária.

Celina, a produtora da fábrica não consegue fazer a tempo os produtos, pois quando ela pede o material no Whatsapp, as mensagens se coincidem com as outras mensagens não relacionadas com o assunto, deixando muitas vezes, desorganizado a produção e a manutenção do estoque.

**Cenário - Depois**

Jeff trabalha como analista de estoque numa fábrica de cosméticos animais, onde sua principal responsabilidade é manter o controle preciso das entradas e saídas de produtos. Para otimizar esse processo e garantir que a produção da fábrica seja eficiente, a empresa implementou o sistema chamado KiStock.

O KiStock é uma ferramenta completa que permite cadastrar fornecedores, produtos e históricos detalhados de todas as transações relacionadas ao estoque. Além disso, ele verifica a disponibilidade de cada item em estoque, tanto para venda quanto para fabricação. Com o KiStock, a fábrica automatizou e facilitou a manutenção do estoque, proporcionando uma maneira organizada e eficaz de gerenciar todas as operações. Jeff consegue atualizar todas as informações sobre o estoque, deixando a comunicação entre o estoque e a produção da fábrica mais eficiente e automatizada.

Agora, Celine não precisa mais depender do Whatsapp para acompanhar as atualizações do estoque. Em vez disso, ela faz login no KiStock para acessar todas as informações necessárias de forma rápida e simplificada, garantindo uma produção mais eficiente e organizada, entregando e repondo o estoque com produtos cosméticos.


## 2. Documentos gerais no repositório

***2.1. Requisitos funcionais***


|Identificador| Descrição|
| -------- | -------- |
|RF01| O software deve permitir o cadastro de funcionários membros e funcionário administrador - Alta|
|RF02| O software deve permitir ao funcionário adiministrador o cadastro de produtos e fornecedores - Alta|
|RF03| O software deve permitir aos funcionários ver o status do estoque (quantidade de produtos disponíveis) - Alta|
|RF04| O software deve permitir aos funcionários a possibilidade que façam a leitura por código de barra de produtos para facilitar o processo de inventário de estoque - Média|
|RF05| O software deve manter um histórico de entrada e saída de produtos em um determinado tempo para auxiliar no controle do estoque. - Alta|
|RF06| O software deve permitir aos funcionários a geração de relatórios de entrada e saída de produtos - Alta|
|RF07| O software deve permitir aos funcionários o acesso às informações do estoque (produtos, histórico e registros) - Alta|
|RF08| O software deve notificar ao funcionário quando uma conta a pagar estiver prestes a vencer - Média|
|RF09| O software deve apresentar as informações do estoque em uma tela única de forma organizada para facilitar a leitura pelos funcionários - Baixa|
|RF10| O software deve efetuar análises do estoque utilizando machine learning - Alta|
|RF11| O software deve permitir que os funcionários apliquem metodologias de gerenciamento de estoque sobre as informações de forma automática - Média |


***2.2. Requisitos Não-Funcionais***

|Identificador| Descrição|
| -------- | -------- |
|RNF01| O software deve responder as requisições no intervalo entre 0,5 à 2 segundos - Média|
|RNF02| O software deve ter um tutorial com indicativos de clique para as funcionalidades - Média|
|RNF03| O software deve criptografar todas as informações aos salvar os dados - Alta|
|RNF04| O software deve funcionar tanto para Web quanto para Mobile - Alta|
|RNF05| O software deve salvar o login e senha do usuário por termpo determinado.Ex:1 semana - Baixa|
|RNF06| O software deve enviar notificações para alertar os funcionários se o produto está perto da data de validade ou a quantidade de produtos no estoque estiver acabando - Baixa|
|RNF07| O software deve permitir o uso do app em modo offline, sincronizando os dados após restaurar a conexão com a internet - Média|
|RNF08| O software deve facilitar a comunicação com sistema de logística para otimizar a gestão de entregas e recebimento de mercadoria - Alta|
|RNF09| O software deve ter um sistema de backup avançado e recuperação de dados para proteger as informações do estoque caso ocorra perdas acidentais ou falhas no hardware - Alta|
|RNF10| O software deve ter um suporte multilíngue disponibilizado tanto para Mobile quanto para o Web em diferentes idiomas - Média|

*<Link para a pasta de requisitos de sistema .>*

***2.3. Histórias de Usuários***

1.Como gerente da empresa,eu quero poder cadastrar novos funcionários,para ter uma organização maior da equipe da empresa.

2.Como fabricante,eu quero poder verificar o estoque,para ter um maior controle dos produtos disponíveis para fabricação.

3.Como funcionário,eu quero receber uma notificação de contas prestes a vencer,para evitar faturas não pagas.

4.Como estoquista,eu quero ter a entrada/saída de todos produtos e matérias-priamas do estoque,para ter um desempenho maior na fabricação e lucro da empresa.

5.Como funcionário administrador,eu quero ser capaz de cadastrar novos produtos e fornecedores,para manter o estoque atualizado.

6.Como funcionário,eu quero acessar as informações do estoque(produtos,histórico e registros),para realizar minhas atividades de forma eficiente.

7.Como funcionário,eu quero utilizar análises do estoque utilizando machine learning,para prever demandas futuras e otimizar o gerenciamento de estoque.

8.Como funcionário,eu quero aplicar metodologias de gerenciamento de estoque sobre as informações de forma automática,para melhorar a eficiência e reduzir erros.


***Entrevista***

[Link para entrevista](https://drive.google.com/file/d/1iSvgwKbPu8mS0f2RmkZpzk3xLLH8myhZ/view?usp=sharing)

Por que? (objetivos da entrevista).
Coletar informações importantes para o desenvolvimento mais eficiente e adequado para o gerenciamento de estoque.

Quem? (perfil).
Joel Roberto, empresário.

Quando? (data, horário,duração).
01/05/2024.

Onde? (local).
Ambiente virtual.

Como? (definição dos tipos de questões e registro).
Pergunta fechada.


| Pergunta | Descrição |
|----------|-----------|
| 1PGT | Como você controla os vencimentos dos produtos? |
| 2PGT | Como faz o rastreio da quantidade de produtos no estoque? |
| 3PGT | Como você realiza o controle de estoque atualmente na sua fábrica? |
| 4PGT | Como são feitos os relatórios de entrada e saída de produtos da sua fábrica? |
| 5PGT | Quais notas fiscais você precisa emitir? |
| 6PGT | Como você gerencia o cadastro de Produtos, Fornecedores, Clientes e Empregados? |
| 7PGT | Como é o seu controle de estoque atualmente e quais funcionalidades tecnológicas gostaria de ter presentes nesse seu controle? |
| 8PGT | Quais os seus gastos atualmente com o gerenciamento de Produtos, Vendas e Compras? |


***2.3. Protótipos***

*<Link para a pasta com os protótipos.>*

## Referências

*<Esta seção é destinada à descrição das referências utilizadas pelo documento, como por exemplo, URLs e livros. Ver exemplo a seguir:>*

[1] “Glossário da _USina_”, <_id_doc glossário_>, Versão <_versão_>. Localização: <_localização_>.
