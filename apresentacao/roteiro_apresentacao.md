# Roteiro de Apresentação - TFG (Defesa Final)
## Cenário Atual do Desenvolvimento de Plataformas de E-commerce: Estratégias Técnicas e Impacto na Receita das Empresas

**Aluno:** Danilo Godofredo de Mattos (Mat. 2018009986)
**Orientadora:** Profa. Bárbara Pimenta Caetano
**Curso:** Engenharia de Computação - UNIFEI
**Duração estimada:** 20 minutos

---

## Estrutura da Apresentação (20 slides)

| Parte | Slides | Tempo |
|-------|--------|-------|
| Introdução e Contexto | 1-2 | 3 min |
| Revisão Bibliográfica | 3-7 | 5 min |
| Metodologia | 8-9 | 2,5 min |
| Resultados | 10-16 | 6,5 min |
| Limitações e Conclusão | 17-20 | 3 min |
| **Total** | **20** | **~20 min** |

---

## SLIDE 1: Contexto e Problema (1,5 minutos)

**[Abertura]**
Bom dia/boa tarde a todos. Meu nome é Danilo Mattos, e este é meu Trabalho Final de Graduação, orientado pela Professora Bárbara Caetano. O título é "Cenário Atual do Desenvolvimento de Plataformas de E-commerce: Estratégias Técnicas e Impacto na Receita das Empresas".

**[Contextualizar o mercado]**
O e-commerce é um mercado em crescimento acelerado. Segundo dados da Shopify, as vendas globais devem passar de 6,56 trilhões de dólares em 2025 para mais de 8 trilhões até 2028. Esse crescimento traz desafios técnicos importantes: como garantir performance com mais usuários? Como melhorar a experiência para converter mais vendas?

**[O problema identificado]**
Na prática, o que se observa é que a informação técnica está dispersa na literatura. Existem estudos sobre arquitetura de software, outros sobre otimização de interface, outros sobre sistemas de recomendação. Mas falta uma visão que integre essas dimensões e, principalmente, que conecte decisões técnicas com resultados financeiros reais.

**[Exemplo concreto]**
Para ilustrar: o Alibaba.com, ao implementar Progressive Web App, teve aumento de 76% nas conversões. Isso mostra que decisões técnicas podem ter impacto direto e significativo na receita.

---

## SLIDE 2: Motivação e Objetivos (1,5 minutos)

**[Motivação]**
A motivação para este trabalho veio da minha experiência profissional. Trabalho há mais de dois anos como responsável técnico de uma plataforma de e-commerce, e frequentemente me deparo com decisões técnicas cujo impacto financeiro não é claro. Migrar de arquitetura? Investir em performance? Implementar personalização? São decisões que demandam recursos, mas cujo retorno é difícil de quantificar.

**[Objetivo geral]**
O objetivo geral é analisar o cenário atual do desenvolvimento de plataformas de e-commerce, identificando estratégias técnicas e discutindo seu potencial impacto na receita.

**[Objetivos específicos]**
Os objetivos específicos são cinco. Destaco o quarto: discutir relações entre decisões técnicas e receita - este é o objetivo central do trabalho.

---

## SLIDE 3: Revisão Bibliográfica - Visão Geral (1 minuto)

**[Estrutura da revisão]**
A revisão bibliográfica analisou 12 trabalhos recentes, de 2023 a 2025, organizados em quatro eixos temáticos:

1. **Arquitetura de Software** - monolítico vs microsserviços, event-driven, trade-offs de escalabilidade
2. **UX/UI e Performance** - Core Web Vitals, PWA, otimização mobile
3. **Inteligência Artificial** - sistemas de recomendação, IA generativa, personalização
4. **Métricas de Conversão** - jornada do usuário, gargalos no checkout

Vou detalhar cada eixo nos próximos slides.

---

## SLIDE 4: Revisão - Arquitetura de Software (1 minuto)

**[Ubur 2023]**
O trabalho de Ubur, de 2023, comparou arquitetura event-driven com monolítica. A conclusão principal é que não existe uma solução universal. Aplicações monolíticas têm menos overhead e respondem melhor em baixa carga. Microsserviços escalam melhor quando a demanda aumenta.

**[Zhao et al. 2024]**
O mapeamento sistemático de Zhao e colaboradores analisou 109 estudos sobre performance arquitetural. Uma das conclusões importantes é a falta de padronização em benchmarks, o que dificulta comparações entre abordagens.

**[Implicação]**
A implicação prática é que a decisão arquitetural deve considerar contexto: tamanho da equipe, escala esperada e recursos disponíveis. Não existe "bala de prata".

---

## SLIDE 5: Revisão - UX/UI e Performance (1 minuto)

**[Nawir 2024]**
O estudo de Nawir, de 2024, é particularmente relevante. Encontrou que 70% da variância nas taxas de conversão pode ser explicada por fatores de usabilidade. Design responsivo e navegação intuitiva são críticos.

**[Bansal 2024]**
Bansal, também de 2024, mostrou a relação entre performance e conversão: queda de 7% nas conversões para cada segundo adicional de carregamento. Core Web Vitals também afetam o ranqueamento no Google.

**[Caso Alibaba]**
O caso mais emblemático é do Alibaba.com, que ao implementar Progressive Web App teve aumento de 76% nas conversões, especialmente em experiência mobile.

---

## SLIDE 6: Revisão - Inteligência Artificial (1 minuto)

**[Stamkou et al. 2025]**
Stamkou e colaboradores, em 2025, analisaram o uso de IA generativa em e-commerce - ChatGPT para atendimento e descrições de produto, DALL-E para geração de imagens. O potencial de personalização em massa é alto.

**[Nguyen et al. 2024 - H&M]**
Um resultado interessante vem do sistema de recomendação da H&M analisado por Nguyen. Comparando LightGBM com Deep Neural Networks, o modelo mais simples teve melhor desempenho: MAP@50 de 0,06 contra 0,02 da rede neural. Isso mostra que modelos simples podem superar complexos dependendo do contexto.

**[Achado-chave]**
O achado-chave é que IA tem alto potencial, mas dados quantitativos sobre impacto direto em receita ainda são escassos na literatura.

---

## SLIDE 7: Síntese da Revisão Bibliográfica (1 minuto)

**[Principais achados]**
Resumindo os principais achados:
- Arquitetura: trade-offs claros, sem solução universal
- UX/UI: evidências fortes de impacto em conversão
- IA: promessa alta, evidências quantitativas limitadas
- Performance: relação direta com métricas de negócio

**[Lacunas identificadas]**
As lacunas identificadas são importantes para situar este trabalho:
- Faltam frameworks integrados que analisem múltiplas dimensões
- Poucos estudos apresentam dados financeiros reais
- Ausência de benchmarks padronizados
- A relação quantitativa entre decisão técnica e receita é pouco explorada

---

## SLIDE 8: Aplicação Prática - Achievece (1,5 minutos)

**[Apresentar a plataforma]**
Além da revisão bibliográfica, o trabalho apresenta uma aplicação prática na plataforma Achievece - achievece.com. É um e-commerce de cursos online especializado em educação continuada para médicos nos Estados Unidos.

**[Números]**
A plataforma tem cerca de 30 mil visitantes mensais, mais de 700 cursos, e receita diária na ordem de 2.500 dólares. Trabalha com modelo híbrido: produtos de pagamento único e assinaturas.

**[Justificativa]**
A escolha se justifica por três razões: tenho acesso completo aos dados e à infraestrutura, o volume de tráfego permite análises significativas, e o modelo de negócio permite observar diferentes estratégias.

**[Período]**
O período de análise foi de aproximadamente um ano de implementações.

---

## SLIDE 9: Estratégias Implementadas (1 minuto)

**[Listar estratégias]**
As estratégias implementadas foram organizadas em quatro grupos:

1. **Arquitetura**: Migração de WordPress para Next.js com arquitetura serverless na Vercel
2. **UX/UI**: Reorganização da interface para destacar produtos por assinatura, e otimização de Core Web Vitals
3. **SEO**: Implementação de dados estruturados JSON-LD para Organização, Produto, FAQ e Artigo. Também criamos mais de 100 páginas personalizadas por estado e profissão
4. **Retenção**: Ofertas de retenção no fluxo de cancelamento e estratégia de upsell pós-compra

**[Ferramentas]**
Para coleta de dados, utilizamos Google Analytics 4, Vercel Speed Insights e Google Search Console.

---

## SLIDE 10: Resultado - Reorganização da Interface (1 minuto)

**[Mostrar imagens]**
Aqui temos a comparação visual. À esquerda, a interface anterior, onde produtos de pagamento único apareciam em destaque. À direita, a nova interface, com os planos de assinatura posicionados no topo, com comparação visual clara entre opções.

**[Mudanças]**
As mudanças incluíram: hierarquia visual favorecendo assinaturas, proposta de valor mais clara, credenciais de acreditação em destaque, e personalização por estado e profissão do usuário.

**[Resultado]**
Os resultados observados foram: aumento de 74% no valor médio do pedido de assinaturas e crescimento de 105% na participação de novas vendas dessa categoria.

---

## SLIDE 11: Resultado - Performance (1 minuto)

**[Mostrar métricas]**
Na questão de performance, a imagem mostra as métricas do Vercel Speed Insights, que mede a experiência real dos usuários.

**[Números]**
Atingimos score de 95, com LCP de 2,92 segundos, INP de 112ms, CLS de 0,07, FCP de 1,55 segundos e TTFB de 0,48 segundos. Todas dentro dos parâmetros considerados bons pelo Google.

**[Arquitetura]**
A arquitetura serverless também trouxe benefício importante: desde a migração, não houve indisponibilidade. A escalabilidade automática eliminou os problemas que existiam no WordPress quando havia picos de usuários.

---

## SLIDE 12: Resultado - SEO e Tráfego de IA (1 minuto)

**[Contexto]**
Uma estratégia interessante foi a otimização para plataformas de IA. Implementamos dados estruturados JSON-LD pensando em como sistemas como ChatGPT interpretam conteúdo.

**[Mostrar gráficos]**
Os gráficos mostram o tráfego vindo de chatgpt.com. Em julho de 2025, antes da implementação completa, tivemos 54 usuários. Em agosto, após as otimizações, foram 109 usuários.

**[Resultado]**
Um aumento de 102%.

**[Ressalva]**
É importante ressalvar: o crescimento da adoção do ChatGPT como ferramenta de busca também pode ter contribuído para esse aumento. Não foi possível isolar completamente o efeito das otimizações.

---

## SLIDE 13: Resultado - Ofertas de Retenção (1 minuto)

**[Mostrar imagem]**
Esta é a estratégia com atribuição mais clara. A imagem mostra o modal apresentado quando um assinante inicia o processo de cancelamento.

**[Explicar estratégia]**
A oferta permite "pular" a próxima cobrança, mantendo o acesso por mais um ciclo gratuitamente. A opção de prosseguir com o cancelamento permanece visível - não é uma estratégia de dark pattern.

**[Resultado]**
Os dados de três meses mostram redução de 30% na intenção de cancelamento. Ou seja, de cada 10 usuários que iniciam o cancelamento, 3 aceitam a oferta e permanecem. Isso tem impacto direto no MRR e no lifetime value dos clientes.

---

## SLIDE 14: Resultado - Upsell (0,5 minutos)

**[Mostrar imagem]**
A estratégia de upsell é apresentada após a compra de um produto avulso. A página usa elementos de urgência - contador regressivo - e destaca o desconto oferecido.

**[Status]**
Esta funcionalidade foi implementada recentemente e ainda não acumulou dados suficientes para análise. Está em observação.

---

## SLIDE 15: Síntese dos Resultados (1 minuto)

**[Mostrar tabela]**
Esta tabela resume a conexão entre a literatura e as observações práticas:

- Migração serverless, baseada nos trade-offs arquiteturais da literatura, resultou em zero indisponibilidade
- Reorganização UX, respaldada pelo dado de 70% de variância em conversões, coincidiu com aumento de 74% no AOV
- Performance, conectada ao dado de -7% por segundo, atingiu score de 95
- SEO para IA, com aumento de 102% no tráfego
- Ofertas de retenção, com redução de 30% nos cancelamentos

**[Destaque]**
O destaque é a inversão no padrão de vendas: produtos por assinatura passaram de categoria secundária para principal fonte de novas vendas.

---

## SLIDE 16: Impacto por Categoria (1 minuto)

**[Mostrar tabela]**
Esta tabela detalha o impacto por categoria de produto.

**[Explicar números]**
Assinaturas: maior crescimento, com aumento de 74% no AOV e 105% na participação de novas vendas.
Avulsos: queda de 23% no AOV e 28% na participação - esperado, já que o objetivo era direcionar usuários para assinaturas.
Planos também tiveram crescimento significativo: 63% no AOV.

**[Interpretação]**
A inversão nos padrões de venda reflete o efeito combinado das estratégias. Não é possível isolar a contribuição individual de cada uma, mas o conjunto de mudanças claramente influenciou as decisões de compra.

---

## SLIDE 17: Limitações do Trabalho (1 minuto)

**[Ser honesto]**
É importante ser honesto sobre as limitações do trabalho.

**[Listar limitações]**
Primeiro, não foi possível aplicar testes A/B. Questões operacionais da empresa impediram a divisão de tráfego para grupos de controle.

Segundo, as estratégias foram implementadas em períodos próximos, o que dificulta a atribuição de resultados a ações específicas.

Terceiro, analisei apenas uma plataforma, limitando a generalização.

Quarto, dados históricos do WordPress foram perdidos, impedindo comparação direta.

**[Implicação]**
A implicação é que os resultados são correlações, não causalidade comprovada. O trabalho apresenta os dados como observações, não como evidências definitivas.

---

## SLIDE 18: Trabalhos Futuros (1 minuto)

**[Direções]**
Para trabalhos futuros, identifico algumas direções importantes:

- Estudos com testes A/B controlados para isolar o impacto de estratégias específicas
- Análises longitudinais que capturem efeitos de longo prazo
- Comparações entre diferentes segmentos de e-commerce
- Criação de benchmarks padronizados

**[Recomendação]**
Para empresas que queiram fazer estudos similares, recomendo: implementar infraestrutura de testes desde o início, alocar recursos específicos para análise de impacto, separar períodos de implementação, e preservar dados históricos.

---

## SLIDE 19: Considerações Finais (1 minuto)

**[Contribuições]**
As contribuições do trabalho são:
- Revisão bibliográfica de 12 trabalhos em 4 eixos temáticos
- Aplicação prática em plataforma real de e-commerce
- Discussão honesta sobre dificuldades de atribuição
- Identificação de lacunas para pesquisa futura

**[Mensagem principal]**
A mensagem principal é que a relação entre decisões técnicas e receita é real, mas complexa de mensurar. A literatura oferece indícios, a prática confirma potencial, mas estabelecer causalidade isolada continua sendo um desafio.

**[Encerramento]**
Obrigado pela atenção. Estou à disposição para perguntas.

---

## SLIDE 20: Perguntas

*[Aguardar perguntas da banca]*

---

# DICAS PARA A DEFESA

## Postura Geral
- **Humildade acadêmica**: reconhecer limitações sem se desculpar excessivamente
- **Não inventar dados**: se não souber algo, diga "não tenho dados para responder isso"
- **Defender o valor do trabalho**: limitações não invalidam contribuições
- **Linguagem precisa**: "coincidiu com" em vez de "causou", "observamos" em vez de "provamos"
- **Conectar com a literatura**: sempre que possível, referenciar os artigos revisados

## Frases Úteis
- "Essa é uma limitação reconhecida no trabalho..."
- "Os dados sugerem correlação, mas não permitem estabelecer causalidade isolada..."
- "O trabalho de [autor] indica que..."
- "Não tenho dados para afirmar isso com certeza, mas..."
- "Para trabalhos futuros, seria importante..."

## Controle de Tempo
- Se perceber que está atrasado: pule detalhes nos slides de revisão bibliográfica
- Se perceber que está adiantado: explore mais os slides de resultados com imagens
- Reserve os últimos 30 segundos para agradecer e convidar para perguntas

---

**Documento de perguntas e respostas completo disponível em:** `perguntas_respostas.md`
