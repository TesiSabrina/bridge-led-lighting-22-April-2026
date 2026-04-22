__**# bridge-led-lighting-22-April-2026**__

A program to light three leds using an Arduino uno , a breadboard,three resitors, a pushbutton, power cable and wires.
The code used was:

int LED1=7;

int LED2=6;

int LED3=5;

int pushbutton=2;

void setup()

{
 pinMode(2,INPUT); 
 
 pinMode(7,OUTPUT);
 
 pinMode(6,OUTPUT);
 
 pinMode(5,OUTPUT);
}

void loop()
{ 
  int buttonState=digitalRead(pushbutton);
  
    if(buttonState==HIGH){
    
    digitalWrite(LED1, HIGH);
    
    digitalWrite(LED2, HIGH);
    
    digitalWrite(LED3, HIGH);
    
  } 
  else{
    digitalWrite(LED1, LOW);
    
    digitalWrite(LED2, LOW);
    
    digitalWrite(LED3, LOW);
    
  }
}

