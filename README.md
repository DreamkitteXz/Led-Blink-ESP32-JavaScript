<h2 align='center'>Piscando o Led com JS no ESP32</h2>
      <h3 align='center'>Pinagem do ESP32</h3>
      <p align='center'>Aqui esta uma <a href="https://microdigisoft.com/getting-started-with-the-esp32-development-board/">Imagem</a> da pinagem do ESP32.</p>
      <p align='center'><img src="https://i0.wp.com/microdigisoft.com/wp-content/uploads/2021/09/ESP32-pinout.png?fit=1024%2C541&ssl=1?v=1634300311" alt="Screen" width="811" height="428"></p>
    <h3 align='center'>Circuito LED</h3>
      <p align='center'>Aqui esta o circuito que iremos utilizar para piscar o led. Foram utilizados os pinos <code>D22</code> e <code>GND</code>.</p>
      <p align='center'><img src="Images\circuit.png" alt="Screen" width="627" height="457"></p>
<h3 align='center'>Executando o código</h3>
<p align='center'>Execute o seguinte código no Espruino IDE</p>
<p align='center'><pre>
<code>
var led = new Pin(22);
var toggle=1;

setInterval(function() {
    toggle=!toggle;
  digitalWrite(led, toggle);
}, 500);</code>
</pre></p>
<p align='center'>Você deve esperar o LED conectado ao D22 piscando</p>
<p align='center'><img src="https://raw.githubusercontent.com/DreamkitteXz/Arduino-IDE-com-ESP32/main/Images/ezgif.com-gif-maker%20(5).gif" alt="Screen" width="600" height="338"></p>
