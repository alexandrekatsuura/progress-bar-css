# Progress-bar CSS

![GitHub repo size](https://img.shields.io/github/repo-size/alexandrekatsuura/progress-bar-css?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/alexandrekatsuura/progress-bar-css?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/alexandrekatsuura/progress-bar-css?style=for-the-badge)
![Bitbucket open issues](https://img.shields.io/bitbucket/issues/alexandrekatsuura/progress-bar-css?style=for-the-badge)
![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/alexandrekatsuura/progress-bar-css?style=for-the-badge)

[get-started-html]: https://github.com/alexandrekatsuura/get-started-html
[get-started-css]: https://github.com/alexandrekatsuura/get-started-css

## Descrição
> Componente de progress-bar utilizando apenas `css` e `div`

## CodePen
[![HORIZONTAL](https://img.shields.io/badge/horizontal%20-%23323330.svg?&style=for-the-badge&logo=codepen&logoColor=white&color=006DEC)](https://codepen.io/Alexandre-Katsuura/details/KKrMyPY)
[![VERTICAL](https://img.shields.io/badge/vertical%20-%23323330.svg?&style=for-the-badge&logo=codepen&logoColor=white&color=006DEC)](https://codepen.io/Alexandre-Katsuura/details/XWyKvKa)

## Pré-requisitos
Antes de começar, verifique se você atendeu aos seguintes requisitos:
* Conhecimento básico em HTML (Conheça em [get-started-html][get-started-html])
* Conhecimento básico em CSS (Conheça em [get-started-css][get-started-css])

## Progress-bar horizontal
### html
```
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <title>Progress-bar horizontal</title>
    <link rel="stylesheet" href="horizontal.css">
</head>
<body>
    <div class="progress-external">
        <div class="progress-internal" style="width:70%">
            <div class="progress-fill"></div>
        </div>
    </div>
</body>
</html>
```
* `<div class="progress-external">` - Consome classe `progress-external` que define `width` e `height` do elemento.
* `<div class="progress-internal" style="width:70%">` - Consome classe `progress-internal` elemento interno que vai definir a quantidade preenchida, `style="width:70%"` no width deve-se colocar a quantidade desejada.
* `<div class="progress-fill">` - Consome classe `progress-fill` elemento que efetua a animação de preenchimento.

### CSS
```
.progress-external{
    border-radius: 8px;
    border: 1px solid #808080;
    width: 200px;
    height: 20px;
    overflow:hidden;
}

.progress-internal{
    max-width: 100%;
    height: 100%;  
}


.progress-fill{
    max-width: 100%;
    width: 100%;
    height: 100%;  
    background-color: #008000;
    animation-name: progress-animation;
    animation-duration: 1s;
    animation-timing-function: linear;
}


@keyframes progress-animation {
    0% {
        width: 0;
    }
    100% {
        width: 100%;
    }
}
```

## Progress-bar vertical
### html
```
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <title>Progress-bar vertical</title>
    <link rel="stylesheet" href="vertical.css">
</head>
<body>
    <div class="progress-external">
        <div class="progress-internal" style="height:80%">
            <div class="progress-fill"></div>
        </div>
      </div>
</body>
</html>

```
* `<div class="progress-external">` - Consome classe `progress-external` que define `width` e `height` do elemento.
* `<div class="progress-internal" style="height:80%">` - Consome classe `progress-internal` elemento interno que vai definir a quantidade preenchida, `style="height:80%"` no height deve-se colocar a quantidade desejada.
* `<div class="progress-fill">` - Consome classe `progress-fill` elemento que efetua a animação de preenchimento.

### CSS
```
.progress-external{
    border-radius: 8px;
    border: 1px solid #808080;
    width: 200px;
    height: 20px;
    overflow:hidden;
}

.progress-internal{
    max-width: 100%;
    height: 100%;  
}


.progress-fill{
    max-width: 100%;
    width: 100%;
    height: 100%;  
    background-color: #008000;
    animation-name: progress-animation;
    animation-duration: 1s;
    animation-timing-function: linear;
}


@keyframes progress-animation {
    0% {
        width: 0;
    }
    100% {
        width: 100%;
    }
}
```




