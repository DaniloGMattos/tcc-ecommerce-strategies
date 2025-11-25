# BANNER/PÔSTER - Workshop TFG
## Engenharia de Computação - UNIFEI

**ESPECIFICAÇÕES TÉCNICAS:**
- Dimensões: 84,1 cm (largura) × 118,9 cm (altura) - Formato A0
- Título: Verdana, 66pt, CAIXA ALTA, Negrito, Centralizado
- Autores/Instituição: Verdana, 32pt, Negrito, Centralizado
- Títulos de Seções: Verdana, 44pt
- Texto Corpo: Arial, 28pt mínimo, Justificado, Parágrafo simples

---

# CONTEÚDO DO BANNER

---

## CABEÇALHO (Centralizado, no meio do pôster)

**[VERDANA, 66, NEGRITO, CAIXA ALTA, CENTRALIZADO]**

CENÁRIO ATUAL DO DESENVOLVIMENTO DE PLATAFORMAS DE E-COMMERCE: ESTRATÉGIAS TÉCNICAS E IMPACTO NA RECEITA DAS EMPRESAS

---

**[VERDANA, 32, NEGRITO, CENTRALIZADO]**

MATTOS, Danilo Godofredo de

**[VERDANA, 32, NEGRITO, CAIXA ALTA, CENTRALIZADO]**

UNIVERSIDADE FEDERAL DE ITAJUBÁ - UNIFEI

ENGENHARIA DE COMPUTAÇÃO

Orientadora: Profa. Bárbara Pimenta Caetano

---

## CORPO DO PÔSTER

### INTRODUÇÃO
**[VERDANA, 44]**

O comércio eletrônico apresenta crescimento acelerado, com vendas globais projetadas em US$ 6,56 trilhões em 2025 e expectativa de US$ 8,09 trilhões até 2028. Este crescimento impõe desafios técnicos relacionados a desempenho, escalabilidade, experiência do usuário e conversão de vendas.

Decisões técnicas no desenvolvimento de plataformas de e-commerce impactam diretamente o sucesso e a receita das empresas. Desde escolhas arquiteturais até implementações de interface, inteligência artificial e otimizações de performance, cada decisão possui implicações mensuráveis nos resultados financeiros.

A diversificação dos modelos de monetização, incluindo pagamento único e assinaturas recorrentes, impõe desafios relacionados à maximização de receita recorrente, aumento do valor do tempo de vida do cliente e redução de taxa de cancelamento. Estratégias técnicas de vendas de produtos superiores, ofertas de retenção e personalização por perfil de assinante representam oportunidades relevantes, mas permanecem pouco exploradas na literatura.

---

### OBJETIVOS
**[VERDANA, 44]**

**Objetivo Geral:**

Analisar o cenário atual do desenvolvimento de plataformas de e-commerce, identificando e caracterizando as principais estratégias técnicas empregadas e avaliando seu impacto na receita e no sucesso das empresas.

**Objetivos Específicos:**

1. **Mapear as estratégias arquiteturais:** Identificar abordagens arquiteturais (monolíticas, microsserviços, orientada a eventos) e analisar as compensações em custo, complexidade e performance.

2. **Analisar estratégias de experiência do usuário:** Examinar técnicas de otimização (mobile, Progressive Web Apps, performance) e seu impacto nas conversões.

3. **Avaliar o papel da inteligência artificial:** Investigar aplicação de IA e machine learning em recomendação, personalização e geração de conteúdo.

4. **Correlacionar decisões técnicas com receita:** Identificar relação mensurável entre decisões técnicas específicas e métricas de negócio.

5. **Identificar lacunas e oportunidades:** Mapear lacunas no conhecimento atual e oportunidades de pesquisa futura.

---

### METODOLOGIA
**[VERDANA, 44]**

**Revisão Bibliográfica Sistemática:**

Análise de 12 trabalhos recentes (2023-2025) organizados em quatro eixos temáticos:

• **Arquitetura e Performance:** Comparação entre arquiteturas monolíticas e distribuídas, mapeamento de 109 estudos sobre análise de desempenho arquitetural.

• **Experiência do Usuário:** Impacto de design UX/UI nas conversões, otimização mobile, SEO e performance, casos de sucesso com Progressive Web Apps.

• **Inteligência Artificial:** IA generativa aplicada a e-commerce, sistemas de recomendação com machine learning.

• **Métricas e Conversão:** Análise da jornada do usuário, taxas de conversão por fonte de tráfego, identificação de gargalos no checkout.

**Experimentos Práticos - Plataforma Achievece:**

Estudo de observação em plataforma de e-commerce de cursos online com 30 mil visitantes mensais e receita diária de US$ 2.500. Implementação de experimentos controlados:

• **Testes A/B de Interface:** Redesign de checkout, otimização de formulários, variações mobile, elementos de urgência.

• **Progressive Web App:** Implementação de cache, funcionalidade offline, notificações push.

• **Otimizações de Performance:** Lazy loading, CDN, otimização de queries, análise de Core Web Vitals.

• **Personalização e Recomendação:** Sistema de filtragem colaborativa e análise comportamental.

• **Estratégias de Retenção em Assinaturas:** Upsell no checkout, ofertas de retenção no cancelamento, análise de impacto em MRR e churn.

**Análise Estatística:**

Testes de significância com 95% de confiança, cálculo de tamanho de amostra, análise de séries temporais.

---

### RESULTADOS E ANÁLISE DOS RESULTADOS
**[VERDANA, 44]**

**Resultados da Revisão Bibliográfica:**

**1. Impacto Mensurável de Decisões Técnicas:**
O caso do Alibaba.com demonstra impacto direto: implementação de Progressive Web App resultou em aumento de 76% nas conversões. Este resultado evidencia que escolhas arquiteturais e de tecnologia têm implicações financeiras diretas e mensuráveis.

**2. Contexto Determina Escolhas Arquiteturais:**
Sistemas centralizados oferecem melhores tempos de resposta em cenários de baixa complexidade, enquanto arquiteturas distribuídas performam melhor com alta demanda. Não existe solução arquitetural universalmente superior.

**3. Experiência do Usuário como Fator Crítico:**
Estudos demonstram correlação positiva significativa entre usabilidade, otimização mobile e satisfação do cliente, com impacto mensurável nas taxas de conversão.

**4. IA e Machine Learning - Eficácia Técnica Comprovada:**
Sistema de recomendação H&M: LightGBM apresentou desempenho superior (MAP@50 = 0,06) comparado a redes neurais profundas (MAP@50 = 0,02), demonstrando que nem sempre abordagens mais complexas são mais eficazes.

**5. Lacunas Identificadas:**
• Falta de frameworks integrados que combinem arquitetura, UX e IA
• Carência de estudos de longo prazo sobre ROI de implementações de IA
• Ausência de benchmarks padronizados para comparação arquitetural
• Falta de estudos sistemáticos sobre estratégias de monetização via assinatura

**Resultados Esperados dos Experimentos (Em Andamento):**

• Framework de análise integrada conectando dimensões técnicas com métricas de negócio
• Evidências quantitativas do impacto de otimizações de performance em conversão
• Análise comparativa de efetividade de diferentes fontes de tráfego
• Avaliação de estratégias de upsell e retenção em modelos de assinatura
• Métricas de impacto: taxa de conversão, receita por visitante, MRR, CLTV, taxa de churn

---

### CONCLUSÕES
**[VERDANA, 44]**

O cenário atual do desenvolvimento de plataformas de e-commerce é caracterizado pela convergência de múltiplas estratégias técnicas que impactam diretamente a receita e o sucesso empresarial:

**Principais Constatações:**

1. **Decisões técnicas têm impacto financeiro mensurável:** Casos documentados demonstram que escolhas arquiteturais e tecnológicas podem resultar em aumentos de conversão superiores a 70%.

2. **Não existe solução técnica universal:** A escolha adequada depende do contexto específico do negócio, volume de transações, padrões de crescimento e recursos disponíveis.

3. **UX/UI é fator crítico de conversão:** Especialmente em dispositivos móveis, a experiência do usuário tem correlação direta com taxas de conversão e receita.

4. **IA oferece oportunidades com desafios:** Sistemas de recomendação demonstram eficácia técnica, mas apresentam desafios de aceitação, privacidade e custos de implementação.

5. **Otimização é processo contínuo:** Análise baseada em dados e experimentação sistemática são essenciais para incremento contínuo de receita.

**Contribuições do Trabalho:**

Este estudo contribui para a academia com evidências empíricas sobre o impacto de decisões técnicas, e para a prática oferecendo orientação baseada em dados para desenvolvimento de plataformas de e-commerce.

A identificação de lacunas na literatura, especialmente sobre estratégias de monetização via assinatura e relação quantitativa entre decisões técnicas e receita, orienta pesquisas futuras nesta área em constante evolução.

---

### REFERÊNCIAS
**[VERDANA, 44]**

SHOPIFY. Relatório de vendas globais de e-commerce. 2025.

UBUR, S. D. Reviewing the Scope and Impact of Implementing a Modernised IT Event-Driven Architecture from Traditional Architecture. arXiv:2303.12082, 2023.

ZHAO, Y. et al. A Systematic Mapping Study on Architectural Approaches to Software Performance Analysis. arXiv:2410.17372, 2024.

STAMKOU, C. et al. User Experience and Perceptions of AI-Generated E-Commerce Content. Data, v. 10, n. 6, p. 89, 2025.

NGUYEN, D. et al. A personalized product recommendation model in e-commerce based on retrieval strategy. Journal of Open Innovation, v. 10, n. 2, p. 100303, 2024.

MURALIDHAR, A.; LAKKANNA, Y. From Clicks to Conversions: Analysis of Traffic Sources in E-Commerce. arXiv:2403.16115, 2024.

ALIBABA. Case Study: Progressive Web App Implementation. web.dev, 2024.

The Role of UX/UI in E-Commerce Conversions. ResearchGate, 2025. DOI: 10.5281/zenodo.14866833.

The Impact of Website Usability and Mobile Optimization on Customer Satisfaction in Indonesia. ResearchGate, 2025. DOI: 10.58812/esiscs.v2i01.324.

Artificial Intelligence in E-Commerce and Digital Marketing: A Systematic Review. ResearchGate, 2025. DOI: 10.9734/ajrcos/2025/v18i3601.

---

### AGRADECIMENTOS E FINANCIAMENTOS
**[VERDANA, 44]**

Agradeço à Profa. Bárbara Pimenta Caetano pela orientação e suporte acadêmico ao longo do desenvolvimento deste trabalho. Agradeço também à Universidade Federal de Itajubá (UNIFEI) pela infraestrutura e oportunidade de realização deste Trabalho Final de Graduação.

---

**OBSERVAÇÕES PARA MONTAGEM DO PÔSTER:**

1. O QR-Code institucional deve ser mantido (será fornecido pela organização do evento)
2. Pode-se inserir gráficos e tabelas nas seções de Metodologia e Resultados
3. As cores e layout devem seguir o padrão institucional da UNIFEI
4. O pôster será impresso em formato A0 (84,1 × 118,9 cm)
5. Usar cordão ou fio de nylon para pendurar
6. O autor deve permanecer junto ao pôster por 90 minutos durante a apresentação
