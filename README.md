# Meses_de_trabalho
Esse programa é apenas para dizer quantos meses um funcionário trabalhou em uma empresa. Nele foi usado html, css e JS.
Explicação:

============================ Parte do html =============================

Dentro do corpo do html foi criado divs que possuem um conteúdo main com um formulário (

) referentes ao d/m/aa em que o usuário foi contratado e ao d/m/aa em que o usuário foi demitido. Vale ressaltar, que no corpo dos inputs possuem uma propriedade, na qual através dela podemos o identificar, essa propriedade é o ID(como se fosse o nome dele), a partir disso podemos usá-los futuramente em funções, as quais irão pegar o valor atribuído pelo usuário por meio desse id. Ademais, foi criado também, dentro da mesma div e do mesmo formulário referente ao CONTRATADO/DEMITIDO, um button. Esse ficou responsável pela parte em que conecta o html ao js, nele existe uma propriedade chamada onclick, a mesma fica encarregada de chamar uma função que retorna algo para o usuário. Função esta que será criada no JS.
como chama uma função?

^^^^^^ ============================ Parte do css ==============================

No css, usei só para não ficar tão feio o formulário skdsjkaskds

Na div criada no html coloquei uma class a qual estilizei no css. Coloquei para ela uma width e um height de 100vw e 100vh, respectivamente. Isso para que a div container, (a qual tem todo o conteúdo dentro, como o formulário), ocupasse a largura e altura completa do monitor. Além disso, utilizei o displey flex para ocupar o seu lugar e alinhei tudo ao centro, já com o flex-direction coloquei-os em colunas para que o conteúdo main ficasse a baixo do h1.

Como havia criado um h1, resolvi estilizá-lo para colocar uma font-size, font-family e uma cor diferente, além da intonação da font com um font-weight. Com isso feito, estilizei o main, o qual tem o formulário. Coloquei um background: white(branco) e defini uma largura e altura fixa. Além disso, novamente utilizei o displey flex e com o aling-items alinhei todos os itens do main ao centro.

Com isso feito, defini ao form que ele ocupasse, com o displey flex, todo o seu lugar e que ficasse todos os itens em colunas com o flex-direction, mas também, novamente, alinhei os itens ao centro.

Então, estilizei o input para que tivesse uma border-radius e um background cinza. Dei também um margin-top para que desgrutassem uns dos outros.

Com o button também dei um margin-top e utilizei o hover para quando o usuário clicar ter um background diferente e uma color da fonte difente.

=============================== Parte do js ==============================

A parte lógica ficou responsável pelo JS(JAVASCRIPT). Nela iremos criar a função que será realizada quando o usuário apertar no button de submit(ou seja, quando o mesmo nos enviar). O JS é chamado no html por meio da tag <script></script> A função seja criada dentro dessa tag.

como criar uma função???

function nameFunction(){

}

^^^^^ Dito isso, é necessário apenas pegar os dados que o usuário digitou no input. Como fazer isso?

Por meio do id que foi atribuído no input, como explicado anteriomente.

sendo assim usaremos uma variável para guardar esse valor. Para podermos ter acesso a tudo isso, é preciso apenas usar o document.querySelect('').value; e dentro dos parentêses passarmos o id.

document.querySelect('#').value; Para id é usado # e o nome do mesmo, o qual foi atribuído no input.

ex:

document.querySelect('#name').value;

Logo após pegar todos os valores passados pelo usuário é preciso armazená-lo na variável. ex: var name = document.querySelect('#name').value;

lá a gente pegou os days, months, years tanto inicial quanto final.

a lógica do problema era apenas informar ao usuário o quanto de meses o mesmo ficou na empresa.

então para sabermos isso foi preciso usar a estrutura de condição: IF, ELSE IF, ELSE.

E a lógica booleana(true, false) do AND(&&).

Lembrando: a lógica do AND só funciona se todas as condições foram verdadeira, caso não, ela passa para a próxima. Por que o ELSE IF(ELIF)? Porque estamos tratando de uma mesma variável, então o else if se encaixa perfeitamente para esse exemplo.

Por fim é preciso ter a lógica de que o usuário pode ter passado apenas alguns dias, alguns meses, ou alguns anos. Pode também ter passado meses incompletos(então é concactenado com os dias). Como o exemplo pedia em meses, foi preciso converter os anos em meses. 1 ANO ------ 12 MESES TAL ANO -------- TAL MESES

Para isso multiplicamos o ano que o usuário permaneceu na empresa por 12. (ano final - ano inicial)*12

Caso o usuário tenha passado 1 ano e 3 meses vai ser igual a 15 meses.

Os dias não podem ser convertidos em meses, porém os anos sim. Caso ele tenha passado só alguns dias, então ele irá receber apenas os dias que passou lá.

==================================== Fim ================================

In english:

html:

Within the body of the html, divs were created that have a main content with a form () referring to the d / m / yy in which the user was hired and the d / m / yy in which the user was fired. It is worth mentioning that no body of the inputs has a property, in which we can identify it, that property is the ID (as if it were his name), from that we can recognize them in future functions, such as which ones will take the value assigned by the user through this id. In addition, a button was also created within the same div and on the same form referring to the CONTRACTOR / DEMITTED. This was responsible for the part where the html connection to js, ​​there is a property called onclick, the same is responsible for calling a function that returns something to the user. This function will be created in JS.

how do you call a function?

^^^^^^

css:

In the css, I used the skdsjkaskds form just so it wouldn't look so ugly

In the div created in the html I put a class which I styled in the css. I put a width and height of 100vw and 100vh, respectively. This is so that the div container, (which has all the content inside, like the form), occupies the full width and height of the monitor. In addition, I used the displey flex to take its place and aligned everything to the center, already with the flex-direction I placed them in columns so that the main content was below the h1.

As I had created an h1, I decided to style it to put a font-size, font-family and a different color, in addition to the font intonation with a font-weight. With that done, I stylized the main, which has the form. I put a background: white (white) and defined a fixed width and height. In addition, again I used the displey flex and with the aling-items I aligned all the items from the main to the center.

With that done, I defined the form that it would occupy, with the displey flex, all its place and that all the items be in columns with the flex-direction, but also, again, I aligned the items to the center.

So, I stylized the input so that it had a border-radius and a gray background. I also gave a margin-top for them to ungroup each other.

With the button I also gave a margin-top and used the hover for when the user clicks to have a different background and a different font color.

JS:

The logical part was responsible for JS (JAVASCRIPT). In it we will create the function that will be performed when the user presses the submit button (that is, when he sends us). JS is called in html using the <script> </script> tag The function is created within that tag.

how to create a function ???

function nameFunction () {

}

^^^^^ That said, it is only necessary to get the data that the user typed in the input. How to do this?

Through the id that was assigned in the input, as previously explained.

so we will use a variable to store that value. In order to have access to all of this, we only need to use the document.querySelect (''). Value; and within parentheses we pass the id.

document.querySelect ('#'). value; For id is used # and the name of the same, which was assigned in the input.

ex:

document.querySelect ('# name'). value;

Right after taking all the values ​​passed by the user it is necessary to store it in the variable. ex: var name = document.querySelect ('# name'). value;

there we took the days, months, years, both initial and final.

the logic of the problem was just to inform the user how many months he stayed in the company.

so to know that it was necessary to use the condition structure: IF, ELSE IF, ELSE.

And the Boolean logic (true, false) of AND (&&).

Remember: the AND logic only works if all conditions were true, if not, it moves on to the next one. Why ELSE IF (ELIF)? Because we are dealing with the same variable, then the else if fits this example perfectly.

Finally, it is necessary to have the logic that the user may have spent only a few days, a few months, or a few years. It may also have been incomplete months (so it is linked to the days). As the example asked for months, it was necessary to convert years into months. 1 YEAR ------ 12 MONTHS SUCH YEAR -------- SUCH MONTHS

To do this, we multiplied the year that the user stayed in the company by 12. (final year - initial year) * 12

If the user has spent 1 year and 3 months it will be equal to 15 months.

Days cannot be converted into months, but years can. If he has only spent a few days, then he will receive only the days he spent there.
