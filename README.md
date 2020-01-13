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

function nombre([parametro1] [,parametro2] [..., parametroN]) {
  
  sentencias
  
}

function calcular_ventas(unidades_a, unidades_b, unidades_c) {

    return unidades_a*79 + unidades_b * 129 + unidades_c * 699;

}

## DOM

- Para obtener un valor de input 

En este caso se obtiene los datos de un formulario que tiene un id = 'product-form' y escuchar el evento de tipo submit y dentro obtenemos el valor del input que tiene un id = 'name'

document.getElementById('product-form').addEventListener('submit', function(e){

    name = document.getElementById('name').value;
    
    e.preventDefault();

})

- Para cancelar el comportamiento por defecto del formulario

document.getElementById('product-form').addEventListener('submit', function(){

    //sentencias de codigo

})

document.getElementById('product-form').addEventListener('submit', function(e){

    //sentencias de codigo
    
    e.preventDefault();

})

- Para insertar o crear un elemento HTML

    const productList = document.getElementById('product-list');
    
    const element = document.createElement('div');

    element.innerHTML = `

    <div class="card text-center mb-4">
    
        <div class="card-body">
    
            <strong>Product Name</strong> : ${product.name}
    
            <strong>Product Price</strong> : ${product.price}
    
            <strong>Product Year</strong> : ${product.year}
    
        </div>
    
    </div>
    
    `;

    productList.appendChild(element); //para insertar el elemento hijo que es el element dentro de productList que es un div en html con id 'product-list'

    Ejemplo:

    addProduct(product){
    
        const productList = document.getElementById('product-list');
    
        const element = document.createElement('div');
    
        //card una vez se inserta el producto
    
        element.innerHTML = `
    
        <div class="card text-center mb-4">
    
            <div class="card-body">
     
                <strong>Product Name</strong> : ${product.name}
    
                <strong>Product Price</strong> : ${product.price}
    
                <strong>Product Year</strong> : ${product.year}
    
            </div>
    
        </div>
    
        `;

        productList.appendChild(element);

    }

- para ver por consola la parte del html que estamos haciendo click

document.getElementById('product-list').addEventListener('click',function(e){

    console.log(e.target);

})

- 