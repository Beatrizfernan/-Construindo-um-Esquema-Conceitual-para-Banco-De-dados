Controle e Gerenciamento de Execução de Ordens de Serviço em uma Oficina Mecânica
Este projeto consiste na criação de um esquema conceitual para um sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica. O objetivo é proporcionar uma visão geral do contexto e dos componentes principais do sistema.

Descrição do Contexto
O sistema foi desenvolvido para atender às necessidades de uma oficina mecânica, onde clientes levam seus veículos para reparos ou revisões periódicas. Cada veículo é designado a uma equipe de mecânicos, que identifica os serviços necessários e preenche uma Ordem de Serviço (OS) com data de entrega.

A partir da OS, é calculado o valor de cada serviço, consultando uma tabela de referência de mão-de-obra. O valor das peças também é incluído na OS. O cliente então autoriza a execução dos serviços.

A mesma equipe de mecânicos avalia e executa os serviços. Cada mecânico possui um código, nome, endereço e especialidade.

Cada OS é identificada por um número único e possui informações como data de emissão, valor total, status e data prevista para conclusão dos trabalhos.

Entidades Principais
Cliente: Representa os clientes que levam seus veículos para a oficina. Pode ter atributos como nome, endereço, contato, etc.
Veículo: Representa os veículos que são deixados na oficina para reparo ou revisão. Pode ter atributos como marca, modelo, ano, placa, etc.
Mecânico: Representa os mecânicos que trabalham na oficina. Possui atributos como código, nome, endereço, especialidade, etc.
Ordem de Serviço (OS): Representa as ordens de serviço geradas para cada veículo. Possui atributos como número, data de emissão, valor total, status, data prevista para conclusão, etc.
Serviço: Representa os serviços a serem realizados em cada veículo. Pode incluir informações como descrição, valor, etc.
Peça: Representa as peças que são utilizadas nos serviços. Pode ter atributos como nome, código, valor, etc.
Relacionamentos
Cliente - Veículo: Relacionamento um-para-muitos indicando que um cliente pode ter vários veículos.
Veículo - Ordem de Serviço: Relacionamento um-para-muitos indicando que um veículo pode ter várias ordens de serviço.
Mecânico - Ordem de Serviço: Relacionamento um-para-muitos indicando que um mecânico pode estar associado a várias ordens de serviço.
Ordem de Serviço - Serviço: Relacionamento um-para-muitos indicando que uma ordem de serviço pode incluir vários serviços.
Ordem de Serviço - Peça: Relacionamento um-para-muitos indicando que uma ordem de serviço pode incluir várias peças.
