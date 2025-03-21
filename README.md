# 📌 Projeto: Aluguel de Games
![image](https://github.com/user-attachments/assets/dd60a8f5-e5e1-437f-abd7-9ed71689d88d)

## 📖 Descrição
Este repositório contém um projeto desenvolvido para praticar a manipulação de elementos HTML com JavaScript. O projeto é uma aplicação de aluguel de boardgames chamada **AluGames**, onde os usuários podem alugar e devolver jogos, alterando dinamicamente o status dos itens na interface.

## 🚀 Tecnologias Utilizadas
- HTML5
- CSS3
- JavaScript (DOM Manipulation)

## 🎯 Conceitos Aplicados
- Análise da estrutura HTML para planejamento da funcionalidade
- Recuperação de elementos com `document.querySelector()` e `document.getElementById()`
- Armazenamento de elementos em variáveis JavaScript
- Manipulação de classes CSS com `classList.add()`, `classList.remove()` e `classList.contains()`
- Modificação do texto de elementos com `textContent`
- Uso de condições (`if/else`) para alteração de status

## 📂 Estrutura do Projeto
```
📁 aluguel-de-games
│-- 📄 index.html
│-- 📄 style.css
│-- 📄 script.js
```

## ⚙️ Como Executar
1. Clone este repositório:
   ```bash
   git clone https://github.com/laisepcosta/aluguel-de-games.git
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd aluguel-de-games
   ```
3. Abra o arquivo `index.html` em um navegador web.

## 🔄 Lógica da Funcionalidade
A página exibe uma lista de boardgames com botões para **alugar** e **devolver** jogos. A interação ocorre via JavaScript da seguinte forma:

1. O botão "Alugar" chama a função `alterarStatus(id)`, onde `id` representa o jogo correspondente.
2. Dentro da função:
   - O elemento do jogo é recuperado usando `document.getElementById()`.
   - A presença da classe `dashboard__item__img--rented` é verificada com `classList.contains()` para saber se o jogo está alugado.
   - Se o jogo **não** estiver alugado:
     - A classe `dashboard__item__img--rented` é adicionada para indicar o aluguel.
     - O texto do botão muda para "Devolver".
     - A classe `dashboard__item__button--return` é adicionada ao botão.
   - Se o jogo **já** estiver alugado:
     - A classe `dashboard__item__img--rented` é removida para indicar a devolução.
     - O texto do botão muda para "Alugar".
     - A classe `dashboard__item__button--return` é removida.

## 📌 Funcionalidade Implementada
O projeto permite alterar dinamicamente o status de um jogo, modificando classes CSS e o texto de elementos com base em interações do usuário.

## 🛠 Melhorias Futuras
- Implementação de eventos adicionais para interatividade
- Aprimoramento do design com animações CSS
- Uso de armazenamento local para persistência de status

