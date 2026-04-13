# 🔐 Cifra Afim – Criptografia e Decifragem

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

**Projeto interativo para a disciplina Elementos de Álgebra – UNIVESP (Semana 3).**  
Implementação de uma ferramenta web que permite cifrar e decifrar mensagens usando a **cifra afim** sobre o anel ℤ₂₆ (inteiros módulo 26).

🔗 **Acesse a demonstração ao vivo:** [[https://seu-usuario.github.io/nome-do-repositorio](https://profsergioericmatematica.github.io/semana-3---Elementos-de-Algebra---Aneis---criptografia-com-Cifra-Afim/)]([https://seu-usuario.github.io/nome-do-repositorio](https://profsergioericmatematica.github.io/semana-3---Elementos-de-Algebra---Aneis---criptografia-com-Cifra-Afim/))  
*(substitua pelo link real do GitHub Pages)*

## ✨ Funcionalidades

- Escolha interativa das chaves **α** (multiplicador) e **β** (deslocamento), com validação automática (α deve ser coprimo com 26).
- Cifragem de qualquer texto (preserva espaços, pontuação, números e acentos – apenas letras A-Z/a-z são transformadas).
- Decifragem automática usando o inverso modular de α.
- Exemplo dinâmico: a frase *“O site usa o sistema de criptografia simples chamado “cifra afim” e utiliza a estrutura de anel de ℤ₂₆.”* é cifrada instantaneamente ao mudar as chaves, demonstrando que apenas a chave correta recupera o texto original.
- Interface responsiva, amigável e 100% client‑side (não envia dados para nenhum servidor).

## 🧠 Como funciona a Cifra Afim?

Cada letra é convertida em um número x (A=0, B=1, ..., Z=25). A cifragem é dada por:
