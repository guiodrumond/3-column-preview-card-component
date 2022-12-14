# Frontend Mentor - 3-column preview card component solution

Esta é a minha solução para o desafio proposto pelo site Frontend Mentor. A proposta era fazer um card com três colunas, com uma pequena imagem, título, texto descritivo e um botão interativo. Cada coluna com uma cor diferente. O componente deveria ser responsivo para o formato mobile.

## Desafios do exercício

Cada coluna possui três cores diferentes. Me propus a não criar diferentes classes no HTML para cada coluna, mas usar o CSS para mudar o estilo das colunas de acordo com sua ordem usando pseudo-classes.

Também era preciso tornar responsivo mudando o formato do elemento para telas mobile.

## Screenshot

![image](https://user-images.githubusercontent.com/87048670/207597277-354b1ddb-4e58-4bb1-bc9c-e656f0aab72d.png)


## Links

- URL da solução: https://www.frontendmentor.io/solutions/3column-preview-card-component-Hbo_uS9U1W
- Site URL: https://3-column-preview-card-component-gilt-eight.vercel.app/

## Processo

### Usei no desafio

- HTML 5
- CSS
  - Flexbox
  - Pseudo seletores
- Google Fonts
  - Big Shoulders 
  - Lexend Deca

### Principais aprendizados

Controlar a estilização da página usando a ordem dos componentes é tranquilo quando usamos pseudo seletores de ordem. Abaixo o código que usei:

```css
main .col:nth-child(2) {
    background-color: hsl(184, 100%, 22%);
}

main .col:nth-child(2)>button {
    color: hsl(184, 100%, 22%);
}
```
Assim consiguimos controlar o estilo de cada elemento segundo a sua ordem no código. No segundo caso eu especifiquei um tipo de elemento combinado com a ordem de aparecimento da seu pai. Ou seja, defini a cor do botão dentro do segundo elemento com a classe .col.

