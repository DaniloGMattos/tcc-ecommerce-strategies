# Como Compilar no Overleaf

## Instruções para Compilação

### 1. Upload dos Arquivos

Faça upload dos seguintes arquivos para o Overleaf:

- `slide.tex` (arquivo principal)
- `zafu.sty` (pacote de estilo da ECO)
- `src/white-logo.png` (logo da UNIFEI)
- `src/cover.png` (imagem de capa)

### 2. Configurar o Compilador

**IMPORTANTE:** Configure o compilador para **pdfLaTeX** (conforme LEIAM-ME.txt)

No Overleaf:
1. Clique no ícone de **Menu** (canto superior esquerdo)
2. Em **Compiler**, selecione **pdfLaTeX**
3. Clique em **Recompile**

### 3. Estrutura dos 6 Slides

1. **Slide de Título** - Capa com título, autor, orientadora
2. **Contexto e Problema** - Crescimento do e-commerce, problema de pesquisa
3. **Motivação e Objetivos** - Motivação + 1 objetivo geral + 5 específicos
4. **Exemplo Prático** - Plataforma Achievece, estrutura de testes A/B
5. **Cronograma e Considerações Finais** - Cronograma 2025, expectativas
6. **Revisão Bibliográfica** - 12 artigos em 4 eixos temáticos
7. **Resultados Esperados** - Framework, evidências, lacunas
8. **Q&A** - Página de perguntas (gerada automaticamente)

### 4. Personalização

Se desejar fazer ajustes:

- **Cores:** Já configuradas no template ECO (azul UNIFEI)
- **Fonte:** Serif (padrão do template)
- **Logo:** Aparece automaticamente no canto superior esquerdo de cada slide
- **Rodapé:** Sem rodapé (footlinecolor vazio por padrão)

### 5. Comandos Úteis do Template

- `\maketitle` - Gera slide de título com imagem de fundo
- `\QApage` - Gera página de Q&A automaticamente
- `\textbf{}` - Negrito
- `\vspace{}` - Espaçamento vertical
- `\centering` - Centralizar texto

### 6. Compilação

Após configurar o compilador como pdfLaTeX, simplesmente clique em **Recompile** ou pressione **Ctrl+S** (Windows/Linux) ou **Cmd+S** (Mac) para compilar automaticamente.

O PDF será gerado automaticamente e aparecerá no painel direito do Overleaf.

### 7. Download

Para baixar o PDF final:
1. Clique no ícone de **Download PDF** (ao lado do botão Recompile)
2. Ou vá em **Menu** > **Download** > **PDF**

---

## Estrutura de Pastas no Overleaf

```
/
├── slide.tex (arquivo principal)
├── zafu.sty (pacote de estilo)
└── src/
    ├── white-logo.png
    └── cover.png
```

---

## Observações

- A apresentação está configurada para formato **16:9** (widescreen)
- Total de 8 páginas: 1 título + 6 conteúdo + 1 Q&A
- Todos os dados estão verificados e alinhados com a literatura
- O template usa o estilo oficial da ECO/UNIFEI
- **Nota:** Utiliza-se "exemplo prático" e "testes" ao invés de "experimentos"
