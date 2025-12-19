# Figuras do Relatório de Estágio

Este diretório deve conter as seguintes figuras:

## arquitetura.png
Diagrama de arquitetura do sistema Simple Juris mostrando:
- Frontend (Vue.js)
- Backend (Django + API REST)
- Banco de Dados (PostgreSQL)
- Sistema de filas (Redis + Celery)
- Workers de Scraping
- Conexão com TJSP

## fluxo.png
Fluxograma do funcionamento da plataforma:
1. Advogado se cadastra
2. Robô valida credenciais no TJSP
3. Scraping busca todos os processos
4. Advogado visualiza processos na plataforma
5. Sistema atualiza diariamente e notifica por e-mail

---

Para compilar o documento sem as figuras, comente as linhas \includegraphics no main.tex.
