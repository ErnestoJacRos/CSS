# tipos de posicionamiento 
## static
es el valor por defecto en display: block; 
no podemos usar top , left, right, bottom  
## relative
ya podremos usar: top, left, right, bottom y mover ese objeto
pero es parte del margin y este se mueve respecto a si posicion oirnal 
si tiene un marge de 10px y ponemos posición position:relative;
left:10px; despegará 10px del lado izquierdo respecto a la pósición actual
10px de la izquierda si ponemos position:relative ;
top:10px; se despegara 10px de arriba he se irá a hacia bajo.
si le aplicamos esa position:relative; y agregamos más objetos ese objetos
se posicionarán en manera natural, pero, no tomará le lugar del objeto que le hemos puesto position 
## fixed
si usamos positio:fixed; top:10px; left:10px;
perdera su posición anterior y otro elementos podrán tomar esos espacios
se va a posicionar de manera relativa al viewport o sea  la pantalla
quetengamos disponible, y se coloca encima de otros objetos y ponerlo  en cualquier lugar 
y asi estará de manera fija a pesar que hagamos scrolla a la  pag este se seguira mostrando, normalte lo usamos para menus de navegación y icono de chat 

## absolute
el div padre debe ser diferente a position:static; para que funcione 
normalmente lo vamos a usar cunado usamos un div en un div padre 
ya que se va a posionar respecto al y en caso de no tner un padre 
se va a posicionar respecto a viewport pero el padre no deber  una position:static ;
al poner position:absolue; en un elemnto como un div que ocuparía todo el ancho d ela pág, al hacerlo "absolute" solo ocupara el espacio que necesario 
es como si fue un elemento de display:inline;() 
## sticky
funciona como position: fixed;