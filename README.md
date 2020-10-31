<h1 style="text-align: center;"> Meses de trabalho </h1>
 Esse programa é apenas para dizer quantos meses um funcionário trabalhou em uma empresa. Nele foi usado html, css e JS.

<h1 style="text-align: center;"> HTML </h1>

### Dentro do corpo do html foi criado divs que possuem um conteúdo main com um formulário referentes ao d/m/aa em que o usuário foi contratado e ao d/m/aa em que o usuário foi demitido. Vale ressaltar, que no corpo dos inputs possuem uma propriedade, na qual através dela podemos o identificar, essa propriedade é o ID(como se fosse o nome dele), a partir disso podemos usá-los futuramente em funções, as quais irão pegar o valor atribuído pelo usuário por meio desse id. Ademais, foi criado também, dentro da mesma div e do mesmo formulário referente ao CONTRATADO/DEMITIDO, um button. Esse ficou responsável pela parte em que conecta o html ao js, nele existe uma propriedade chamada onclick, a mesma fica encarregada de chamar uma função que retorna algo para o usuário. Função esta que será criada no JS.
como chama uma função?

<h1 style="text-align: center;"> CSS </h1>

### Na div criada no html coloquei uma class a qual estilizei no css. Coloquei para ela uma width e um height de 100vw e 100vh, respectivamente. Isso para que a div container, (a qual tem todo o conteúdo dentro, como o formulário), ocupasse a largura e altura completa do monitor. Além disso, utilizei o displey flex para ocupar o seu lugar e alinhei tudo ao centro, já com o flex-direction coloquei-os em colunas para que o conteúdo main ficasse a baixo do h1.

### Como havia criado um h1, resolvi estilizá-lo para colocar uma font-size, font-family e uma cor diferente, além da intonação da font com um font-weight. Com isso feito, estilizei o main, o qual tem o formulário. Coloquei um background: white(branco) e defini uma largura e altura fixa. Além disso, novamente utilizei o displey flex e com o aling-items alinhei todos os itens do main ao centro.

### Com isso feito, defini ao form que ele ocupasse, com o displey flex, todo o seu lugar e que ficasse todos os itens em colunas com o flex-direction, mas também, novamente, alinhei os itens ao centro.

#### Então, estilizei o input para que tivesse uma border-radius e um background cinza. Dei também um margin-top para que desgrutassem uns dos outros.

### Com o button também dei um margin-top e utilizei o hover para quando o usuário clicar ter um background diferente e uma color da fonte difente.

<h1 style="text-align: center;"> JavaScript </h1>

### A parte lógica ficou responsável pelo JS(JAVASCRIPT). Nela iremos criar a função que será realizada quando o usuário apertar no button de submit(ou seja, quando o mesmo nos enviar). O JS é chamado no html por meio da tag <script></script> A função seja criada dentro dessa tag.

## como criar uma função???

```
function nameFunction(){

}
```

### Dito isso, é necessário apenas pegar os dados que o usuário digitou no input. Como fazer isso? Por meio do id que foi atribuído no input, como explicado anteriomente. Sendo assim usaremos uma variável para guardar esse valor. Para podermos ter acesso a tudo isso, é preciso apenas usar o document.querySelect('').value; e dentro dos parentêses passarmos o id.

document.querySelect('#').value; Para id é usado # e o nome do mesmo, o qual foi atribuído no input.

ex:
```
document.querySelect('#name').value;
```
Logo após pegar todos os valores passados pelo usuário é preciso armazená-lo na variável. 
```
ex: var name = document.querySelect('#name').value;
```

### Lá a gente pegou os days, months, years tanto inicial quanto final. A lógica do problema era apenas informar ao usuário o quanto de meses o mesmo ficou na empresa.

## Então para sabermos isso foi preciso usar a estrutura de condição e a lógica booleana: 

- IF, ELSE IF, ELSE.
- (true, false) do AND(&&).

**Lembrando: a lógica do AND só funciona se todas as condições foram verdadeira, caso não, ela passa para a próxima. Por que o ELSE IF(ELIF)? Porque estamos tratando de uma mesma variável, então o else if se encaixa perfeitamente para esse exemplo.**

### Por fim é preciso ter a lógica de que o usuário pode ter passado apenas alguns dias, alguns meses, ou alguns anos. Pode também ter passado meses incompletos(então é concactenado com os dias). Como o exemplo pedia em meses, foi preciso converter os anos em meses. 1 ANO ------ 12 MESES TAL ANO -------- TAL MESES

### Para isso multiplicamos o ano que o usuário permaneceu na empresa por 12. (ano final - ano inicial)*12. Caso o usuário tenha passado 1 ano e 3 meses vai ser igual a 15 meses.
### Os dias não podem ser convertidos em meses, porém os anos sim. Caso ele tenha passado só alguns dias, então ele irá receber apenas os dias que passou lá.



