# Estrutura Modular da Monografia

A monografia foi reorganizada para usar uma estrutura modular, similar à revisão bibliográfica. Isso facilita a edição e manutenção do documento.

## Estrutura de Arquivos

```
/monografia/
├── monografia_tcc_danilo.tex          # Arquivo PRINCIPAL (configurações + estrutura)
├── monografia_tcc_danilo_OLD.tex      # Backup da versão anterior
├── referencias_tcc.bib                # Referências bibliográficas
│
├── sections/                          # Diretório com os capítulos
│   ├── 01_introducao.tex              # Capítulo 1 - Introdução ✅ COMPLETO
│   ├── 02_revisao_bibliografica.tex   # Capítulo 2 - Revisão Bibliográfica ⏳
│   ├── 03_metodologia.tex             # Capítulo 3 - Metodologia ⏳
│   ├── 04_analise_discussao.tex       # Capítulo 4 - Análise e Discussão ⏳
│   └── 05_conclusao.tex               # Capítulo 5 - Conclusão ⏳
│
├── SUMARIO_DETALHADO.md               # Planejamento completo da monografia
├── ESTRUTURA_MODULAR.md               # Este arquivo
└── README_MONOGRAFIA.md               # Instruções gerais
```

---

## Arquivo Principal (monografia_tcc_danilo.tex)

O arquivo principal agora está **muito mais limpo** e contém apenas:

### 1. Configurações e Preâmbulo
- Classe do documento (abntex2)
- Pacotes LaTeX
- Informações da capa (título, autor, orientadora)
- Configurações de formato

### 2. Elementos Pré-Textuais
- Capa e folha de rosto
- Dedicatória
- Agradecimentos
- Resumo (PT)
- Abstract (EN)
- Listas (figuras, tabelas, siglas)
- Sumário automático

### 3. Elementos Textuais (MODULAR)
```latex
\textual

% Capítulos incluídos via \input{}
\input{sections/01_introducao.tex}
\input{sections/02_revisao_bibliografica.tex}
\input{sections/03_metodologia.tex}
\input{sections/04_analise_discussao.tex}
\input{sections/05_conclusao.tex}
```

### 4. Elementos Pós-Textuais
- Referências bibliográficas
- Apêndices (comentados, prontos para uso)

---

## Vantagens da Estrutura Modular

### ✅ Organização
- Cada capítulo em arquivo separado
- Fácil localização de conteúdo
- Estrutura clara e hierárquica

### ✅ Manutenção
- Editar apenas o arquivo do capítulo necessário
- Menos risco de quebrar a formatação geral
- Arquivo principal permanece limpo

### ✅ Colaboração
- Múltiplas pessoas podem trabalhar em capítulos diferentes
- Controle de versão mais eficiente (Git)
- Revisões focadas por capítulo

### ✅ Compilação
- Compilar documento completo normalmente
- Mesmo processo de antes (pdflatex + bibtex)
- Compatível com Overleaf

---

## Como Editar

### Para editar um capítulo:

1. **Abra o arquivo correspondente** em `/sections/`:
   - Introdução: `01_introducao.tex`
   - Revisão Bibliográfica: `02_revisao_bibliografica.tex`
   - Metodologia: `03_metodologia.tex`
   - Análise: `04_analise_discussao.tex`
   - Conclusão: `05_conclusao.tex`

2. **Edite o conteúdo** normalmente com comandos LaTeX

3. **Compile o arquivo principal** (`monografia_tcc_danilo.tex`) para ver o resultado

### Comandos LaTeX nos arquivos de seção:

Cada arquivo de seção já contém:
```latex
% ----------------------------------------------------------------
% Título do Capítulo
% ----------------------------------------------------------------
\chapter{Nome do Capítulo}
\label{ch:label}

\section{Nome da Seção}
Conteúdo...

\subsection{Nome da Subseção}
Conteúdo...
```

**IMPORTANTE**: Não inclua preâmbulo, `\begin{document}` ou `\end{document}` nos arquivos de seção. Apenas o conteúdo do capítulo.

---

## Como Adicionar Novo Capítulo

Se precisar adicionar um novo capítulo:

1. **Crie um novo arquivo** em `sections/`:
   ```
   sections/06_novo_capitulo.tex
   ```

2. **Adicione o conteúdo** no novo arquivo:
   ```latex
   \chapter{Título do Novo Capítulo}
   \label{ch:novo}

   Conteúdo...
   ```

3. **Inclua no arquivo principal** (`monografia_tcc_danilo.tex`):
   ```latex
   \input{sections/01_introducao.tex}
   \input{sections/02_revisao_bibliografica.tex}
   \input{sections/03_metodologia.tex}
   \input{sections/04_analise_discussao.tex}
   \input{sections/05_conclusao.tex}
   \input{sections/06_novo_capitulo.tex}  % <-- ADICIONE AQUI
   ```

---

## Estrutura de Cada Capítulo

### Capítulo 1 - Introdução ✅
- Contexto e Relevância
- Motivação e Justificativa
- Objetivos (Geral + 5 Específicos)
- Escopo e Delimitações
- Estrutura do Trabalho

### Capítulo 2 - Revisão Bibliográfica ⏳
- Arquiteturas de Software e Desempenho
- Experiência do Usuário e Otimizações
- Inteligência Artificial e Personalização
- Métricas de Conversão e Análise de Tráfego
- Síntese e Lacunas

### Capítulo 3 - Metodologia ⏳
- Tipo de Pesquisa
- Revisão Bibliográfica Sistemática
- Framework de Análise
- Limitações Metodológicas

### Capítulo 4 - Análise e Discussão ⏳
- Panorama Geral
- Relação Arquitetura x Performance
- UX/UI e Conversões
- IA e ROI
- Síntese de Decisões Técnicas

### Capítulo 5 - Conclusão ⏳
- Principais Contribuições
- Respostas aos Objetivos
- Lacunas Identificadas
- Limitações do Estudo
- Trabalhos Futuros
- Considerações Finais

---

## Comparação: Antes vs. Depois

### ❌ Antes (Arquivo Único)
```
monografia_tcc_danilo.tex (600+ linhas)
- Configurações
- Elementos pré-textuais
- Capítulo 1 inline (60 linhas)
- Capítulo 2 inline (100 linhas)
- Capítulo 3 inline (80 linhas)
- Capítulo 4 inline (120 linhas)
- Capítulo 5 inline (90 linhas)
- Elementos pós-textuais
```

### ✅ Depois (Estrutura Modular)
```
monografia_tcc_danilo.tex (323 linhas - LIMPO!)
- Configurações
- Elementos pré-textuais
- \input{sections/01_introducao.tex}
- \input{sections/02_revisao_bibliografica.tex}
- \input{sections/03_metodologia.tex}
- \input{sections/04_analise_discussao.tex}
- \input{sections/05_conclusao.tex}
- Elementos pós-textuais

sections/
- 01_introducao.tex (62 linhas)
- 02_revisao_bibliografica.tex (estrutura pronta)
- 03_metodologia.tex (estrutura pronta)
- 04_analise_discussao.tex (estrutura pronta)
- 05_conclusao.tex (estrutura pronta)
```

---

## Compilação

O processo de compilação **não muda**:

```bash
cd /Users/danilomattos/work/tcc/monografia
pdflatex monografia_tcc_danilo.tex
bibtex monografia_tcc_danilo
pdflatex monografia_tcc_danilo.tex
pdflatex monografia_tcc_danilo.tex
```

O LaTeX automaticamente inclui o conteúdo dos arquivos `\input{}` durante a compilação.

---

## Status Atual

| Capítulo | Arquivo | Status | Conteúdo |
|----------|---------|--------|----------|
| 1 - Introdução | `01_introducao.tex` | ✅ Completo | 5 seções escritas |
| 2 - Revisão Bibliográfica | `02_revisao_bibliografica.tex` | ⏳ Estrutura | Subseções definidas |
| 3 - Metodologia | `03_metodologia.tex` | ⏳ Estrutura | Subseções definidas |
| 4 - Análise e Discussão | `04_analise_discussao.tex` | ⏳ Estrutura | Subseções definidas |
| 5 - Conclusão | `05_conclusao.tex` | ⏳ Estrutura | Subseções definidas |

---

## Próximos Passos

1. **Revisar Introdução** (01_introducao.tex)
2. **Desenvolver Revisão Bibliográfica** usando conteúdo de `/ECO_revisao_bibliografica_TFG/sections/03-revisao.tex`
3. **Escrever Metodologia**
4. **Desenvolver Análise e Discussão**
5. **Concluir com Conclusão**

---

**Estrutura organizada, limpa e pronta para desenvolvimento!** ✨
