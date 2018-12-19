<img src="en.png" alt="English"> [ENGLISH](equipment.md) | <img src="es.png" alt="Castellano"> [CASTELLANO](equipo.md) | <img src="ca.png" alt="Català"> *CATALÀ*

Per a realitzar els projectes realitzats en aquesta pàgina web, es necessiten els elements que es mostren a la següent figura.

![Equipment](equipment.PNG)

<ul>
  <li><b>Arduino Due:</b> Hi ha diverses plaques similars d'Arduino que podrien ser utilitzats. Tots ells tenen un preu similar però diferent càrrega computacional. Per a aquest projecte s'ha seleccionat la placa Arduino Due causa del seu alt rendiment de computació i al fet que té convertidors D/A reals (la majoria de la placa Arduino només té sortida PWM).
  </li>
  <li><b>Servosistema LJ Technical Systems:</b> Aquest mòdul permet a l'usuari realitzar un control de llaç tancat, posicional o de velocitat d'un motor de CC.
    La velocitat i la direcció de rotació del motor es poden controlar mitjançant un senyal analògic o un senyal modulat en amplada de pols (PWM).
    A part d'això, la velocitat de rotació i la informació de realimentació posicional estan disponibles en forma analògica i digital, de manera que el mòdul pot ser controlat per un sistema analògic o digital. En aquest cas, controlarem el mòdul mitjançant senyals analògiques, però el controlador utilitzat per tancar el llaç serà discret, d'aquesta manera farem servir l'Arduino com convertidor A/D i D/A.</li>
</ul>   

![Motor](motorra2.png)

<ul>
  <li><b>Arduino Due shield:</b> El rang d'entrada i sortida de la nostra planta és de &plusmn 5v, mentre que el Arduino Due només pot gestionar senyals en el rang [0,3.3] v. Per evitar aquest problema, s'ha dissenyat un condicionador de senyal amb forma de <i>shield</i>. </li>
</ul>   

![DueShield](shield.png)


El disseny del *shield* està disponible a: <https://github.com/DuinoBasedLearning/Lab/blob/master/Ca/AdapSenyal.pdf>, i els *gerbers* a <https://github.com/DuinoBasedLearning/Lab/blob/master/Common/Gerbers.zip>


<ul>
  <li><b>Cables Banana:</b> Aquests cables s'utilitzen per connectar el Arduino Due amb la nostra planta. Mitjançant ells, podem obtenir i transferir dades relacionades amb el voltatge d'entrada i els voltatges de sortida del potenciòmetre i el dinamòmetre. La connexió a terra comú entre el Arduino i el servosistema també es realitza mitjançant aquests cables.</li>
  <li><b>USB cable:</b> El cable USB s'usa per connectar el Arduino Due des del <i>programming port</i> a l'ordinador.</li>
</ul>  

En les següents imatges podem analitzar el diagrama de connexió del nostre sistema. <br>
En aquests projectes, el Arduino ha estat programat mitjançant Simulink, però també pot ser programat per MATLAB. <br>
  Per a programar l'Arduino mitjançant Simulink, es necessita el paquet de suport de Simulink per Arduino. Aquest paquet permet crear i executar models de Simulink en plaques Arduino. Per a més informació <https://es.mathworks.com/hardware-support/arduino-simulink.html>. <br>
 Per a programar l'Arduino mitjançant MATLAB, es necessita el paquet de suport de MATLAB per Arduino. Aquest paquet li permet usar MATLAB per comunicar-se amb una placa Arduino. Podeu llegir i escriure dades de sensors a través de l'Arduino i immediatament veure els resultats en MATLAB sense haver de compilar. Per a més informació <https://es.mathworks.com/hardware-support/arduino-matlab.html>. <br>
  Per a més informació sobre aquests paquets <https://es.mathworks.com/discovery/programacion-arduino.html>.


![ConnectionDiagram](Connection.PNG)
![Desktop](desktop.jpg)
