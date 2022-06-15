# Teste Blastoff - Front-End

### Construa os elementos básicos para formar uma página HTML. Ela não precisa ter nenhum conteúdo.
```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
  </body>
</html>

```


### Em um determinado projeto os cabeçalhos devem estar previamente definidos com fonte Arial, devem estar em negrito e em caixa alta. Como você faria para esses parâmetros serem implementados neste projeto?

```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Questão 2</title>
    <style>
        h1,h2,h3,h4,h5,h6{
            font-family: Arial, Helvetica, sans-serif;
            font-weight: bold;
            text-transform: uppercase;
        }
    </style>
</head>
<body>
    <h1>Cabecalho 1</h1>
    <h2>Cabecalho 2</h2>
    <h3>Cabecalho 3</h3>
    <h4>Cabecalho 4</h4>
    <h5>Cabecalho 5</h5>
    <h6>Cabecalho 6</h6>
</body>
</html>


```


### Construa utilizando HTML e JavaScript um link que ao ser clicado, abre um alerta do navegador.

```
<!DOCTYPE html>
<html>
    <head>
    <title>Questao 3</title>
    <script>
        function funcao1(){
            alert("Eu sou um alert!");
        }
    </script>
    </head>
    <body>
        <a onclick="funcao1()" value="Exibir Alert" > Clique </a>
    </body>
</html>

```

### Descreva em CSS a seguinte regra: todos os itens de uma lista devem estar orientados na vertical.
```
ul{
    display: flex;
    flex-direction: column;
}
```

### Descreva em CSS a seguinte regra: somente o último item de uma lista não deve ter uma linha na sua base.

```
ul li:not(:last-child){
    text-decoration: underline;
}

```

### - Um arquivo externo chamado styles.css precisa ser carregado na página HTML. Escreva o código para fazer tal carregamento.

```
<link rel="stylesheet" href="styles.css">    

```

### Um dos critérios de um determinado projeto é que todos os links devem ficar sublinhados quando o usuário passar o mouse por cima deles. Escreva o código para garantir essa regra.

```
a:hover{
    cursor: pointer;
    text-decoration: underline;
}
```

### Escreva um comando JavaScript onde o texto Hello World! seja exibido no console do navegador através de uma variável.
```
<script>
    const texto = "Hello World!"
    console.log(texto);
</script>
```


### Usando o mesmo código da questão anterior, substitua o texto que será exibido no console do navegador para Hello Toodoo! O novo valor deve sobrescrever o valor original.

```
<script>
    let texto = "Hello World!"
    texto = "Hello Toodoo"
    console.log(texto);
</script>

```

### Faça um algoritmo que receba um número e retorne o Fatorial desse número.Desenvolva via JavaScript a seguinte estrutura de código levando em consideração as seguintes regras: a) Uma variável deve ter o nome de sorvete de chocolate; b) Se o seu valor for igual a chocolate, deve ser exibido no alerta do navegador a mensagem: Amo sorvete de chocolate; c) Se o seu valor for outro, deve exibir a mensagem: Prefiro outros sabores.

```
<script>
    let sorveteDeChocolate = prompt("Digite o sabor do sorvete")

   if(sorveteDeChocolate.toLowerCase() === "chocolate"){
    alert("Amo sorvete de chocolate")
   }else{
    alert("Prefiro outros sabores")
   }

</script>
```

### Na função JavaScript a seguir, responda quais serão os resultados respectivos:
Saída:
```
28
30
9
```

### Em CSS existe uma maneira de sobrescrever um estilo, quando não há outra maneira, além dessa, de se fazer isso. Qual das propriedades a seguir é utilizada para isso?
Obs: Por ter duas questões 11, essa foi considerada a 11-2.

```
(c) !important
```

###  Analisando a estrutura CSS a seguir, qual cor prevalecerá no elemento HTML?

```
(c) green
```

### Levando em consideração a semântica de código, escreva o HTML de uma tabela que possui as seguintes características: a) Deve possuir 3 colunas (Nome, Idade, Gênero); b) Deve possuir 2 linhas (com dados fictícios); c) E uma última linha com todas as suas colunas mescladas.

```
<table border="1">
    <tr>
        <th>Nome</th>
        <th>Idade</th>
        <th>Gênero</th>
    </tr>
    <tr>
        <td>Ana</td>
        <td>22</td>
        <td>Feminino</td>
    </tr>
    <tr>
        <td>Cristiano</td>
        <td>23</td>
        <td>Masculino</td>
    </tr>
    <tr>
        <td colspan="3">Colunas mescladas</td>
    </tr>
</table>

```

### Utilizando grid system, não sendo necessário a responsividade, elabore uma página web que siga o layout da imagem abaixo:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Questão 14</title>
    <link rel="stylesheet" href="style.css"> 
   
</head>
<body>
    <section class="conteudo">
        <div class="header">Header</div>
        <div class="menu">Menu</div>
        <div class="main">Main</div>
        <div class="right">Right</div>
        <div class="footer">Footer</div>
    </section>

</body>

</html>
```
html


```
.conteudo{
    display: grid;
    grid-template-areas: 
    "header header header"
    "menu main right"
    "menu footer footer";
    text-align: center;
    
    background-color: rgba(0, 191, 255, 0.452);
}



.header{
    grid-area: header;
    
}

.menu{
    grid-area:menu
}

.main{
    grid-area:main
}
.right{
    grid-area:right
}

.footer{
    grid-area: footer;
}

.header,
.footer,
.main,
.menu,
.right{
    padding: 30px;
    border: 5px solid ;
    font-size: 20pt;
}
```
css

### Crie uma página web conforme o layout abaixo que seja responsiva para ser utilizada nos diferentes navegadores e dispositivos:

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Questão 15</title>
    <link rel="stylesheet" href="style.css"> 
   
</head>
<body>
    <section class="conteudo">
        <div class="A">A</div>
        <div class="B">B</div>
        <div class="C">C</div>
        <div class="D">D</div>
        <div class="E">E</div>
    </section>

</body>

</html>
```
html

```
.conteudo {
    display: grid;
    grid-template-areas:
        "A A A"
        "B B E"
        "C D E";
    text-align: center;
    gap: 10px;   
}

.A {
    grid-area: A;

}

.B {
    grid-area: B
}

.C {
    grid-area: C
}

.D {
    grid-area: D;
}

.E {
    grid-area: E
}

.A,
.D,
.C,
.B,
.E {
    padding: 30px;
    border: 5px solid;
    font-size: 20pt;
    background-color: rgba(0, 191, 255, 0.452);
}

@media screen and (max-width:532px) {

    .conteudo {
        grid-template-areas:
            "A A"
            "B B"
            "B B"
            "C D"
            "E E";
    }

}
```
css
