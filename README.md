# 🍷 Vinheria Agnello – Check-Point 03 (Flexbox & Transformações)

## 📖 Descrição

Página web única inspirada na **Vinheria Agnello**, uma loja de vinhos fictícia. O objetivo do projeto é praticar a construção de layouts com **Flexbox** e criar efeitos interativos com **pseudo-classes** e **transformações CSS**.

A página tem menu fixo, seção de destaque, cards de vinhos, uma seção "Sobre", um formulário de newsletter e rodapé, todos organizados com Flexbox e responsivos para celular.

## 🛠️ Recursos aplicados

### Flexbox
| Elemento | Propriedades usadas |
|---|---|
| Cabeçalho (`.cabecalho`) | `display: flex`, `justify-content: space-between`, `align-items: center`, `flex-wrap` |
| Menu (`.menu ul`) | `display: flex`, `gap` |
| Destaque (`.destaque`) | `flex-direction: column`, centralização com `justify-content` e `align-items` |
| Cards (`.cards`, `.card`) | `flex-wrap: wrap`, `flex: 1 1 240px`, `flex-grow`, `align-self`, `margin-top: auto` |
| Sobre (`.sobre`, `.diferenciais`) | Layout em linha que vira coluna, `flex-basis` |
| Newsletter (`.form-newsletter`) | Campo e botão lado a lado com `flex-wrap` |
| Rodapé (`.rodape`, `.redes`) | `justify-content: space-between`, ícones centralizados |

### Pseudo-classes
- `:hover`: links do menu, botões, cards, itens da lista "Sobre" e ícones das redes sociais (mudança de cor, sombra e borda)
- `:focus` / `:focus-visible`: botões, links e campo de e-mail (borda dourada e sombra)
- `:active`: botão principal "afunda" ao ser clicado
- `:nth-child(even)`: cor de borda alternada na lista de diferenciais
- `:invalid` + `:not(:placeholder-shown)`: borda vermelha quando o e-mail digitado é inválido

### Transformações
- `scale()`: botão principal e campo de e-mail em `:focus`
- `translateY()`: links do menu e cards "sobem" no hover
- `translateY()` + `scale()`: card flutua e aumenta
- `rotate()` + `scale()`: emoji do card e botão "Comprar"
- `rotate(360deg)`: ícones das redes sociais giram
- `translateX()`: itens da lista de diferenciais deslizam

Todas as transformações usam `transition` para a animação ficar suave.

## 📁 Estrutura

```
checkpoint03-flexbox/
│
├── index.html
├── README.md
└── css/
    └── flex-style.css
```

## 👤 Autor

**Tiago Santos**

## 🔗 Links

- **Repositório no GitHub:** https://github.com/Tiagos0uzadv/checkpoint03-flexbox
- **Site no GitHub Pages:** https://tiagos0uzadv.github.io/checkpoint03-flexbox/
