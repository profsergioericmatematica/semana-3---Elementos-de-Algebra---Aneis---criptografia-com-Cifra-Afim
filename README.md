# 🔐 Cifra Afim – Criptografia e Decifragem

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

**Projeto interativo educacional para a disciplina Elementos de Álgebra – UNIVESP (Semana 3).** Implementação de uma ferramenta web focada em acessibilidade que permite cifrar e decifrar mensagens usando a **Cifra Afim** sobre o anel ℤ₂₆ (inteiros módulo 26).

🔗 **Acesse a demonstração ao vivo:** [Link para o GitHub Pages](https://seu-usuario.github.io/nome-do-repositorio) *(substitua pelo link real)*

## ✨ Funcionalidades

* **Validação Algorítmica:** Escolha interativa das chaves **α** (multiplicador) e **β** (deslocamento), com validação automática garantindo que α seja coprimo com 26.
* **Processamento de Texto:** Cifragem de qualquer texto preservando espaços, pontuação, números e acentos (apenas letras A-Z/a-z são transformadas através da álgebra modular).
* **Matemática Aplicada:** Decifragem automática utilizando o inverso modular de α.
* **Feedback em Tempo Real:** Exemplo dinâmico integrado. A frase *"O site usa o sistema de criptografia simples chamado 'cifra afim' e utiliza a estrutura de anel de ℤ₂₆."* é cifrada instantaneamente ao mudar as chaves, demonstrando visualmente que apenas a chave correta recupera o texto original.
* **Client-Side Puro:** Interface responsiva, amigável e com processamento 100% no navegador, sem envio de dados para servidores externos.

## 🧠 Como funciona a Cifra Afim?

Cada letra do alfabeto latino é convertida em um número x (A=0, B=1, ..., Z=25). A cifragem é dada pela seguinte função:

> E(x) = (α · x + β) mod 26

A decifragem exige o inverso modular α⁻¹, que existe **se, e somente se**, o máximo divisor comum for 1 (mdc(α, 26) = 1). A função de decodificação é:

> D(y) = α⁻¹ · (y - β) mod 26

No projeto, a chave **α** é validada e escolhida estritamente entre os valores **coprimos com 26**:  
`{1, 3, 5, 7, 9, 11, 15, 17, 19, 21, 23, 25}`.  
A chave **β** pode assumir qualquer valor inteiro no intervalo de 0 a 25.

## 🚀 Como usar localmente

1. [Clique aqui:](https://profsergioericmatematica.github.io/semana-3---Elementos-de-Algebra---Aneis---criptografia-com-Cifra-Afim/)
 

Selecione os valores de α e β, digite ou cole um texto na área indicada e clique em Cifrar ou Decifrar.

🛠️ Tecnologias Utilizadas
HTML5

CSS3 (Flexbox e arquitetura Mobile-First para adaptação em qualquer tela)

JavaScript (Vanilla/ES6) para a lógica matemática e manipulação do DOM

Nenhuma dependência ou biblioteca externa foi utilizada

📝 Licença
Este projeto está sob a licença MIT. Consulte o arquivo LICENSE para mais informações.

👨‍🏫 Autor
Sergio Eric

📷 Instagram: @prof.sergio.eric.matematica

🔗 GitHub: seu-usuario (substitua pelo seu link)

Projeto desenvolvido como atividade prática e ferramenta de apoio didático para a disciplina Elementos de Álgebra – UNIVESP.
