# 🖊️ Pen Factory & Writing Instruments

A Java-based project demonstrating core Object-Oriented Design Patterns through a real-world pen system.

## 🚀 Features
- Factory Method Pattern → Creating different types of pens  
- Inheritance & Abstraction → Shared behaviour via base class  
- Decorator Pattern → Adding grip dynamically  
- State Management → start, write, close lifecycle  
- Exception Handling → Robust validation  

## 📁 Project Structure

pen-factory-writing-instruments  
└── src  
&ensp;&ensp;└── main  
&ensp;&ensp;&ensp;&ensp;└── java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;└── pen  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── WritingInstrument.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── Pen.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── BallPen.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── GelPen.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── FountainPen.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── GripPenDecorator.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;├── PenFactory.java  
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;└── PenDemo.java  


## 🧩 Core Components

### WritingInstrument
Defines methods:
- start()
- write(String s)
- close()
- refill(String color)

### Pen (Abstract Class)
- Common attributes like type, color, inkLevel (100)
- Handles start, write, close, refill logic

## ✒️ Pen Types
- BallPen → basic pen  
- GelPen → smooth writing  
- FountainPen → uses more ink & limited refill colors  

## 🎯 Decorator
GripPenDecorator adds:
- Extra grip message while writing  

## 🏭 Factory
PenFactory.getPen(type, color, hasCap, hasClip)

## ▶️ Run Instructions

Compile:
javac -d out src/main/java/pen/*.java

Run:
java -cp out pen.PenDemo
