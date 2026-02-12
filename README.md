# Documentação do Projeto: Slider de Imagens com Miniaturas

Este projeto consiste em um componente de interface de usuário (UI) para exibição de slides dinâmicos, utilizando HTML5 semântico e ganchos para CSS e JavaScript.

---

## 1. Estrutura do Cabeçalho (Header)
O topo da página é composto por uma barra de navegação simples:
* **Logo**: Identificado pela classe `.logo` (Lundev).
* **Menu**: Uma lista não ordenada (`ul`) contendo links para Home, Blog e Info.
* **Busca**: Um ícone de lupa renderizado via **SVG** para garantir nitidez em qualquer resolução.

---

## 2. Componente Slider
O slider é o elemento central da página e está dividido em três partes principais:

### A. Lista de Itens (`.list`)
Contém os slides principais. Cada `.item` possui:
* Uma imagem de fundo ou destaque.
* Um contêiner `.content` que sobrepõe informações como categoria, título e descrição (Lorem Ipsum).
* A classe `.active` indica qual slide está visível no momento.

### B. Controles de Navegação (`.arrows`)
Contém dois botões de direção:
* **id="prev"**: Para retornar ao slide anterior.
* **id="next"**: Para avançar para o próximo slide.

### C. Miniaturas (`.thumbnail`)
Uma linha de visualização rápida das imagens disponíveis. 
* Serve para dar contexto visual ao usuário sobre o que vem a seguir.
* Assim como na lista principal, a classe `.active` destaca a miniatura correspondente ao slide atual.

---

## 3. Integração de Arquivos
O HTML serve como o esqueleto do projeto, dependendo de recursos externos para funcionar plenamente:
* **style.css**: Responsável pelo posicionamento absoluto dos conteúdos, transições de animação e o layout responsivo.
* **app.js**: Gerencia a lógica de clique nos botões, a troca das classes `.active` e o ciclo automático dos slides.

---

## 4. Hierarquia de Conteúdo


A estrutura segue esta ordem de profundidade:
1. **Background**: Imagem do item ativo.
2. **Camada de Conteúdo**: Texto e botões sobre a imagem.
3. **Interface de Navegação**: Setas laterais e miniaturas posicionadas na parte inferior.

---

> **Nota de Implementação**: Para adicionar novos slides, basta replicar o bloco de código `<div class="item">` tanto na div `.list` quanto na div `.thumbnail`, garantindo que as imagens correspondam.
<img width="1808" height="889" alt="Image" src="https://github.com/user-attachments/assets/8c06ecc5-00b8-437a-a54b-4b88483dd365" />
