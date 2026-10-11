# Contador Numérico

Um contador numérico simples, feito com HTML, CSS e JavaScript puro. Permite aumentar, diminuir e zerar um valor com apenas um clique.

**Demo online:** https://manzatomari.github.io/contador_numerico/

## Funcionalidades

- **Incrementar**: soma 1 ao valor atual
- **Decrementar**: subtrai 1 do valor atual (o contador aceita valores negativos)
- **Resetar**: volta o contador para 0
- Layout responsivo: o cartão ocupa 90% da largura da tela, com máximo de 400px
- Efeito de *hover* nos botões (leve elevação e escurecimento)

## Tecnologias

- HTML5
- CSS3 (Flexbox)
- JavaScript (vanilla, sem dependências)
- GitHub Pages (hospedagem)

## Como usar

### Online

Acesse a [página do projeto](https://manzatomari.github.io/contador_numerico/) e use os botões.

### Localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/ManzatoMari/contador_numerico.git
   ```
2. Entre na pasta do projeto:
   ```bash
   cd contador_numerico
   ```
3. Abra o arquivo `index.html` no navegador.

Não é necessário instalar nada nem rodar um servidor.

## Estrutura do projeto

```
contador_numerico/
├── index.html    # Estrutura da página
├── style.css     # Estilos
└── app.js        # Lógica do contador
```

## Como funciona

O estado do contador fica na variável `count`, que começa em `0`. O `app.js` seleciona todos os botões com a classe `.btn` e adiciona um evento de clique a cada um. Ao clicar, o código verifica a classe do botão:

| Classe         | Ação              |
| -------------- | ----------------- |
| `.incrementar` | `count++`         |
| `.decrementar` | `count--`         |
| `.resetar`     | `count = 0`       |

Depois disso, o novo valor é exibido no elemento `#value` por meio de `textContent`.

## Possíveis melhorias

- Impedir valores negativos (opcional)
- Definir um passo personalizado (ex.: +5, +10)
- Salvar o valor com `localStorage`
- Adicionar atalhos de teclado
- Tema claro/escuro
