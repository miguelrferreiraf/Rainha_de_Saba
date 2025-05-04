# RAINHA DE SABÁ - ML4T 
**Autor**:
**Miguel Ferreira<br>**
**miguel.ribeiro@live.com<br>**
**gihtub.com/miguel-r-ferreira<br>**
<div align="center">
  <img src="img/QoS_muse.png" alt="Queen of Sheba" width="450" height="450">
</div>

## :books: GLOSSÁRIO
- Descrição
- Proposta
- Modelos
- Serviço
- Comunicação
- Rainha de Sabá

## :page_facing_up: DESCRIÇÃO

O projeto "Rainha de Sabá - ML4T" consiste numa **coligação de modelos de Machine Learning congregados numa aplicação robusta de processamento distribuído, que visa fazer operações no mercado financeiro de forma segura e lucrativa**. Diferentemente das aplicações convencionais, que utilizam modelos preditivos e de NLP para prever comportamentos de mercado com base em análises gráficas e notícias, esta aplicação concentra-se, além destas primeiras tarefas, em usar complexos modelos de aprendizado por reforço especializados em análise probabilística e estocástica para averiguar os riscos e retornos de cada tomada de decisão (independentemente do output do modelo preditivo avulso), para então gerenciar os riscos de forma a prover a melhor administração possível do capital, tudo isto com auxílio do **processamento distribuído** para uma evolução mais acelerada de desempenho.

**Palavras-Chave**: *machine learning, algotrading, ML4T, processamento distribuído, gerenciamento de risco, modelos preditivos, aprendizado por reforço*.

## :feelsgood: PROPOSTA

![Concept](img/monolito_concept.png)

O fluxograma acima explica o processo geral de funcionalidades da aplicação. Como podemos ver, ele **não difere muito do paradigma dos modelos de inteligência artificial financeira especializados em trading** (que, por vez, não difere-se muito do próprio paradigma CRIPS-DM da Ciência de Dados como um todo), tal qual podemos encontrar em quaisquer livros sobre o tema. Excetua-se, entretanto, o processo no qual **um modelo de gerenciamento de risco assume a decisão quanto ao tamanho das posições e ao posicionamento dos stops, além de outros objetos mais técnicos de análise**. Também é diferente do paradigma comum do ML4T a arquitetura distribuída do processamento, que é um recurso externo relativo à hospedagem e lançamento da aplicação, com algumas poucas ressalvas a serem implementadas diretamente no código fonte dos modelos. 

## :nerd_face: MODELOS 

Há dois modelos centrais, pelos quais toda a aplicação funciona. O primeiro, mais comum, é o:

:one: **Modelo preditivo**:crystal_ball: , que, no caso desta aplicação, é composto de diversos recursos teóricos tradicionais aplicados em código, para análise e previsão de datasets multivariados. 

:two: **Modelo de aprendizado por reforço para análise e gerenciamento de risco**:warning: baseado em análise probabilística e estocástica. Este segundo modelo é responsável pela releitura do paradigma do ML4T, no qual a previsão dos movimentos de mercado é substituída de sua centralidade em favor dos modelos de ML para gerenciamento de risco. 

Como este segundo modelo tende a ser mais teoricamente abstrato e a fundamentação matemática por trás deste é um tanto nebulosa, hoje, a previsão dos movimentos do mercado tornou-se o Santo Graal do ML4T, quando, na verdade, deveria ser o gerenciamento do risco. Os cientistas de dados gastam muito recursos técnicos e financeiros para prever os movimentos do mercado, quando deveriam estar investindo seus recuros de ML em ganhar dinheiro.

O Rainha de Sabá - ML4T objetiva corrigir esta abordagem, no parecer do autor, defeituosa.

## :gear: SERVIÇO

O uso concebido para esta aplicação é semelhante ao de um *hedge fund* tradicional, que paga seus clientes segundo o investimento inicial e perfil de investidor dos mesmos. Contudo, o investimento neste fundo é feito em conjunto com um "pagamento de processamento", no qual o usuário da aplicação, além de fazer um depósito inicial, auxilia também na evolução do modelo transferindo processamento via internet a partir de seu dispositivo.

## :link: COMUNICAÇÃO

Um dos aspectos mais importantes deste serviço, além de sua abordagem inovadora referente aos modelos de gerenciamento de risco, é sua versatilidade comunicacional: **os resultados de todas as operações devem imediatamente ser compartilhados através da rede social do usuário, endereço de email, aplicativo de mensagem, ou todos estes juntos, via APIs**. 

Outro ponto extensivamente considerado durante a criação da aplicação são as medidas de segurança: **a privacidade, tal qual crida e ideologicamente compreendida pelo autor do projeto, é uma virtude inegociável do serviço, desde sua concepção até o emprego da aplicação**. Concebe-se, futuramente, hospedar uma versão desta aplicação para *deep web* em domínio '.onion', para ser acessada somente através de sistemas operacionais com Tor nativo, como Tails, Whonix e Qubes. 

Esta medida, no entanto, demorará a ser implementada.

# **RAINHA DE SABÁ** <img src="img/tumblr_mqbb3a73fp1spo3yuo1_400.gif" alt="the big short" width="78" height="48">

O Rainha de Sabá surgiu com a prospota inicial de conciliar **tecnologias de machine learning distribuído ao uso do blockchain baseado em smart contracts de inteligência artificial**. No pontual momento de sua concepção, a tecnologia de blockchain não estava suficientemente desenvolvida para comportar esta arquitetura de software. Portanto, o projeto RdS se dividiu em dois braços: o **Rainha de Sabá - ML4T** (presente neste diretório) e o **RdS - DeFi** (em diretório próprio, nesta mesma conta).

A proposta empresarial do RdS - DeFi é o de uma **Organização Autônoma Descentralizada (DAO) de prestação de serviços em smart contracts especializadas em derivativos financeiros, administrada via smart contracts governamentais e emissão de tokens nativos**. Ela disponibiliza uma seara de serviços e produtos descentralizados, incluindo as inovadoras smart contracts para serviços de swap com recursos de transmissão de mensagens entre negociantes e anexação de arquivos de texto e vídeo (smart contract + swap services + aplicativo de mensagem).

Espera-se, no futuro, também converter esta aplicação para *deep web*.

Mais pode ser encontrado no diretório do projeto: https://github.com/rainha-de-saba-defi







