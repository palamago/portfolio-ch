#Soporte
http://caniuse.com/#feat=flexbox


 inicial

```css
#contenedor{
	height: 400px;
	background-color: #fff;
	margin: 20px;
	border: 5px solid orange;
	padding: 10px;
}

.item{
	color: #fff;
	background-color: steelblue;
	text-align: center;
	margin: 10px;
	padding: 10px;
}
```

#Para el padre

###Display Flex

Esta propiedad nos permite establecer cual sera el contenedor de los elementos a los que queremos dar un acomodo y/o distribución.

```css
display: flex | inline-flex;

###Flex Direction

Nos permite establecer la dirección en la que se acomodaran nuestros elementos.

```css
flex-direction: row | column | row-reverse | column-reverse ;
```

###Flex Wrap

Podemos indicar si todos los elementos estarán en linea con su máximo ancho posible o establecido o si queremos que respete el ancho y los elementos se posicionen en varias lineas de elementos.

```css
flex-wrap: no-wrap | wrap | wrap-reverse;
```

###Flex Flow

Es un atajo entre flex-direction y flex-wrap.

```css	
flex-flow:row wrap;
/* Primer valor es el valor que le daríamos a flex-direction */
/* Segundo valor es el valor que le daríamos a flex-wrap */
```

###Justify Content

Nos permite decidir la posición de nuestros elementos y la distribución que tendran.
	
```css
justify-content: flex-end | flex-start | center | space-around | space-between ;
```

###Align Items

Nos permite posicionar / distribuir elementos verticalmente. (solo para una linea de elementos)

```css	
align-items: flex-start | flex-end | center | stretch | baseline;
```

###Align Content

Nos permite posicionar / distribuir elementos verticalmente, igual que align-items, solo que align-content solo funciona para lineas de elementos, por ejemplo cuando tenemos establecido un flex-wrap:wrap; y los elementos se posicionan en VARIAS LINEAS.

```css
align-content: flex-start | flex-end | center | stretch | space-between | space-around ;
```

#Para el hijo

###Flex Basis

Establecemos el tamaño que tendrá un elemento.

```css
flex-basis:1;
```

###Flex Grow

Establecemos la proporción de crecimiento que tendrá un elemento a comparacion con los demás.

```css
flex-grow:1;
```

###Flex Shrink

Establecemos la proporción de encogimiento que tendrá un elemento a comparacion con los demás.
	
```css
flex-shrink:1;
```

###Flex

Atajo entre flex-grow, flex-shrink, flex-basis

```css
flex:1 1 50%;
```

###Order

Establecemos el orden que tendrá un elemento a comparacion con otros elementos.

```css
order:;
```

###Align Self

Nos permite alinear un elemento independientemente de los demás

```css
align-self: flex-start | flex-end | center | stretch | baseline ;
```