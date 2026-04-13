```markdown
# 🔐 Cifra Afim – Criptografia e Decifragem

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)

**Projeto interativo para a disciplina Elementos de Álgebra – UNIVESP (Semana 3).**  
Implementação de uma ferramenta web que permite cifrar e decifrar mensagens usando a **cifra afim** sobre o anel ℤ₂₆ (inteiros módulo 26).

🔗 **Acesse a demonstração ao vivo:** [https://seu-usuario.github.io/nome-do-repositorio](https://seu-usuario.github.io/nome-do-repositorio)  
*(substitua pelo link real do GitHub Pages)*

## ✨ Funcionalidades

- Escolha interativa das chaves **α** (multiplicador) e **β** (deslocamento), com validação automática (α deve ser coprimo com 26).
- Cifragem de qualquer texto (preserva espaços, pontuação, números e acentos – apenas letras A-Z/a-z são transformadas).
- Decifragem automática usando o inverso modular de α.
- Exemplo dinâmico: a frase *“O site usa o sistema de criptografia simples chamado “cifra afim” e utiliza a estrutura de anel de ℤ₂₆.”* é cifrada instantaneamente ao mudar as chaves, demonstrando que apenas a chave correta recupera o texto original.
- Interface responsiva, amigável e 100% client‑side (não envia dados para nenhum servidor).

## 🧠 Como funciona a Cifra Afim?

Cada letra é convertida em um número x (A=0, B=1, ..., Z=25). A cifragem é dada por:

```
E(x) = (α · x + β) mod 26
```

A decifragem exige o inverso modular α⁻¹ (que existe **se e somente se** mdc(α,26) = 1):

```
D(y) = α⁻¹ · (y - β) mod 26
```

No projeto, α é escolhido entre os valores **coprimos com 26**:  
`{1, 3, 5, 7, 9, 11, 15, 17, 19, 21, 23, 25}`.  
β pode ser qualquer inteiro de 0 a 25.

## 🚀 Como usar localmente

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   ```
2. Abra o arquivo `index.html` em qualquer navegador moderno.
3. Selecione α e β, digite ou cole um texto e clique em **Cifrar** ou **Decifrar**.

## 🛠️ Tecnologias utilizadas

- HTML5
- CSS3 (Flexbox, design responsivo)
- JavaScript (ES6)
- Nenhuma dependência externa – puro HTML/CSS/JS.

## 📝 Licença

Este projeto está sob a licença MIT. Consulte o arquivo [LICENSE](LICENSE) para mais informações.

## 👨‍🏫 Autor

**Sergio Eric**  
📷 Instagram: [@prof.sergio.eric.matematica](https://instagram.com/prof.sergio.eric.matematica)  
🔗 GitHub: [[seu-usuario](https://github.com/profsergioericmatematica)]([https://github.com/seu-usuario](https://github.com/profsergioericmatematica))

---

*Projeto desenvolvido como atividade prática da disciplina Elementos de Álgebra – UNIVESP.*
```
