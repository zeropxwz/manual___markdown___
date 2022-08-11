# Markdown manual

## параграфы и текст 

Абзацы создаются при помощи пустой строки.  
Если вокруг текста сверху и снизу есть пустые строки, то текст превращается в абзац.

Чтобы сделать перенос строки вместо абзаца,   
нужно поставить два пробела в конце предыдущей строки.

## Заголовки

Заголовки отмечаются диезом `#` в начале строки, от одного до шести. Например:

```md
# Заголовок h1
## Заголовок h2
### Заголовок h3
#### Заголовок h4
##### Заголовок h5
###### Заголовок h6
```
В декоративных целях заголовки можно «закрывать» с обратной стороны.
```md
# Заголовок h1 #
```

## списки

Для разметки неупорядоченных списков можно использовать:  

`*`  
`-`  
`+`  

```md
- элемент 1
- элемент 2
- элемент ...
- элемент n
```

Вложенные пункты создаются четырьмя пробелами перед маркером пункта:

```md
* элемент 1
* элемент 2
    * вложенный элемент 2.1
    * вложенный элемент 2.2
* элемент ...
```

Упорядоченный список:  

```md
1. элемент 1
2. элемент 2
    1. вложенный
    2. вложенный
3. элемент 3
```

На самом деле не важно как в коде пронумерованы пункты, главное, чтобы перед элементом списка стояла цифра (любая) с точкой. Можно сделать и так:  

```md
0. элемент 1
0. элемент 2
0. элемент 3
0. элемент 4
```

## Цитаты

Цитаты оформляются как в емейлах, с помощью символа `>`

```md
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
```

В цитаты можно помещать всё что угодно, в том числе вложенные цитаты:  

```md
> ## This is a header.
>
> 1.   This is the first list item.
> 2.   This is the second list item.
>
> > Вложенная цитата.
>
> Here's some example code:
>
>     return shell_exec("echo $input | $markdown_script");
```

## Исходный код

Блок с исходным кодом указывается тремя ковычками и расширением языка: ` ```js // here yor code ``` `

## Инлайн код

Для вставки кода внутри предложений нужно заключать этот код в апострофы: 
```md
обычный текст `<html class="ie no-js">`, продолжение обычноего текста
```
