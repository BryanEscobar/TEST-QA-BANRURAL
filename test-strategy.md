
Plan de Ataque 
Bryan Adrián Escobar Menéndez 

-------------------------------------------------------------------------------------------------------------
line 87: guessSubmit.addeventListener('click', checkGuess);
addeventListener = addEventListener
	
	Presenta error de sintaxis, posee letra minuscula y debe de ser mayuscula "Event"

-------------------------------------------------------------------------------------------------------------
line 46: const ATTEMPS = 5;
const ATTEMPS = 5; = const ATTEMPS = 10;

Tenia los intetos como limite a 5, y tenia que ser a 10 segun las instrucciones del plan.

-------------------------------------------------------------------------------------------------------------
line 49: const lowOrHi = document.querySelector('lowOrHi');
('lowOrHi'); = ('.lowOrHi');

	Presenta error de sintaxis, para llamar correctamente un elemento por medio del nombre de la clase debe llevar un "." al principio

-------------------------------------------------------------------------------------------------------------
line 95: resetButton.addeventListener('click', resetGame);
addeventListener = addEventListener

	Presenta error de sintaxis, posee letra minuscula y debe de ser mayuscula "Event"

-------------------------------------------------------------------------------------------------------------
line 56: function checkGuess()

Dentro de dicha función hacia falta condición de el numero ingresado es entero o no. Si no imprime un mensaje en pantalla
 lowOrHi.textContent = 'El numero debe ser un entero!';

-------------------------------------------------------------------------------------------------------------
line 71, 72: lastResult.textContent = 'Felicitaciones! adivinaste el número!';
      lastResult.style.backgroundColor = 'green';

Se corrigo el color que deberia de aparecer en el modal, anteriomente salia en rojo y deberia de ser en verde.

-------------------------------------------------------------------------------------------------------------
line 75, 76:       lastResult.textContent = 'Incorrecto! ';
      lastResult.style.backgroundColor = 'red';


Se corrigo el color que deberia de aparecer en el modal, anteriomente salia en verde y deberia de ser en rojo.


-------------------------------------------------------------------------------------------------------------
line 66, 67:       lastResult.textContent = '!!!Perdiste!!!';
      lastResult.style.backgroundColor = 'red';


Se corrigo el color que deberia de aparecer en el modal, anteriomente salia en negro y deberia de ser en rojo.


-------------------------------------------------------------------------------------------------------------
line 78 , 79, 80 : lowOrHi.style.color = 'white';
	lowOrHi.textContent = 'El número es mayor!';
        lowOrHi.style.backgroundColor = 'black';

Se corrigo los colores de los modales de alerta, adiconal se le agrego color blanco al texto para que se pudiera leer


-------------------------------------------------------------------------------------------------------------
 line 82, 83, 84 :        lowOrHi.style.color = 'white';
        lowOrHi.textContent = 'El número es menor!';
        lowOrHi.style.backgroundColor = 'black';

Se corrigo los colores de los modales de alerta, adiconal se le agrego color blanco al texto para que se pudiera leer


-------------------------------------------------------------------------------------------------------------
line 64 : if(userGuess > 0 && userGuess < 101){
    }
Se agrego una validación que evalue si el numero ingresado es mayor o menor de 100 como lo solicta el caso


-------------------------------------------------------------------------------------------------------------
line 65:   guesses.textContent += userGuess + ', ';
se le agrego una "," para separacion del contador de los valores ingresados, para legibilidad


-------------------------------------------------------------------------------------------------------------
line: 66 a la 70
      if(userGuess === randomNumber) {
      lastResult.textContent = 'Felicitaciones! adivinaste el número!';
      lastResult.style.backgroundColor = 'green';
      setGameOver();
    } else if(guessCount === ATTEMPS) {
      lastResult.textContent = '!!!Perdiste, tus 10 intentos se agotaron!!!';
      lastResult.style.backgroundColor = 'red';
      lowOrHi.textContent = '';
      setGameOver();
     } 

Se les cambio logica a las validaciones ya que en la primera lanzaba el mensaje que perdiste y en la segunda validación de Felicidades, y era lo contrario.




