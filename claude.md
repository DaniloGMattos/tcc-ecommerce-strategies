# Projeto TCC/TFG - Revisão Bibliográfica

## Informações do Trabalho

**Título:** Cenário Atual do Desenvolvimento de Plataformas de E-commerce: Estratégias Técnicas e Impacto na Receita das Empresas

**Aluno:** Danilo Godofredo de Mattos (Mat. 2018009986)
**Orientadora:** Profa. Bárbara Pimenta Caetano
**Curso:** Engenharia de Computação - UNIFEI
**Modalidade:** TFG (Trabalho Final de Graduação) - Individual

## Objetivo Geral
Analisar o cenário atual do desenvolvimento de plataformas de e-commerce, identificando e caracterizando as principais estratégias técnicas empregadas e avaliando seu impacto na receita e no sucesso das empresas.

## Estrutura do Projeto

### Diretório pesquisa/
- `tcc_docs.bib`: 12 referências bibliográficas em formato BibTeX
- `arquivos/`: PDFs dos artigos científicos organizados por ID

### Diretório ECO_revisao_bibliografica_TFG/
- `main.tex`: Arquivo principal LaTeX (NÃO ALTERAR, apenas compilar com xelatex)
- `referencias.bib`: Arquivo de referências BibTeX (12 referências)
- `sections/`: Arquivos LaTeX editados com conteúdo completo:
  - `title.tex`: Capa com título, dados do aluno e orientadora ✅
  - `01-introducao.tex`: Introdução contextualizada ✅
  - `02-motivacao.tex`: Motivação alinhada ao título ✅
  - `03-revisao.tex`: **Revisão bibliográfica completa** ✅
  - `04-objetivos.tex`: Objetivos específicos definidos ✅
  - `05-materiais_e_metodos.tex`: A ser completado
  - `06-resultados.tex`: A ser completado
  - `07-cronograma.tex`: A ser completado

## Arquivo Principal para Visualização

**Para visualizar a revisão bibliográfica completa, compile o documento:**

```bash
cd ECO_revisao_bibliografica_TFG
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

**O PDF gerado será:** `ECO_revisao_bibliografica_TFG/main.pdf`

**Para editar diretamente a revisão bibliográfica:** `ECO_revisao_bibliografica_TFG/sections/03-revisao.tex`

## Objetivos Específicos do Trabalho

1. **Mapear as estratégias arquiteturais** - Identificar abordagens arquiteturais (monolíticas, microsserviços, event-driven) e analisar trade-offs
2. **Analisar estratégias de UX** - Examinar técnicas de otimização de experiência do usuário (mobile, PWA, performance)
3. **Avaliar o papel da IA** - Investigar aplicação de IA e ML (recomendação, personalização, conteúdo gerado)
4. **Correlacionar decisões técnicas com receita** - Identificar relação mensurável entre decisões técnicas e métricas de negócio
5. **Identificar lacunas e oportunidades** - Mapear lacunas no conhecimento e oportunidades de pesquisa

## Temas dos 12 Artigos Revisados

### 1. Arquitetura de Software e Performance
- Event-Driven Architecture vs Monolítica (Ubur, 2023)
- Mapeamento sistemático de análise de desempenho (Zhao et al., 2024)
- Servidores distribuídos para e-commerce

### 2. UX/UI e Experiência do Usuário
- Impacto do design UX/UI nas conversões
- Usabilidade mobile e satisfação do cliente (Indonésia)
- SEO e velocidade de carregamento
- **Caso Alibaba.com:** +76% conversões com PWA
- Coleção de estudos de caso PWA

### 3. Inteligência Artificial e Personalização
- IA generativa em e-commerce (Stamkou et al., 2025) - ChatGPT e DALL·E
- Revisão sistemática sobre IA em e-commerce e marketing digital
- Sistema de recomendação H&M (Nguyen et al., 2024)
  - LightGBM: MAP@50 = 0.06, MAR@50 = 0.03
  - Deep Neural Networks: MAP@50 = 0.02, MAR@50 = 0.01

### 4. Métricas de Conversão e Análise de Tráfego
- Análise da jornada do usuário (Muralidhar & Lakkanna, 2024)
- Taxas de conversão por fonte de tráfego
- Gargalos no processo de checkout
- Otimização mobile e compatibilidade entre navegadores

## Estrutura da Revisão Bibliográfica (sections/03-revisao.tex)

A revisão bibliográfica está organizada em 6 subsections:

1. **Arquiteturas de Software e Desempenho em E-commerce**
   - Comparação monolítico vs microsserviços (Ubur, 2023)
   - Mapeamento sistemático (Zhao et al., 2024)
   - Servidores distribuídos

2. **Experiência do Usuário e Otimizações de Interface**
   - UX/UI e conversões
   - Usabilidade mobile e otimização
   - SEO e performance
   - Caso Alibaba.com (+76% conversões)
   - Estudos PWA

3. **Inteligência Artificial e Personalização**
   - IA generativa (Stamkou et al., 2025)
   - Revisão sistemática IA em e-commerce
   - Sistema de recomendação H&M (Nguyen et al., 2024)

4. **Métricas de Conversão e Análise de Tráfego**
   - Jornada do usuário (Muralidhar & Lakkanna, 2024)
   - Gargalos e otimizações

5. **Síntese: Estratégias Técnicas e Impacto na Receita**
   - Decisões arquiteturais e escalabilidade
   - Experiência do usuário como fator crítico de conversão
   - Personalização via IA: oportunidades e desafios
   - Otimização de métricas como estratégia contínua

6. **Lacunas e Oportunidades de Pesquisa**
   - Frameworks integrados de análise
   - Estudos longitudinais sobre ROI de IA
   - Benchmarks padronizados para comparação arquitetural
   - Otimização integrada via ML/AI
   - Relação quantitativa entre decisões técnicas e receita

## Status do Projeto

- ✅ Estrutura do projeto analisada
- ✅ Referências BibTeX copiadas para referencias.bib (12 referências)
- ✅ PDFs verificados e legíveis
- ✅ **Capa (title.tex)** atualizada com título e dados do aluno/orientadora
- ✅ **Introdução (01-introducao.tex)** escrita e alinhada ao título
- ✅ **Motivação (02-motivacao.tex)** escrita com foco em impacto na receita
- ✅ **Revisão bibliográfica (03-revisao.tex)** completa com 12 artigos
- ✅ **Objetivos (04-objetivos.tex)** definidos (1 geral + 5 específicos)
- ✅ Arquivos auxiliares (.aux, .log, etc) removidos
- ⏳ Materiais e métodos (05-materiais_e_metodos.tex) - a completar
- ⏳ Resultados esperados (06-resultados.tex) - a completar
- ⏳ Cronograma (07-cronograma.tex) - a completar

## Próximos Passos

1. **Compilar o documento localmente:**
   ```bash
   cd /Users/danilomattos/work/tcc/ECO_revisao_bibliografica_TFG
   xelatex main.tex
   bibtex main
   xelatex main.tex
   xelatex main.tex
   ```

2. **Visualizar o PDF gerado** em `main.pdf` para revisar formatação e conteúdo

3. **Completar seções restantes:**
   - Materiais e métodos (metodologia da revisão bibliográfica)
   - Resultados esperados
   - Cronograma de execução

4. **Revisão final** seguindo normas ABNT

## Diretrizes de Escrita

### Tom e Estilo do Texto
O texto deve ser escrito com **tom de estudante universitário em TFG**, seguindo estas diretrizes:

1. **Humildade e realismo**: Evitar afirmações grandiosas ou promessas que um TFG não consegue cumprir
2. **Linguagem acadêmica simples**: Usar vocabulário técnico quando necessário, mas sem exageros
3. **Reconhecer limitações**: Sempre mencionar que o trabalho possui limitações e é uma contribuição modesta
4. **Evitar superlativos**: Não usar termos como "revolucionário", "inovador", "pioneiro" sem justificativa
5. **Citações adequadas**: Todo dado ou afirmação de terceiros deve ter citação no formato ABNT usando `\citeonline{}` ou `\cite{}`
6. **Verbos no condicional**: Preferir "pode influenciar", "tende a refletir" em vez de afirmações absolutas
7. **Naturalidade**: O texto deve parecer escrito por um estudante, não por IA - evitar estruturas muito padronizadas ou listas excessivas

### Formato de Citações (ABNT - abntex2)
- Citação no meio do texto: `\citeonline{chave}` → Autor (ano)
- Citação entre parênteses: `\cite{chave}` → (AUTOR, ano)
- Citação com página: `\citeonline[p. 10]{chave}` → Autor (ano, p. 10)

### Referências Disponíveis
As referências estão em `referencias_tcc.bib` com as seguintes chaves principais:
- `shopify_relatorio_2025` - Dados de vendas globais de e-commerce
- `ubur_reviewing_2023` - Arquitetura monolítica vs microsserviços
- `muralidhar_clicks_2024` - Jornada do usuário e conversões
- `nguyen_personalized_2024` - Sistemas de recomendação (H&M)
- `stamkou_user_2025` - IA generativa em e-commerce
- `zhao_systematic_2024` - Mapeamento sistemático de performance
- `noauthor_alibaba_nodate` - Case study Alibaba PWA (+76% conversões)

## Notas Importantes

- O documento está configurado para fonte Arial, conforme especificações da UNIFEI
- Margens: superior 1,5cm; inferior 2,5cm; esquerda e direita 2,0cm
- Espaçamento entre linhas: 1,5
- Títulos: Arial 12, negrito
- Corpo do texto: Arial 10, justificado
- Bibliografia no estilo IEEEtran (pode ser alterado para abntex2-alf se necessário)
