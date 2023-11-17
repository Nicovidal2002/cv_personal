# Ejemplos de código desarrollados por mi.

## KOTLIN
```kotlin

fun main {
    
    println("Cual es tu peso?")
    val peso= readln().toDouble()
    println("Ahora escribe tu altura en metros")
    val altura= readln().toDouble()

    val imc= peso/ (altura * altura)
    println("tu IMC es $imc")

    println("tabla IMC")
    println("---------")
    println("Delgado: <18.5")
    println("Normal: entre 18.5 y 24.9")
    println("Sobrepeso: entre 25 y 29.9")
    println("Obeso: >=30")

    if (imc <18.5) {println("Estás delgado")}
    if (imc >=18.5 && imc <=24.9 ) {println("Estás en un peso normal")}
    if (imc >=25 && imc <=29.9) {println("Estás en sobrepeso")}
    if (imc >=30) { println("Estás obeso")}

}
```

## JAVAC

```java

class Coche {
	
    String modelo;
	int pasajeros;
	int deposito;
	int kpl;

	Coche(String m, int p, int d, int k) {
	modelo = m;
	pasajeros = p;
	deposito = d;
	kpl = k;
	}
	int calcularAutonomia() {
	return deposito * kpl;
	}


	Coche mayorAutonomia(Coche c){
		Coche cocheMayorAut= new Coche("nada",0,0,0);
		if(calcularAutonomia()>c.calcularAutonomia()){
			cocheMayorAut.modelo=modelo;
			cocheMayorAut.pasajeros=pasajeros;
			cocheMayorAut.deposito=deposito;
			cocheMayorAut.kpl=kpl;
		}else{
			cocheMayorAut.modelo=c.modelo;
			cocheMayorAut.pasajeros=c.pasajeros;
			cocheMayorAut.deposito=c.deposito;
			cocheMayorAut.kpl=c.kpl;
		}
		return cocheMayorAut;
	}
}

class Unidad2 {
	
    public static void main(String[] args) {
		Coche coche1 = new Coche("un coche", 5, 60, 20);
		Coche coche2 = new Coche("otro coche", 7, 70, 30);
			Coche coche3=coche1.mayorAutonomia(coche2);
			System.out.println("el coche de mayor autonomía es: "+ coche3.modelo);
	}
}
```

## HTML
```html

<html>
    <head>
        <title>My first webpage</title>
        <link rel="shortcut icon" href="./IMG/favicon.ico" type="image/x-icon">
    </head>
    <body>
        <!--Comment in HTML-->
        <h1>heading number 1</h1>
        <h2>heading number 2</h2>
        <p>Hello HTML!</p>
        <h2>repeated<strong>strong</strong>heading<em>empathic</em>number 2</h2>
        <h2>repeated heading number 2</h2>
        <h3>normal text</h3>
        <h4>heading 4</h4>
        <h5>heading 5</h5>
        <h6>heading 6</h6>
        <p>Git Hub</p>
        <img src="IMG/lion1.jpg" alt="lion" width="500">
        <img src="https://cdn0.ecologiaverde.com/es/posts/7/3/9/el_canguro_en_peligro_de_extincion_causas_e_informacion_1937_600_square.jpg" alt="url" width="600">
        <h2>Unordered list of fruits</h2>
        <ul>
            <li>Apple</li>
            <li>Orange</li>
            <li>Strawberry</li>
            <li>Grape</li>
        </ul>
        <h2>Ordered lst of beautiful places:</h2>
        <ol>
            <li>Beach</li>
            <li>Wood</li>
            <li>City</li>
            <li>Museum</li>
        </ol>
        Links
        <a href="#top">Top</a>
        <a href="./link.html">Link page</a>
        <br>
        <a href="https://www.ecologiaverde.com/el-canguro-en-peligro-de-extincion-causas-e-informacion-1937.html" target="_blank">Macropus rufus</a>
    </body>
</html>

```

## Ejemplo de repositorio en Git-Hub

[![Alt text](img/GitHub-Mark-ea2971cee799.png)](https://github.com/Nicovidal2002/cv_personal)


