# 🔊 PulseTone: LED & Buzzer Sync System

## 📌 Overview

PulseTone is a simple Arduino project that combines a buzzer and an LED to create a synchronized alert system. The buzzer plays a short melody while the LED lights up in sync, demonstrating basic embedded system concepts.

## 🚀 Features

* 🎵 Plays a melody using a buzzer
* 💡 LED lights up in sync with sound
* ⏱ Demonstrates timing using delays
* 🧠 Beginner-friendly Arduino project

## 🛠 Components Used

* Arduino Board (Uno/Nano)
* Buzzer
* LED
* Resistor (220Ω recommended)
* Jumper wires

## ⚙️ How It Works

The Arduino controls both the buzzer and LED. When the melody plays, the LED turns ON. After the sequence, the LED turns OFF and the system pauses before repeating.

## 💻 Code

```cpp
const int BUZZER = 5;
const int ledPin = 13;

void setup() {
  pinMode(BUZZER, OUTPUT);
  pinMode(ledPin, OUTPUT);
}

void loop() {
  digitalWrite(ledPin, HIGH);

  tone(BUZZER, 523, 150);  delay(180);
  tone(BUZZER, 659, 150);  delay(180);
  tone(BUZZER, 784, 150);  delay(180);
  tone(BUZZER, 880, 300);  delay(800);

  digitalWrite(ledPin, LOW);
  delay(2000);
}
```

## 🎯 Learning Outcomes

* Understanding digital output (LED control)
* Using the `tone()` function for sound
* Timing and delays in Arduino
* Basic circuit design

## 📸 Future Improvements

* Sync LED blinking with each note
* Add multiple LEDs
* Create custom melodies
* Integrate sensors for smart alerts

## 🤝 Contributing

Feel free to fork this repo and improve the project!

## 📜 License

This project is open-source and free to use.
LIVE LINK ------> https://wokwi.com/projects/466162003199740929
