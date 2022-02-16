## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/maria-carnevali/imc-calculo/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/maria-carnevali/imc-calculo/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

<meta charset="UFT-8">

<script>

    function pulaLinha() {
        document.write("<br>");
    }

    function mostra(frase) {
        document.write(frase);
        pulaLinha();
    }

    function calculaImc(altura, peso) {

        return peso / (altura * altura);
    }

    var nome = prompt("Infome seu nome");
    var alturaInformada = prompt(nome + ", infome sua altura");
    var pesoInformado = prompt(nome + ", infome seu peso");
    var imc = calculaImc(alturaInformada, pesoInformado);

    mostra(nome + ", o seu IMC é: " + imc);


    if(imc < 18.5) {

        mostra("Você está abaixo do recomendado.");
    }


    if(imc >= 18.5 && imc <=24.9) {

            mostra("Você está com o peso ideal de acordo com a OMS.");
        }


    if(imc >= 25 && imc <=29.9) {

            mostra("Você está levemente acima do peso.");
        }


    if(imc >= 30 && imc <= 34.9) {

            mostra("Atenção: obesidade grau I.");
        }


    if(imc >= 35 && imc <= 39.9) {

            mostra("Atenção: obesidade grau II (severa).");
        }


    if(imc > 40) {

            mostra("Atenção: obesidade grau III (mórbida).");
        }


</script>
