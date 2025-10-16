# 📸 Especificação Funcional — PhotoGram  
**Versão:** 1.0  
**Sistema:** PhotoGram  
**Propósito:** Aplicação web para criação e compartilhamento de fotos e postagens entre usuários.  
**Autor:** Diego Saltori  
**Evento:** Bug Hunt — PhotoGram  

---

## 📝 Sobre o PhotoGram

O **PhotoGram** é uma aplicação web desenvolvida para permitir que usuários criem, visualizem e compartilhem postagens com fotos, de forma simples e interativa.  
O sistema possui funcionalidades de registro, login, criação, edição e exclusão de postagens, além de visualização em formato de feed e interação por meio de comentários.  

A funcionalidade de **criação de postagens** conta ainda com **integração de Inteligência Artificial (IA)**, permitindo sugerir melhorias automáticas no texto da descrição, aprimorando a clareza e o estilo das postagens de forma dinâmica.

Durante o evento **Bug Hunt**, esta aplicação é utilizada como ambiente de testes controlado, contendo falhas intencionais de implementação e interpretação de requisitos.  
Essas falhas foram inseridas para simular situações reais de desenvolvimento, incentivando a análise crítica de histórias de usuário, validações e comportamento da interface.

---

## 📂 Estrutura das Histórias de Usuário

As histórias de usuário estão organizadas por tela e localizadas na pasta:


Dentro dela, cada arquivo descreve os requisitos e critérios de aceite específicos de cada parte da aplicação:

| Tela | Arquivo | Descrição |
|------|----------|------------|
| Registro | `historiaUsuario/telaRegistro.md` | Criação de novas contas de usuário |
| Login | `historiaUsuario/telaLogin.md` | Acesso de usuários cadastrados |
| Dashboard | `historiaUsuario/telaDashboard.md` | Exibição e gerenciamento de postagens |
| Postagem | `historiaUsuario/telaPostagem.md` | Detalhamento e comentários das postagens |
| Add | `historiaUsuario/telaNovaPostagem.md` | Criação de nova postagem |
| Edit | `historiaUsuario/telaEdicao.md` | Edição e atualização de postagens existentes |

Cada história foi escrita com base em cenários reais de uso, mas com **pontos ambíguos ou incompletos**, que refletem decisões de design ou comunicação que podem gerar bugs funcionais, visuais ou de segurança.

---

## 🎯 Objetivo do Documento

Este repositório serve como **documentação base** do PhotoGram, descrevendo as funcionalidades esperadas da aplicação de forma simplificada.  
Ele foi elaborado para apoiar o evento **Bug Hunt — PhotoGram**, oferecendo contexto funcional para os testes exploratórios e para a análise das falhas encontradas.

---

**© 2025 — Diego Saltori**  
*Caçando bugs desde o início dos tempos 🐞*
