
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


|Identificador| Descrição| Prioridade|
| -------- | -------- | -------- |
|RF01| O software deve permitir o cadastro de funcionários membros e funcionário administrador. |Alta|
|RF02| O software deve permitir ao funcionário administrador o cadastro de produtos e fornecedores |Alta|
|RF03| O software deve permitir aos funcionários ver o status do estoque (quantidade de produtos disponíveis). |Alta|
|RF04| O software deve permitir aos funcionários a possibilidade de que se faça a leitura de produtos por um leitor de código de barras, como meio de facilitar o processo de inventário de estoque, isto é, substituindo o processo de escrita de códigos GTIN em planilhas ou papéis de forma manuscrita. |Média|
|RF05| O software deve manter um histórico de entrada de produtos, registrando as compras pela Nota Fiscal de Entrada gerada pelo fornecedor, por um período mínimo de 5 anos. |Alta|
|RF06| O software deve manter um histórico de saída de produtos, registrando as venda pela Nota Fiscal de Saída gerada pelo cliente usuário do controle de estoque, por um período mínimo de 15 anos. |Alta|
|RF07| O software deve permitir aos funcionários a geração de relatórios de entrada e saída de produtos, seja diário, semanal, mensal, semestral ou anual. |Alta|
|RF08| O software deve alertar na aba de notificações da página inicial com antecedência ao funcionário quando uma conta a pagar advinda de fornecedores tiver seu vencimento apontado para os próximos 3 dias. |Média|
|RF09| O software deve apresentar as informações do estoque em uma coluna com scroll à esquerda da tela principal - exibida assim que o usuário é autenticado no sistema, assim como um drawer layout, possibilitando fácil acesso a uma informação assim que selecionado um item à esquerda, como vendas, compras, estoque com os produtos, dashboard e o emissor de nota fiscal. |Baixa|
|RF10| O software deve efetuar análises dos valores faturados nas vendas de todos os produtos que houveram movimentações, gerando gráficos semanais, mensais, semestrais e anuais, possibilitando que o usuário cliente possa avaliar melhor as suas decisões na compra de novos produtos. |Alta|
|RF11| O software deve ter um tutorial com indicativos de clique para as funcionalidades. | Média|
|RF12| O software deve enviar notificações para alertar os funcionários avisando de que um determinado produto está perto da data de validade ou a quantidade de produtos no estoque estiver acabando com 7 dias de antecedência. |Baixa|
|RF13| O software deve permitir o uso do app em modo offline, sincronizando os dados após restaurar a conexão com a internet. | Média|
|RF14| O software deve facilitar a relação com a logística para otimizar a gestão de entregas e recebimento de mercadoria, gerando e imprimindo de forma automática notas fiscais de vendas e informações de entrega para a etiquetagem de produtos. | Alta|

***2.2. Requisitos Não-Funcionais***

|Identificador| Descrição| Prioridade|
| -------- | -------- | -------- |
|RNF01| O software deve responder às requisições no intervalo entre 0,5 à 2 segundos. | Média|
|RNF02| O software deve criptografar todas as informações aos salvar os dados. | Alta|
|RNF03| O software deve funcionar tanto para Web quanto para Mobile. | Alta|
|RNF04| O software deve permitir o uso do app em modo offline, sincronizando os dados após restaurar a conexão com a internet. | Média|
|RNF05| O software deve facilitar a relação com a logística para otimizar a gestão de entregas e recebimento de mercadoria, gerando e imprimindo de forma automática notas fiscais de venda e informações de entrega para a etiquetagem de produtos. | Alta|
|RNF06| O software deve ter um sistema de backup avançado e recuperação de dados para proteger as informações do estoque caso ocorra perdas acidentais ou falhas no hardware. | Alta|
|RNF07| O software deve ter um suporte multilíngue disponibilizado tanto para Mobile quanto para o Web em diferentes idiomas. | Média|
|RNF08| O software deve ser fácil de manter e atualizar, permitindo que desenvolvedores possam corrigir erros, adicionar novas funcionalidades e melhorar o desempenho de forma eficiente. | Alta|
|RNF09| O software deve permitir migração tranquila entre versões e atualizações sem causar interrupções significativas no serviço. | Alta|
|RNF10| O software deve ser acessível para pessoas com deficiências, seguindo padrões e diretrizes de acessibilidade. | Média|
|RF12| O software deve salvar o token de autenticação encriptado do usuário nos cookies do navegador, quando na web, e em key-stores, quando dispositivos móveis, por um período de 30 dias, até que se renove com outro login após a sua expiração. |Alta|

*<Link para a pasta de requisitos de sistema .>*

***2.3. Histórias de Usuários***
|Identificador| Descrição|
| -------- | -------- |
|HU01| Como gerente da empresa, eu quero poder cadastrar novos funcionários, para ter uma organização maior da equipe da empresa. |
|HU02| Como operador de estoque, eu quero pesquisar produtos no sistema pelo nome ou código, para encontrar rapidamente as informações necessárias. |
|HU03| Como funcionário, eu quero receber uma notificação de contas prestes a vencer,para evitar faturas não pagas. |
|HU04| Como gerente financeiro, eu quero gerar relatótios de inventário, para ter uma visão clara das quantidades e valores dos produtos em estoque. |
|HU05| Como funcionário administrador, eu quero ser capaz de cadastrar novos produtos e fornecedores, para manter o estoque atualizado. |
|HU06| Como funcionário, eu quero acessar as informações do estoque(produtos, histórico e registros), para realizar minhas atividades de forma eficiente. |
|HU07| Como gerente de vendas, eu quero poder visualizar as vendas representadas em uma dashboard com o custo,faturamento e lucro, ordenado por data. |
|HU08| Como funcionário, eu quero poder reutilizar arquivos de planível .xlsx e .csv com informações de produtos e estoque para adicionar novos registro no sistema.  |


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
