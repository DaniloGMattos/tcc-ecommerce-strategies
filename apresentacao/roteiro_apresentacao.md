# Roteiro de Apresentação - TFG
## Cenário Atual do Desenvolvimento de Plataformas de E-commerce: Estratégias Técnicas e Impacto na Receita das Empresas

**Aluno:** Danilo Godofredo de Mattos (Mat. 2018009986)
**Orientadora:** Profa. Bárbara Pimenta Caetano
**Curso:** Engenharia de Computação - UNIFEI

---

## SLIDE 1: Contexto e Problema

**[Iniciar]**
Bom dia a todos. Meu trabalho investiga o cenário atual do desenvolvimento de plataformas de e-commerce, com foco nas estratégias técnicas e seu impacto na receita das empresas.

**[Contextualizar o problema]**
O e-commerce cresceu bastante nas últimas décadas. Segundo dados da Shopify, as vendas globais devem passar de 6,56 trilhões de dólares em 2025 para mais de 8 trilhões até 2028. Mas esse crescimento traz desafios técnicos sérios: como garantir performance quando o tráfego aumenta? Como melhorar a experiência do usuário para converter mais vendas? Como usar inteligência artificial de forma efetiva?

**[O problema real]**
O que percebi trabalhando com e-commerce é que há muita informação técnica dispersa na literatura. Vários estudos falam sobre arquitetura de software, outros sobre otimização de interface, outros sobre sistemas de recomendação. Mas falta uma visão integrada que conecte essas decisões técnicas com o impacto financeiro real nas empresas. Um engenheiro ou gestor que vai desenvolver uma plataforma não tem clareza sobre qual decisão técnica vai trazer mais retorno.

**[Transição]**
Por isso resolvi fazer este trabalho: mapear o estado da arte nessa área e fazer experimentos práticos que demonstrem o impacto real dessas decisões.

---

## SLIDE 2: Motivação e Relevância

**[Três aspectos principais]**
A motivação para este trabalho veio de três pontos que observei na prática:

**Primeiro - Impacto econômico direto:**
Decisões técnicas erradas custam dinheiro. Há um caso documentado do Alibaba.com que ilustra bem isso: quando implementaram Progressive Web App, tiveram 76% de aumento nas conversões. Setenta e seis por cento! Só essa mudança técnica. Isso mostra que escolhas de arquitetura e tecnologia não são apenas questões de engenharia, são questões de negócio.

**Segundo - Complexidade das escolhas:**
Hoje um desenvolvedor precisa decidir entre arquitetura monolítica ou microsserviços, entre aplicação web tradicional ou PWA, entre usar filtragem colaborativa ou deep learning para recomendação. Cada escolha tem ganhos e perdas em custo, complexidade e performance. As empresas precisam de orientação baseada em evidências para tomar essas decisões.

**Terceiro - Lacuna entre pesquisa e prática:**
A literatura tem estudos isolados sobre cada aspecto: performance arquitetural, otimização de UX, algoritmos de IA. Mas falta trabalho que integre essas dimensões e mostre o impacto conjunto na receita. É isso que este TFG busca fazer.

**[Contexto pessoal]**
Além disso, trabalho há alguns anos com plataformas de e-commerce e assinaturas, então pude trazer essa experiência prática para o trabalho acadêmico.

---

## SLIDE 3: Objetivos do Trabalho

**[Objetivo geral]**
O objetivo geral é analisar o cenário atual do desenvolvimento de plataformas de e-commerce, identificando as principais estratégias técnicas e avaliando o impacto delas na receita das empresas.

**[Objetivos específicos - ir comentando cada um]**
Para isso, dividi em cinco objetivos específicos:

**1. Mapear estratégias arquiteturais**
Identificar as principais abordagens arquiteturais usadas hoje - monolíticas, microsserviços, event-driven - e analisar os trade-offs de cada uma. Quando vale a pena a complexidade de microsserviços? Quando um monólito é suficiente?

**2. Analisar estratégias de UX e interface**
Examinar técnicas de otimização da experiência do usuário, especialmente em mobile. Progressive Web Apps, otimizações de performance, design responsivo. O que realmente impacta a conversão?

**3. Avaliar o papel da inteligência artificial**
Investigar como IA e machine learning estão sendo aplicados: sistemas de recomendação, personalização de conteúdo, geração automática de descrições de produtos. Qual o retorno real desses investimentos?

**4. Correlacionar decisões técnicas com receita**
Este é o objetivo central: identificar a relação mensurável entre decisões técnicas específicas e métricas de negócio como taxa de conversão, valor médio de pedido, receita recorrente.

**5. Identificar lacunas e oportunidades**
Mapear o que ainda falta na literatura e quais são as oportunidades de pesquisa futura nessa área.

---

## SLIDE 4: Metodologia - Revisão da Literatura

**[Duas frentes]**
A metodologia do trabalho tem duas frentes principais: revisão bibliográfica e experimentos práticos.

**[Revisão bibliográfica]**
Na revisão, analisei 12 trabalhos recentes que cobrem as principais áreas do desenvolvimento de e-commerce. Organizei em quatro eixos temáticos:

**Arquitetura e Performance:**
Estudos como o do Ubur comparando arquitetura event-driven com monolítica, trabalho do Zhao mapeando 109 estudos sobre análise de desempenho arquitetural. O que esses estudos mostram é que não existe arquitetura "melhor" em absoluto - depende do contexto, volume de transações, padrão de crescimento.

**UX e Interface:**
Vários trabalhos sobre impacto da experiência do usuário nas conversões. Destaque para estudos sobre otimização mobile na Indonésia, sobre SEO e velocidade de carregamento, e principalmente os casos de sucesso com PWA. Além do Alibaba que mencionei, há vários outros casos documentados.

**Inteligência Artificial:**
Trabalhos sobre IA generativa aplicada a e-commerce, sistemas de recomendação. Tem um estudo interessante do Nguyen sobre sistema de recomendação para a H&M que compara LightGBM com deep neural networks. O LightGBM performou melhor e com menos complexidade.

**Métricas e Conversão:**
Análise da jornada do usuário, taxas de conversão por fonte de tráfego, identificação de gargalos no processo de checkout. O trabalho do Muralidhar mostra como a análise detalhada das métricas pode revelar oportunidades de otimização.

---

## SLIDE 5: Metodologia - Experimentos Práticos (Achievece)

**[Experimentos reais]**
Além da revisão teórica, estou fazendo experimentos práticos na plataforma Achievece, que é uma plataforma de assinaturas de audiobooks que desenvolvi. Ela tem cerca de 30 mil visitantes mensais e receita diária na ordem de 2.500 dólares, então dá para fazer testes estatisticamente significativos.

**[Estrutura dos experimentos]**
Os experimentos seguem metodologia rigorosa de A/B testing. Divido o tráfego aleatoriamente entre versão de controle e versão de teste, rodo por tempo suficiente para ter significância estatística, e analiso o impacto em métricas como taxa de conversão, receita média por usuário, lifetime value.

**[Três dimensões de experimentos]**

**1. Performance e Core Web Vitals**
Estou testando otimizações de carregamento, lazy loading de imagens, code splitting. Medindo o impacto direto na taxa de conversão quando melhoro LCP, FID e CLS. A hipótese é que cada melhoria de 100ms no tempo de carregamento deve aumentar a conversão.

**2. UX e fluxo de checkout**
Testando diferentes designs de checkout, simplificação de formulários, indicadores de progresso. Um experimento interessante é testar checkout em uma página versus multipáginas. Outro é sobre transparência de preços - mostrar ou não o preço total logo no início.

**3. Estratégias de retenção em assinaturas**
Como a Achievece trabalha com modelo de assinatura recorrente, estou testando estratégias de upsell e ofertas de retenção. Por exemplo: oferecer upgrade de plano durante o checkout, oferecer desconto quando o usuário tenta cancelar. Medindo o impacto em MRR, churn rate e lifetime value.

**[Coleta de dados]**
Todo experimento é instrumentado com tracking detalhado. Uso ferramentas de analytics para coletar dados de comportamento, testes de significância estatística para validar resultados.

---

## SLIDE 6: Resultados Esperados e Cronograma

**[O que espero obter]**
Com este trabalho, espero gerar três tipos de resultados:

**1. Framework de análise integrada**
Um framework que conecte as diferentes dimensões técnicas - arquitetura, UX, IA - com métricas de negócio. A ideia é que outro engenheiro ou gestor possa usar esse framework para tomar decisões mais informadas sobre onde investir recursos técnicos.

**2. Evidências quantitativas**
Dados reais dos experimentos na Achievece mostrando o impacto de cada otimização. Por exemplo: "melhorar LCP de 3s para 1.5s aumentou conversão em X%", "implementar ofertas de retenção reduziu churn em Y%". Isso vai além da teoria e traz números concretos.

**3. Identificação de lacunas**
Mapear claramente o que ainda falta ser estudado. A revisão bibliográfica já está mostrando várias áreas pouco exploradas, especialmente sobre estratégias de assinatura e relação quantitativa entre decisões técnicas e receita em diferentes contextos de negócio.

**[Cronograma]**
O cronograma está distribuído ao longo de 2025:

- **Primeiro trimestre:** Finalizando revisão bibliográfica, definindo protocolos dos experimentos
- **Segundo trimestre:** Executando os experimentos na Achievece, coletando dados
- **Terceiro trimestre:** Análise estatística dos resultados, escrita do trabalho final
- **Quarto trimestre:** Revisão, ajustes finais, preparação da defesa

**[Considerações finais]**
Este trabalho busca contribuir tanto para a academia quanto para a prática. Para a academia, trazendo evidências empíricas sobre o impacto de decisões técnicas. Para a prática, oferecendo orientação baseada em dados para quem desenvolve plataformas de e-commerce.

Obrigado pela atenção. Estou aberto a perguntas.

---

---

# PERGUNTAS E RESPOSTAS PARA A DEFESA

## Perguntas sobre Metodologia

### P1: Por que você escolheu apenas 12 artigos para a revisão bibliográfica? Não seria necessário um número maior para ter representatividade?

**R:** A escolha dos 12 artigos foi criteriosa e baseada em cobertura temática, não apenas em quantidade. Priorize trabalhos recentes (maioria de 2023-2025) que representam o estado da arte em cada dimensão do problema: arquitetura, UX, IA e métricas. Além disso, incluí estudos de caso documentados como o do Alibaba.com e a coleção de cases de PWA que trazem evidências quantitativas reais. O trabalho do Zhao et al., por exemplo, é um mapeamento sistemático que já analisou 109 estudos sobre análise de desempenho arquitetural, então indiretamente estou coberto por uma revisão muito mais ampla. Considero que esses 12 trabalhos dão uma visão sólida e atualizada do cenário atual.

### P2: Você mencionou que vai fazer experimentos na plataforma Achievece. Como você garante que os resultados são generalizáveis para outras plataformas de e-commerce?

**R:** Essa é uma limitação reconhecida do trabalho. A Achievece é um caso específico - modelo de assinatura, segmento de audiobooks. Os resultados não vão ser universalmente aplicáveis a qualquer e-commerce. Mas existem alguns pontos que tornam os experimentos relevantes: primeiro, o volume de tráfego (30 mil visitantes mensais) permite significância estatística. Segundo, muitos dos testes - como otimização de Core Web Vitals, simplificação de checkout - têm princípios que se aplicam a diferentes contextos. Terceiro, a própria revisão bibliográfica complementa os experimentos mostrando evidências de outros contextos. O trabalho deixa claro as limitações de generalização e sugere que estudos futuros repliquem os experimentos em outros segmentos.

### P3: Como você vai garantir rigor estatístico nos experimentos de A/B testing?

**R:** Vou seguir práticas estabelecidas de experimentação: tamanho de amostra calculado com base em poder estatístico desejado (geralmente 80%) e significância de 95%. Divisão aleatória do tráfego entre grupos de controle e teste. Duração mínima de experimentos para capturar variações de comportamento ao longo da semana. Vou usar testes de hipótese apropriados - qui-quadrado para taxas de conversão, teste t para médias de receita. E vou reportar não apenas p-values mas também intervalos de confiança e tamanho de efeito. Pretendo usar ferramentas como Python com scipy e statsmodels para as análises.

## Perguntas sobre Conteúdo e Resultados

### P4: Você falou sobre o caso do Alibaba.com com 76% de aumento nas conversões. Mas esse é um caso isolado de uma empresa gigante. Como isso se relaciona com a realidade de empresas menores?

**R:** É verdade que o Alibaba é um caso extremo em termos de escala. Mas o princípio por trás do resultado se aplica: investimento em tecnologia web moderna (PWA) melhorou a experiência do usuário, especialmente em mobile e redes lentas, e isso se traduziu em mais conversões. O que muda em empresas menores é a magnitude do impacto e a viabilidade do investimento. Por isso a revisão bibliográfica inclui outros estudos sobre otimização mobile e performance que mostram resultados em contextos variados. E os experimentos na Achievece, que é uma plataforma de porte médio, vão justamente gerar dados em uma escala mais próxima da realidade de muitas empresas.

### P5: Na revisão bibliográfica, você identificou que o modelo LightGBM performou melhor que redes neurais profundas no sistema de recomendação da H&M. Por que isso aconteceu?

**R:** O trabalho do Nguyen et al. mostra que o LightGBM teve MAP@50 de 0,06 contra 0,02 das redes neurais. Vários fatores podem explicar isso: primeiro, LightGBM é muito eficiente com dados tabulares e features engenheiradas, que é o caso típico de sistemas de recomendação (histórico de compras, categorias de produtos, comportamento do usuário). Segundo, redes neurais profundas geralmente precisam de volumes maiores de dados e mais tempo de treinamento para convergir. Terceiro, a interpretabilidade do LightGBM é maior, o que facilita debugging e otimização do modelo. O resultado sugere que nem sempre a abordagem mais sofisticada é a melhor - há um trade-off entre complexidade e eficácia que precisa ser avaliado em cada contexto.

### P6: Você mencionou "estratégias de retenção" em modelos de assinatura. Pode explicar melhor o que testou e por quê?

**R:** Em modelos de assinatura, churn é o grande vilão - cada cliente que cancela é receita recorrente perdida. As estratégias que estou testando incluem: ofertas de desconto quando o usuário inicia o processo de cancelamento (por exemplo, "fique por mais 3 meses com 30% de desconto"), downsell (oferecer um plano mais barato ao invés de cancelar completamente), pausa temporária da assinatura. Também estou testando upsell durante o checkout - oferecer o plano anual com desconto quando o usuário vai comprar o mensal. A ideia é medir o impacto de cada estratégia em métricas como taxa de churn, lifetime value do cliente, e receita incremental. A literatura tem pouco sobre implementação técnica dessas estratégias, então os experimentos vão contribuir com evidências práticas.

## Perguntas sobre Lacunas e Contribuições

### P7: Quais você considera as principais lacunas que identificou na literatura?

**R:** Identifiquei cinco lacunas principais:

Primeira: falta de frameworks integrados que conectem arquitetura, UX e IA de forma holística. Os estudos tendem a focar em uma dimensão isoladamente.

Segunda: faltam estudos de longo prazo sobre ROI real de implementações de IA. Sabemos que sistemas de recomendação funcionam tecnicamente, mas qual o retorno financeiro ao longo de 1, 2 anos considerando custos de desenvolvimento e manutenção?

Terceira: falta de benchmarks padronizados para comparar diferentes abordagens arquiteturais. O Zhao et al. apontaram isso - é difícil replicar estudos e fazer comparações objetivas.

Quarta: falta explorar melhor técnicas de ML/AI para otimização integrada e automática de plataformas.

Quinta, e talvez a mais relevante para o meu trabalho: falta estabelecer relações quantitativas claras entre decisões técnicas específicas e receita em diferentes contextos de negócio. Por exemplo, qual o impacto de melhorar tempo de resposta de APIs de 200ms para 100ms? Como isso varia por segmento, por dispositivo?

### P8: Qual você espera que seja a principal contribuição do seu trabalho?

**R:** Espero que a principal contribuição seja conectar o técnico com o financeiro de forma prática e baseada em evidências. Muitos trabalhos acadêmicos focam em aspectos técnicos isolados. Muitos conteúdos de mercado são superficiais ou anedóticos. Este trabalho busca o meio termo: rigor metodológico da academia com aplicabilidade prática para quem desenvolve e-commerce. O framework de análise integrada e os dados quantitativos dos experimentos devem ajudar engenheiros e gestores a priorizar onde investir recursos técnicos para maximizar impacto na receita. E a identificação clara das lacunas deve orientar pesquisas futuras.

## Perguntas Técnicas Específicas

### P9: Você vai usar alguma arquitetura específica na Achievece ou vai testar diferentes arquiteturas?

**R:** A Achievece já está em produção, então não vou fazer mudanças arquiteturais drásticas durante o TFG. A arquitetura atual é uma aplicação web moderna com frontend em React, backend em Node.js, banco de dados PostgreSQL. O foco dos experimentos não é comparar arquiteturas diferentes (monolítico vs microsserviços), mas sim otimizações dentro da arquitetura existente: performance de frontend (Core Web Vitals), otimização de queries no backend, estratégias de caching. A revisão bibliográfica complementa isso analisando estudos que fazem comparações arquiteturais em outros contextos.

### P10: Como você vai medir Core Web Vitals e garantir que as melhorias são causadas pelas suas otimizações e não por outros fatores?

**R:** Vou usar ferramentas padrão do ecossistema web: Google Lighthouse para análises de performance, Web Vitals library para coleta de métricas reais dos usuários (RUM - Real User Monitoring), Chrome User Experience Report para dados agregados. A metodologia de A/B testing resolve o problema de causalidade: ao dividir o tráfego aleatoriamente entre a versão atual (controle) e a versão otimizada (teste), com ambas rodando simultaneamente, fatores externos afetam os dois grupos igualmente. Diferenças significativas na taxa de conversão podem ser atribuídas às otimizações de performance. Vou também controlar por variáveis como tipo de dispositivo, horário do dia, fonte de tráfego na análise.

### P11: E sobre privacidade e LGPD? Como você vai lidar com a coleta de dados dos usuários para os experimentos?

**R:** Boa pergunta. A coleta de dados segue as práticas de privacidade e conformidade com LGPD. Os dados são anonimizados, não identificam usuários individuais. Uso de cookies e tracking está declarado na política de privacidade da plataforma, com consentimento dos usuários. Para o TFG, vou trabalhar com dados agregados e estatísticas - não preciso de informações pessoais identificáveis. Métricas como taxa de conversão, receita média, tempo de sessão são calculadas de forma agregada. Se houver necessidade de análises mais detalhadas de jornada do usuário, vou usar identificadores anonimizados e garantir que não seja possível reidentificar indivíduos.

## Perguntas sobre Cronograma e Viabilidade

### P12: O cronograma parece ambicioso. Como você vai garantir que consegue concluir tudo no prazo?

**R:** O cronograma é apertado mas viável. Alguns fatores ajudam: primeiro, a revisão bibliográfica já está bem avançada. Segundo, a plataforma Achievece já existe em produção, não preciso desenvolver do zero - só implementar variações para os experimentos. Terceiro, tenho experiência prática com as tecnologias envolvidas, o que reduz a curva de aprendizado. Quarto, os experimentos vão rodar em paralelo quando possível. O risco maior é se algum experimento não atingir significância estatística no tempo esperado - para isso, tenho experimentos de backup mais simples que podem ser executados mais rapidamente. E a própria revisão bibliográfica já gera contribuições mesmo que os experimentos demorem mais.

### P13: Você está fazendo o TFG sozinho. Não seria melhor ter uma equipe ou parceria com alguma empresa?

**R:** É individual sim, que é o formato do TFG. Mas tenho algumas vantagens: já trabalho com a plataforma Achievece, então tenho acesso aos dados e estrutura para fazer os experimentos. Tenho suporte da orientadora para direcionamento metodológico e acadêmico. E a decisão de fazer experimentos em uma plataforma que eu mesmo desenvolvo, embora limite a escala, dá agilidade - não dependo de aprovações de terceiros para implementar mudanças e rodar testes. Claro que uma parceria com uma empresa maior poderia trazer dados em escala diferente, mas também traria complexidades de acordos, confidencialidade, tempos de aprovação que poderiam inviabilizar o TFG no prazo.

---

**Observação:** Estas perguntas cobrem os principais aspectos do trabalho e antecipam questionamentos que orientadores e bancas costumam fazer. As respostas são diretas, reconhecem limitações quando existem, e demonstram compreensão profunda tanto da teoria quanto da prática.
