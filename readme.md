# 🕷️ Spider-Man | Multiversos

# preview

<img scr="./assets/images/capa.png">

Landing Page interativa inspirada no universo do **Homem-Aranha**, destacando os três atores que deram vida ao herói nos cinemas: **Tobey Maguire, Andrew Garfield e Tom Holland**.  

O projeto combina **HTML, CSS e JavaScript** para criar um carrossel 3D dinâmico, efeitos de hover imersivos e páginas individuais personalizadas para cada versão do herói.

---

## 🚀 Tecnologias utilizadas

- **HTML5** → estrutura semântica da página  
- **CSS3** → animações, responsividade e componentes reutilizáveis  
- **JavaScript (ES6)** → lógica de interatividade e manipulação do DOM  

---

## 🎨 Funcionalidades

✔️ **Carrossel 3D rotativo** controlado por botões.  
✔️ **Efeito hover** que altera:
- Destaque do card selecionado  
- Imagem de fundo da página (dinâmica via `body.id`)  
✔️ **Sistema de navegação** com menu fixo.  
✔️ **Controle de estado ativo** nos botões do carrossel.  
✔️ Estrutura modular de CSS (global + componentes).  
✔️ **Páginas dedicadas** para cada Homem-Aranha com vídeos de fundo, descrições e links interativos.  

---

## 📜 Detalhes Técnicos

### Interatividade nos Cards
- Cada card recebe a classe `.s-card--hovered` ao passar o mouse.  
- O `body` ganha dinamicamente um `id` correspondente ao card ativo (`spider-man-01-hovered`, etc.), permitindo **alteração de background via CSS**.  
- Ao sair do card, o efeito é removido.

### Carrossel Dinâmico
- O carrossel gira em **3D** usando `transform: rotateY()`.  
- Cada botão corresponde a um card e aplica uma rotação de `-120° * índice do botão`.  
- O botão ativo recebe a classe `.s-controller__button--active`.  

### Estrutura do Código
- `handleMouseEnter / handleMouseLeave` → gerenciam hover nos cards  
- `addEventListenersToCards` → adiciona eventos a todos os cards automaticamente  
- `selectCarouselItem` → controla rotação do carrossel e atualização do botão ativo  

---


