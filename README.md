![fundo](https://github.com/AlbertoFAraujo/DashEnade2021/assets/105552990/38711a77-0076-4d26-8a5e-bb9bb9a3fb34)

# 📊DASHBOARD INDICADORES DE PERFORMANCE

### Tecnologias utilizadas: 
| [<img align="center" alt="Python" height="60" width="60" src="https://api.iconify.design/vscode-icons/file-type-excel.svg">](https://support.microsoft.com/en-us/excel) |
|:---:|
| Excel |
<hr>

### Objetivo:

O objetivo da análise é extrair informações de performances individuais dos colabores de uma empresa fictícia para tomadas de decisão. Trata-se de um cenário comum de gestão de operações, na qual é necessário com base em parâmetros de produção, qualidade, tma, entre outros, determinar se um analista está atuando dentro ou fora do esperado e a partir disso tomar as devidas medidas (feedbacks, acompanhamento individual, sanções, dentre outras conforme as políticas prevista pela empresa).

**Obs:** Todos os dados são fictícios e gerados aleatoriamente. A ideia da criação desse *dashboard* é utilizar somente tabelas com funções básicas e dispensar o uso de programação e/ou tabelas dinâmicas.
<hr>

### Etapas do projeto:

1. Definição do objetivo da análise e geração da base de valores fictícios;
2. Tratamento dos dados (Limpeza, transformações, formatações, criação de tabelas auxiliares e filtros-chave);
3. Identificação das métricas-alvo e escolha das visualizações gráficas adequadas para cada cenário;
4. Criação do layout e composição de paleta de cores;
5. Teste de qualidade e eficácia do *dashboard* (garantir que todos os gráficos estejam funcionando corretamente e que os dados estejam sendo atualizados).
<hr>

### Tempo de Execução:

O tempo estimado para a execução de todas as etapas é de 1 dia.

### Projeto Final a ser desenvolvido:

![DashOp_print](https://github.com/AlbertoFAraujo/DashOperacoes/assets/105552990/bc852084-dfcc-4d75-be13-5eb007a94861)
<hr>

### Execução das Etapas:

#### 1. Definição do objetivo da análise e geração da base de valores fictícios;

O objetivo da análise é extrair informações de performances individuais dos colabores de uma empresa fictícia para tomadas de decisão. Trata-se de um cenário comum de gestão de operações, na qual é necessário com base em parâmetros de produção, qualidade, tma, entre outros, determinar se um analista está atuando dentro ou fora do esperado e a partir disso tomar as devidas medidas (feedbacks, acompanhamento individual, sanções, dentre outras conforme as políticas prevista pela empresa).

A base de dados foi gerada de forma aleatória, mas dentro do cenário de uma operação comum de crédito, com variáveis padrões a serem analisadas.

#### 2. Tratamento dos dados (Limpeza, transformações, formatações, criação de tabelas auxiliares e filtros-chave);
- Foi gerado nomes fictícios a partir do site [Mockaroo - Random Data Generator and API Mocking Tool | JSON / CSV / SQL / Excel](https://www.mockaroo.com/);
- As demais variáveis geradas são explicadas abaixo:

    | Variáveis: | Significado: |  
    | --- | --- |   
    | Fila_atuacao | Subdividida em: Agendamento, Contato, Vendas. Trata-se da fila/etapa ou esteira de atuação na qual o analista está realizando o tratamento da demanda. |
    | UF_Loja | Subdividida em 27 valores correspondente às siglas dos estados do Brasil. |
    | Analista | Analista que realizou o tratamento da proposta. |
    | Data | Data na qual foi realizado o tratamento da proposta. |
    | Status | Subdividida em: Aprovação, Pendencia, Reprova ou Fraude. Trata-se da definição final do analista em relação à proposta tratada, ou seja, como classificou o tratamento final. |
    | TMA | Tempo médio de Análise da proposta. |
    | Valor | Valor equivalente da proposta. |
<hr>

#### 3. Identificação das métricas-alvo e escolha das visualizações gráficas adequadas para cada cenário:

Os gráficos foram escolhidos conforme a disposição dos dados das variáveis e que melhor atendem ao objetivo e visualização das informações;
<hr>

#### 4. Criação do layout e composição de paleta de cores:

O layout foi pensando na disposição das informações, como a ideia é obter informações rápidas sobre a performance do analista selecionado através do filtro do painel lateral, o layout apresenta as métricas-alvo para que essa análise seja realizada de forma eficiente e clara.

- **Gráfico “Status”:** O objetivo desse gráfico é exibir o percentual dos status das propostas e garantir que o analista esteja dentro dos parâmetros médio da operação, ou seja, controlar o número de pendências, fraudes retidas, reprovas e aprovações. Com isso, o gestor é capaz de monitorar os indicadores de forma visual e garantir que esteja controlado e dentro dos aceites da política da empresa.

 - **Gráfico “Produção Fila”:** O objetivo desse gráfico é exibir de forma comparativa a produção do analista por fila/esteira de tratamento, garantindo que o mesmo não esteja atuando de forma desproporcional nas demais, às vezes por serem mais rápidas, menos etapas…

- **Gráfico “TMA”:** O objetivo desse gráfico é demonstrar de forma visual o tempo médio de análise em cada uma das filas de tratativa, ou seja, se o analista está dentro do parâmetro médio global de cada uma das filas, visto que, cada fila possuem um TMA Médio que deve ser seguido, sendo calculado por diversos fatores e com base em dados histórico. O gráfico pode ser implementado com uma meta por fila, por exemplo, garantindo de forma visual e intuitiva todas as vezes que o analista esteja fora ou dentro da meta de TMA por fila.

- **Gráfico “Produção x Dia”:** O objetivo desse gráfico é exibir de forma clara a produção por dia do analista filtrado, e em tempo, demonstrar em qual dia o mesmo esteve abaixo ou acima da meta através das cores do gráfico. O gráfico pode ainda ser implementado em exibir informações de quantos dias o analista esteve abaixo, acima…para que o gestor possa criar um plano de ação com base nesse resultado e garantir a entrega da meta e/ou entender por quais motivos o analista esteve fora da margem da meta.

- **Gráfico “Fraude x Estado”:** O gráfico apresenta o número de fraudes por estado, podendo ser correlacionado de forma global entre a operação e garantir planos de ações para futuras propostas derivadas do estado ou de alerta.

- **Gráfico “Valor Retido”:** O gráfico apresenta o controle de valores retidos por região do Brasil, também pode ser utilizado como um parâmetro de alerta, seguido de um plano de ação para as futuras derivações de propostas e cuidados a serem tomados, identificar padrões de ataques e afins.

- **Gráfico “Fraudes”:** O gráfico apresenta a porcentagem de fraudes derivadas em cada uma das filas/esteira de análise, podendo ser correlacionado de forma global e de alerta para as futuras derivações.

- **Paletas de cores utilizadas:** O uso de paletas de cores torna-se a visualização mais atraente, portanto deve ser escolhida seguindo uma lógica de cores, geralmente utilizo com base na logo do produto, empresa, marca e afins.

| RGB (255, 217, 102) | RGB (132, 60, 12) | RGB (244, 177, 131) |
|-------------------|-------------------|-------------------|
| ![255_217_102](https://github.com/AlbertoFAraujo/DashOperacoes/assets/105552990/d652794c-c580-4a7f-89ca-e4b696a12449) | ![132_60_12](https://github.com/AlbertoFAraujo/DashOperacoes/assets/105552990/5b463a1b-6387-4f49-ae79-63b5688c991b) | ![244_177_131](https://github.com/AlbertoFAraujo/DashOperacoes/assets/105552990/36c2d537-830a-48d8-b6ea-6974350ba609) |
<hr>

#### 5. Teste de qualidade e eficácia do *dashboard* (garantir que todos os gráficos estejam funcionando corretamente e que os dados estejam sendo atualizados)

Foi realizado diversos testes para garantir que todos os gráficos estivessem sendo alterados automaticamente, assim como os rótulos não sendo impedidos de serem visualizados corretamente.
<hr>

### Resultado final

![DashOp_video](https://github.com/AlbertoFAraujo/DashOperacoes/assets/105552990/ca6457d7-345e-44c1-835a-fa653a95d877)

