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

## Bem - Bloco
- Entidade que existe por só só, é autônoma.
- Exemplo: header, footer, checkbox.

```sh
.menu {}
```

## bEm - Elemento
- Faz parte do bloco, elemento-filho.
- Fica vinculado ao seu bloco de origem.
- Exemplo: item de menu, item de lista, label de checkbox.

```sh
.menu__item {}
.menu__link {}
```

## beM - Modificador
- Uma variante de um bloco ou elemento.
- Ele muda aparência.
- Varia uma propriedade.
- Atribuir uma estado.
- Exemplo: disabled, checked, full-width, dark.

```sh
.menu--dark {}
.menu__item--disable {}
```

## Boas práticas:
- Não replique estrutura HTML

