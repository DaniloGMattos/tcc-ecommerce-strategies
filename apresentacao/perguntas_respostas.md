# Perguntas e Respostas Esperadas - Defesa TFG

## Cenário Atual do Desenvolvimento de Plataformas de E-commerce: Estratégias Técnicas e Impacto na Receita das Empresas

**Aluno:** Danilo Godofredo de Mattos
**Orientadora:** Profa. Bárbara Pimenta Caetano

---

## 1. Perguntas sobre Metodologia

### P1: Por que você não conseguiu fazer testes A/B? Isso não compromete os resultados?

**Resposta:** A impossibilidade de fazer testes A/B foi uma limitação operacional real. A empresa estava em funcionamento, com metas de receita, e dividir tráfego para grupos de controle por períodos longos não foi aprovado pela liderança. Isso de fato compromete a capacidade de estabelecer causalidade - por isso o trabalho é honesto em dizer que os dados sugerem correlação, não causalidade. No entanto, as observações ainda têm valor: mostram que o conjunto de estratégias coincidiu com melhorias nas métricas. Para estudos futuros, sugiro que a infraestrutura de testes A/B seja implementada desde o início do projeto, não como adaptação posterior.

---

### P2: Como você garante que os resultados não foram causados por fatores externos como sazonalidade ou campanhas de marketing?

**Resposta:** Não garanto completamente, e essa é uma limitação reconhecida no trabalho. O período de análise foi de aproximadamente um ano, o que pode não capturar todas as variações sazonais. Fatores como campanhas de marketing, mudanças na concorrência e variações macroeconômicas podem ter influenciado. Por isso, os resultados são apresentados como observações, não como evidências definitivas. A estratégia de ofertas de retenção é a que tem atribuição mais clara, porque afeta um momento específico - o usuário que vai cancelar - e podemos medir diretamente quantos aceitaram a oferta.

---

### P3: A amostra de uma única plataforma não limita muito a generalização?

**Resposta:** Sim, limita. A Achievece tem características específicas: é um e-commerce de cursos online, no segmento de educação médica, no mercado americano. Os resultados podem não se aplicar a outros segmentos, tamanhos ou públicos. No entanto, muitos princípios - como a importância de performance, a relação entre UX e conversão, a efetividade de ofertas de retenção - têm respaldo na literatura para outros contextos. O trabalho contribui com um caso detalhado que pode ser comparado com estudos futuros em outros segmentos.

---

### P4: Por que você escolheu Next.js para a migração? Não existiam outras opções?

**Resposta:** Existiam várias opções. A escolha de Next.js foi baseada em alguns fatores: primeiro, é um framework React com suporte nativo a renderização server-side e geração estática, o que é importante para SEO. Segundo, a integração com Vercel oferece arquitetura serverless sem necessidade de gerenciar infraestrutura. Terceiro, a equipe já tinha familiaridade com React. Não foi uma decisão baseada em comparação rigorosa com outras alternativas - foi uma decisão pragmática considerando contexto, recursos e conhecimento disponível.

---

## 2. Perguntas sobre Resultados

### P5: O aumento de 74% no AOV de assinaturas é muito expressivo. Você tem certeza de que é real?

**Resposta:** Os dados vêm do Google Analytics e dos sistemas internos de pagamento, então são dados reais de transações. O que não posso afirmar com certeza é que esse aumento foi causado exclusivamente pela reorganização da interface. Outras mudanças aconteceram no mesmo período: melhorias de performance, ajustes na comunicação textual, otimizações de SEO. O aumento é real, mas a atribuição é incerta. É possível que parte do aumento viesse de tendências já existentes ou de fatores externos. Por isso o trabalho usa linguagem cuidadosa: "coincidiu com", não "causou".

---

### P6: O que significa "redução de 30% na intenção de cancelamento"?

**Resposta:** Quando um assinante inicia o processo de cancelamento, apresentamos uma oferta - por exemplo, pular a próxima cobrança. Dos usuários que chegam nessa tela, 30% aceitam a oferta e não cancelam naquele momento. Esses 30% representam assinantes retidos que, sem a oferta, teriam cancelado. Claro, alguns podem cancelar depois, mas a estratégia dá uma chance de reter o cliente. Essa foi a estratégia com atribuição mais clara porque podemos medir diretamente: de X usuários que iniciaram cancelamento, Y aceitaram a oferta.

---

### P7: O aumento de 102% no tráfego de plataformas de IA não pode ser simplesmente porque mais pessoas estão usando ChatGPT?

**Resposta:** Pode sim, e essa é uma limitação que reconheço no trabalho. O crescimento da adoção de plataformas de IA como ferramenta de busca certamente contribuiu para o aumento, independentemente das otimizações que fizemos. Não foi possível isolar quanto veio das melhorias de SEO e quanto veio do crescimento natural do canal. O que posso dizer é que implementamos dados estruturados JSON-LD especificamente pensando em como sistemas de IA interpretam conteúdo, e houve um aumento no período seguinte. Mas correlação não é causalidade.

---

### P8: Por que a personalização foi feita manualmente e não com IA?

**Resposta:** Foi uma decisão pragmática baseada nos recursos disponíveis. A empresa tem uma equipe dedicada à área de conteúdo que conhece bem o público - médicos em diferentes estados e especialidades. Implementar um sistema de recomendação baseado em IA exigiria investimento em desenvolvimento, dados de treinamento, e manutenção contínua. A abordagem manual, criando páginas específicas por estado e profissão, alcança objetivos similares com os recursos que já existiam. O desafio técnico foi arquitetar o sistema para gerar muitas páginas sem repetição de código.

---

## 3. Perguntas sobre a Revisão Bibliográfica

### P9: Por que apenas 12 artigos? Não seria pouco para uma revisão bibliográfica?

**Resposta:** A escolha foi por cobertura temática, não por quantidade. Priorizei artigos recentes (2023-2025) que representam o estado da arte em cada eixo: arquitetura, UX, IA e métricas. Alguns trabalhos, como o mapeamento sistemático de Zhao et al., já sintetizam dezenas de outros estudos - esse artigo sozinho analisou 109 trabalhos sobre análise de desempenho arquitetural. Também incluí estudos de caso documentados como o do Alibaba. Considero que os 12 trabalhos dão uma visão representativa do cenário atual. Não segui protocolo formal de revisão sistemática, o que reconheço como limitação.

---

### P10: Você encontrou estudos que contradigam suas conclusões?

**Resposta:** Não encontrei contradições diretas, mas encontrei nuances. Por exemplo, sobre arquitetura, os estudos mostram que microsserviços não são sempre melhores - em cargas baixas, monólitos podem ter melhor tempo de resposta. Sobre IA, alguns trabalhos apontam que sistemas de recomendação mais simples (como LightGBM) podem superar redes neurais profundas em certos contextos. A literatura não é homogênea, e isso reforça que não existem soluções universais - o contexto importa.

---

### P11: O que você considera a principal lacuna identificada na literatura?

**Resposta:** A principal lacuna é a falta de estudos que quantifiquem de forma rigorosa a relação entre decisões técnicas específicas e receita. Sabemos que performance importa, que UX importa, que personalização importa - mas quanto cada melhoria específica impacta em reais? Quanto vale reduzir 100ms no tempo de carregamento? Quanto vale implementar um sistema de recomendação? A literatura tem evidências fragmentadas, mas faltam estudos integrados com dados financeiros reais.

---

## 4. Perguntas sobre Contribuições e Trabalhos Futuros

### P12: Qual você considera a principal contribuição do seu trabalho?

**Resposta:** A principal contribuição é mostrar a complexidade real de analisar o impacto de decisões técnicas em métricas de negócio. Muitos trabalhos acadêmicos focam em aspectos técnicos isolados; muitos conteúdos de mercado são superficiais. Este trabalho combina revisão bibliográfica com aplicação prática honesta, que reconhece suas limitações. Não promete soluções mágicas - mostra que a relação existe, mas é difícil de isolar. Para desenvolvedores e gestores, espero que ofereça um panorama realista das estratégias disponíveis e suas complexidades.

---

### P13: Se você pudesse refazer o trabalho, o que faria diferente?

**Resposta:** Implementaria infraestrutura de testes A/B desde o início. Isso exigiria ter discutido com a liderança da empresa antes sobre a importância de ambientes controlados para pesquisa. Também tentaria preservar dados históricos da plataforma anterior para ter linha de base comparativa. E separaria mais claramente os períodos de implementação de cada estratégia, mesmo que isso atrasasse algumas entregas. O aprendizado principal é que rigor metodológico em empresas reais exige planejamento e comprometimento antecipado.

---

### P14: Você acha que os resultados justificam o investimento que foi feito nas mudanças?

**Resposta:** Do ponto de vista da empresa, sim. O aumento de 74% no AOV de assinaturas e 105% na participação de novas vendas dessa categoria representam impacto significativo em receita recorrente. A redução de 30% na intenção de cancelamento impacta diretamente o churn e o lifetime value. Mesmo sem poder atribuir cada resultado a uma estratégia específica, o conjunto de mudanças coincidiu com melhorias relevantes. Do ponto de vista acadêmico, não posso afirmar causalidade, mas posso dizer que as evidências são encorajadoras.

---

## 5. Perguntas Técnicas Específicas

### P15: O que são Core Web Vitals e por que são importantes?

**Resposta:** Core Web Vitals são métricas definidas pelo Google para medir a qualidade da experiência do usuário em páginas web. São três principais: LCP (Largest Contentful Paint) mede o tempo até o maior elemento visível carregar; FID/INP mede a responsividade a interações; CLS mede a estabilidade visual da página. São importantes porque o Google usa essas métricas como fator de ranqueamento, então afetam tanto a experiência do usuário quanto a visibilidade em buscas. Na Achievece, atingimos score de 95, com LCP de 2,92 segundos.

---

### P16: O que são dados estruturados JSON-LD e como ajudam no SEO?

**Resposta:** JSON-LD é um formato para marcar informações estruturadas no código da página. Por exemplo, posso informar aos mecanismos de busca que uma página é um produto, com preço X, avaliação Y, disponibilidade Z. Isso ajuda os algoritmos a entenderem o conteúdo da página sem precisar interpretar o texto. Para plataformas de IA como ChatGPT, que buscam informações para responder perguntas dos usuários, ter dados bem estruturados pode aumentar a chance de ser citado como fonte. Implementamos schemas de organização, produto, FAQ e artigo na Achievece.

---

### P17: Como funciona a arquitetura serverless que você implementou?

**Resposta:** Em arquitetura serverless, não gerenciamos servidores dedicados. O código é executado em funções que escalam automaticamente conforme a demanda. Na prática, usamos Next.js hospedado na Vercel, que provisiona recursos automaticamente. Quando há mais usuários, mais instâncias são criadas; quando o tráfego diminui, os recursos são liberados. Isso elimina problemas de indisponibilidade por sobrecarga que tínhamos no WordPress, onde um servidor dedicado tinha limite de capacidade.

---

### P18: Você considerou questões de privacidade e LGPD na coleta de dados?

**Resposta:** Sim. Os dados são coletados de forma agregada, sem identificação de usuários individuais. O uso de cookies e tracking está declarado na política de privacidade da plataforma, com consentimento dos usuários. Para o trabalho acadêmico, uso apenas métricas agregadas - taxa de conversão, receita média, tempo de sessão - que não permitem identificar pessoas. A plataforma atende principalmente usuários nos EUA, então também há conformidade com regulamentações americanas.

---

## 6. Perguntas Desafiadoras

### P19: Seu trabalho não é essencialmente um relatório de melhorias que você fez no seu emprego? Onde está a contribuição acadêmica?

**Resposta:** Entendo a preocupação. A contribuição acadêmica está em três pontos: primeiro, a revisão bibliográfica sistematiza conhecimento disperso sobre estratégias técnicas em e-commerce. Segundo, a aplicação prática oferece dados reais que podem ser comparados com outros estudos. Terceiro, e mais importante, a discussão honesta sobre as dificuldades de atribuição contribui para a metodologia de pesquisa nessa área. O trabalho mostra por que é difícil fazer estudos rigorosos em ambientes de produção e sugere caminhos para trabalhos futuros. Não é só um relatório de melhorias - é uma reflexão crítica sobre como analisar impacto de decisões técnicas.

---

### P20: Se você não pode provar causalidade, qual é o valor prático das suas conclusões?

**Resposta:** O valor prático está em mostrar que o conjunto de estratégias implementadas coincidiu com melhorias significativas nas métricas. Para um desenvolvedor ou gestor tomando decisões, saber que essas estratégias têm potencial - respaldado tanto pela literatura quanto por observações práticas - já é útil. Não posso dizer "faça X e terá Y% de aumento", mas posso dizer "a literatura indica que X importa, e na prática observamos melhorias quando implementamos X junto com outras mudanças". É uma orientação informada, não uma garantia.

---

### P21: Você menciona que a literatura tem "evidências fragmentadas". Isso não invalida suas próprias conclusões baseadas nessa literatura?

**Resposta:** Não invalida, mas contextualiza. A fragmentação significa que os estudos abordam dimensões isoladas - um fala de arquitetura, outro de UX, outro de IA. A contribuição deste trabalho é justamente tentar integrar essas dimensões e mostrar que elas se conectam na prática. As evidências individuais são sólidas dentro de seus escopos - o que falta é a visão integrada. Meu trabalho não resolve essa lacuna completamente, mas contribui com um passo nessa direção ao analisar múltiplas estratégias em uma mesma plataforma.

---

## Dicas para a Defesa

1. **Postura de humildade acadêmica**: Reconhecer limitações sem se desculpar excessivamente
2. **Não inventar dados**: Se não souber algo, diga "não tenho dados para responder isso"
3. **Defender o valor do trabalho**: Limitações não invalidam contribuições
4. **Usar linguagem precisa**: "coincidiu com" em vez de "causou", "observamos" em vez de "provamos"
5. **Conectar com a literatura**: Sempre que possível, referenciar os artigos revisados
