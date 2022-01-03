---
layout: post
title:  "Começando com Arduino!"
date:   2022-01-02 05:55:00 -0300
author: "Arthur Kuwahara"
categories: ARDUINO APRENDENDO
---
Comentei um tempo atrás com a Melissa que eu estava planejando comprar um Arduino. Até então, meus conhecimentos sobre isso eram: os obtidos nas três aulas que frequentei de Organização de Computadores Digitais (do professor Simões) e alguma coisa de conhecimento comum na internet.

Passaram-se algumas semanas e, no início de novembro, Melissa me presenteou com uma UNO R3 CH340G Atmega328P ![Alt Text](/uno-r3.jpg/), uma versão da [Arduino UNO](arduino-uno). Obviamente, fiquei muito feliz, mas por conta de uma viagem acabei levando um tempo para poder mexer na placa.

De início, comecei a usar o [Tinkercad](https://www.tinkercad.com/) para aprender o básico das [protoboards](https://pt.wikipedia.org/wiki/Placa_de_ensaio) e de Arduino.

Depois me aventurei com a LED interna da placa. Melissa me deu uma protoboard depois de eu aprender o básico (a gente não tinha ideia do que precisava para começar a brincar com os protótipos). Fiz um código básico em Arduino, no caso, o *blink*, que é basicamente fazer a LED interna ficar piscando:

```cpp
void setup() {
  // 
  pinMode(LED_BUILTIN, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);   // turn the LED on (HIGH is the voltage level)
  delay(1000);                       // wait for a second
  digitalWrite(LED_BUILTIN, LOW);    // turn the LED off by making the voltage LOW
  delay(1000);                       // wait for a second
}
```

Depois disso, fiz algumas variações, como por exemplo: escrever "MELISSA" em código morse ou fazer a LED piscar mais rapidamente.

Futuramente, quando a protoboard chegar, pretendo comprar botões, LEDs RGB, muitos cabos, resistores etc.

[arduino-uno]:https://store.arduino.cc/products/arduino-uno-rev3/
