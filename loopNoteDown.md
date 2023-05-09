## LOOP WHILE

Para criar um loop while, é bem parecido com o if;
````
$number =0;

while($number < 10) {
    echo "N. ".$number . "<br>";
    number += 1;
}
````
******************************************
## LOOP FOR
estrutura:

1 parâmetro: definir uma variável;
2 condição;
3 a cada fim de loop;
````
for($numero = 0; $numero < 10; $numer0++ "esse ++ significa incrementar">) {
    echo "N. ".$number . "<br>";
};
````
******************************************
## LOOP FOREACH
tem um único propósito, trabalhar com arrays.

Realizando noso loop desta maneira, estamos apenas pegango o valor, ou seja a variável $newIngredients é nosso variavel correspondente ao valor. Se quisermos pegar a chavede identificação, podemosar usar a sseguinte estrutura:
```` 
    foreach($ingredients as $key => $newIngredients) {
        echo "Item $key: " .$newIngredients . '<br>';
    };
    
````
desta maneira, podemos exibir nosso index de cada item do array;
isso é muito útil, mas vale ressaltar que como programador, noso array sempre vai começar do zero, então o item que seria o 1 para o usuário, para nos vai er zero, e irá aparecer como zero, nesse caso, para resolver podemo fazer uma expressão e somar 1.

Ficará desta forma:
`````
echo '<h2>Ingredients</h2>';
foreach($ingredients as $key => $newIngredients) {
    echo "Item ". ($key +1). ":".$newIngredients . '<br>';
};

`````
<hr>

````
<h2>última aula - foreach</h2>
<?php
$ingredients = [
    'apple',
    'orange',
    'pineapple',
    'mango',
    'guava',
    'blueberry',
    'banana'
];

echo '<h2>Ingredients</h2>';

echo '<ul>';
foreach($ingredients as $ingredient) {
    echo '<li>'.$ingredient.'</li>';
};
echo '</ul>';

;
````
