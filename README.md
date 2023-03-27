![image description](https://storage.googleapis.com/dpw/app/uploads/2020/05/image.png)

# default-BEM-for-css
BEM, metodologia CSS / convenção de nomenclatura para deixar o código front end no padrão internacional.

## Referencias:
- [https://getbem.com/]
- [https://desenvolvimentoparaweb.com/css/bem/]

## Metodologia/Convenção BEM:
- Convenção de nome de classes e só...
- Modular, flexivel.

## Os 3 pilares do BEM:
- 1• Pilar: Bloco.
- 2• Pilar: Elemento.
- 3• Pilar: Modificador.

```sh
.block__element--modifier{}
.block__element{}
.block--modifier{}
```

## Bem - Bloco
- Entidade que existe por só só, é autônoma.
- Exemplo: header, container, menu, checkbox,input

```sh
.menu {}
```

## bEm - Elemento 
- Faz parte do bloco, elemento-filho.
- Fica vinculado ao seu bloco de origem.
- Exemplo: menu item, list item, checkbox caption, header title.

```sh
.menu__item {}
.menu__link {}
```

## beM - Modificador
- Uma variante de um bloco ou elemento.
- Ele muda aparência.
- Varia uma propriedade.
- Atribuir uma estado.
- Exemplo: disabled, highlighted, checked, fixed, size big,color yellow.

```sh
.menu--dark {}
.menu__item--disable {}
```

## Boas práticas  BEM:
- Não replique estrutura HTML *Ver BEM_correto.html e BEM_errado.html
- O elemento desendente herda a descrição do bloco.
- Usar Bloco dentro de bloco e elemento dentro de bloco.

# Namespaces CSS
- Evitar conflitos de nomes.
- Codigo mais informativo e comunicativo.
- Identifica as funções e responsábilidades.
- Trás confiança nos códigos.
- Namespaces identificadores para css.

## Referencias:
- [https://zellwk.com/blog/css-architecture-2/]

```sh
    .l-: layouts
    .o-: objects
    .c-: components
    .js: JavaScript hooks
    .is-|.has-: state classes
    .t1|.s1: typography sizes
    .u-: utility classes
```