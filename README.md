![image description](https://storage.googleapis.com/dpw/app/uploads/2020/05/image.png)

# best-practices-for-front
Documentação com exemplos criada para a equipe front-end da EULABS [https://eulabs.com.br/]

Conteúdo:
1- BEM, metodologia CSS / convenção de nomenclatura para deixar o código front end no padrão internacional.
2- Namespaces CSS
3- QuasaJS Typography

# 1 - BEM css

## Referencias:
- [https://getbem.com/]
- [https://desenvolvimentoparaweb.com/css/bem/]

## Metodologia/Convenção BEM:
- Convenção de nomes de classes e só...
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

## (B)em - Bloco
- Entidade que existe por sí só, é autônoma.
- Exemplo: header, container, menu, checkbox,input

```sh
.menu {}
```

## b(E)m - Elemento 
- Faz parte do bloco, elemento-filho.
- Fica vinculado ao seu bloco de origem.
- Exemplo: menu item, list item, checkbox caption, header title.

```sh
.menu__item {}
.menu__link {}
```

## be(M) - Modificador
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
- O elemento descendente herda a descrição do bloco.
- Usar Bloco dentro de bloco e elemento dentro de bloco.

# 2 - Namespaces CSS
- Evitar conflitos de nomes.
- Código mais informativo e comunicativo.
- Identifica as funções e responsábilidades.
- Traz confiança nos códigos.
- Namespaces identificadores para css.

## Referencias:
- [https://zellwk.com/blog/css-architecture-2/]

```sh
    .l-: layouts
    .o-: objects
    .c-: components
    .js-: JavaScript hooks // Classes manipuladas por JS // Não usar para estilo
    .is-|.has-: state classes // Estado ou condição das classes
    .u-: utility classes
    .s-: scope
    .qa-: QA classe para testes
    .s1|.t1: typography sizes
        .t1 - largest font-size.
        .t2 - second largest font-size.
        .t3 - third largest font-size.
        .s1 - first font-size smaller that base font-size.
        .s2 - second font-size smaller that base font-size.
```

## Boas práticas  Namespaces css:
- Usar !importante somente em classes utilitárias .u-


# 3 - QuasarJS Namespaces & Typography
- Tipografia e padronização das classes css no QuasarJs

## Referencias:
- [https://quasar.dev/style/typography]

```sh
    .q- : components do quasar |
        ex:  .q-tab-panels {
                box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.05);
                border-radius: 0 0 8px 8px;
              }
        [
            <q-tab-panels>
                ....
            </q-tab-panels>
        ]

    .clr- : set color | ex: clr-white: #ffffff;
        [
             <q-icon color="white" /> ou
             <q-icon class="clr-white" />
        ]

    .bcg- : set background | ex: bcg-white: #ffffff;
        [
             <q-btn class="bcg-white" /> ou
             <q-pagination color="white"/>
        ]

    .text- : set style/size/align para textos | ex: text-white: #ffffff;
        [
            <div class="text-white text-bold">Tipo ônibus</div>
        ]

```

## Boas práticas  QuasarJS Typography:
- Quando for mudar o style do componente do quasar globalmente deve-ser seguir a tipografia do framework.
