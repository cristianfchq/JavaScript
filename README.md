# operadores

- suma                    +  
- resta                   -
- multiplicacion           *
- division                /

- comparacion             ==
- distinto                !=
- mayor o mayorIgual      > >=
- menor o menorIgual      < <=

- &&	Operador and (y)	a && b
- ||	Operador or (o)	a || b
- !	Operador not (no)	!a


# blucles y condicionales
## if
if (condicion) {
    sentencia1;
} else {
    sentencia2;
}
## while
while (condicion)
{
    sentencia;    
}

do
{
    sentencia;
}
while (condición);
## swith
switch (expresión) {
    case valor1:
      //Declaraciones ejecutadas cuando el resultado de expresión coincide con el valor1
      break;
    case valor2:
      //Declaraciones ejecutadas cuando el resultado de expresión coincide con el valor2
      break;
    case valorN:
      //Declaraciones ejecutadas cuando el resultado de expresión coincide con valorN
      break;
    default:
      //Declaraciones ejecutadas cuando ninguno de los valores coincide con el valor de la expresión
      break;
}   

## for
for (var i = 0; i < 9; i++) {
    n += i;
    mifuncion(n);
}
## for each
for each (variable in objeto)
{
    sentencia
}

- El siguiente fragmento de código itera sobre las propiedades de un objeto, calculando su suma:

var sum = 0;
var obj = {prop1: 5, prop2: 13, prop3: 8};
for each (var item in obj) {
  sum += item;
}
print(sum); // imprime "26", que es 5+13+8

# funciones

function nombre([parametro1] [,parametro2] [..., parametroN]) {sentencias}

function calcular_ventas(unidades_a, unidades_b, unidades_c) {
    return unidades_a*79 + unidades_b * 129 + unidades_c * 699;
}