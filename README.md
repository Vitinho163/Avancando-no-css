# Avançando no CSS

## PROPRIEDADES FUNDAMENTAIS

Todo grid é composto de 2 principais grupos:
`container: o pai` e `itens: o(s) filhos`

---
### CONTAINER (pai)

- display: grid;
- grid-template;
  - grid-template-columns;
  - grid-template-rows;
  - grid-template-areas;
- gap;
  - row-gap;
  - column-gap;

---
### ITENS (filhos)

- grid-column;
  - grid-column-start;
  - grid-column-end;
- grid-row;
  - grid-row-start;
  - grid-row-end;
- grid-area;


---
### PROPRIEDADES DE ALINHAMENTO

Existem 9 propriedades FUNDAMENTAIS

**6 aplicadas em container**
`align-content`
`justify-content`
`place-content`

`align-items`
`justify-items`
`place-items`

**3 aplicadas em items**
`align-self`
`justify-self`
`place-self`

Então podemos separar em 3 grupos:
`align`, `justify`, `place`

E cada um deles irá observar ou o
- conteúdo do elemento `content`
- itens do elemento `items`
- o próprio elemento `self`
--- 

### PROPRIEDADES AUTO

- grid-auto-flow
- grid-auto-rows
- grid-auto-columns

# Grid ou Flex?

Qualquer um, pois você consegue chegar no mesmo lugar utilizando flex ou grid.

Tem layouts que você vai ver e vai olhar que é melhor grid e outras que você vai ver e vai falar que é melhor flex pela simplicidade.

Exemplo basico: 

![Exemplo com ul](https://imgur.com/lTwPSJW.png)

```css
#grid {
  display: grid;
  grid-auto-flow: column;
  justify-content: start;
  list-style: none;
  gap: 16px;
}

#flex {
  display: flex;
  list-style: none;
  gap: 16px;
}
```

Ambos chegam no mesmo lugar.