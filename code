#include <LiquidCrystal.h>  
int Contrast=0;
int contrast_pin6 = 6;
int backlight_pin9= 9;
int brightness =128;
int button1 =10;
int button2 = 8;
int buttonState =0;
int buttonState2= 0;
int screenState=0;
int value1= 0;
int value2 = 0;
int column = 0;
int binarynumber= 0;

int lastButtonState1 = LOW;
int lastButtonState2 = LOW;
int buttonStatedo1;
int buttonStatedo2;
unsigned long lastDebounceTime = 0;
unsigned long debounceDelay = 50;
    
    int x11= 0;
    int x12= 0;
    int x13= 0;
    int x14= 0;
    int x15= 0;
    int x16= 0;
    int x17= 0;
    int x18= 0;
    int x21= 0;
    int x22= 0;
    int x23= 0;
    int x24= 0;
    int x25= 0;
    int x26= 0;
    int x27= 0;
    int x28= 0;
    int x31= 0;
    int x32= 0;
    int x33= 0;
    int x34= 0;
    int x35= 0;
    int x36= 0;
    int x37= 0;
    int x38= 0;
    int x39= 0;
    int x40= 0;

 LiquidCrystal lcd(12, 11, 5, 4, 3, 2);   
 void setup()
 { 
    analogWrite(contrast_pin6,Contrast);
     lcd.begin(16, 2);
     lcd.setCursor (0,0);
     lcd.print("Click Both");
     lcd.setCursor (0,1);
     lcd.print("Buttons 2 Adv");
     pinMode(backlight_pin9,OUTPUT);
     pinMode(button1,INPUT);
     pinMode(contrast_pin6,OUTPUT);
     pinMode(button2,INPUT);
     Serial.begin(9600);
  }  
     void loop()
 {  
    analogWrite(backlight_pin9,brightness);  // PWM values from 0 to 255 (0% â€“ 100% duty cycle)
    analogWrite(contrast_pin6,Contrast);
buttonState = digitalRead(button1);
buttonState2 = digitalRead(button2);

if(buttonState != lastButtonState1 && buttonState2 != lastButtonState2 || buttonState2 != lastButtonState2 ||buttonState != lastButtonState1){
  lastDebounceTime = millis();
  }
  if ((millis() - lastDebounceTime) > debounceDelay){
    
    if(buttonState != buttonStatedo1  || buttonState2 != buttonStatedo2){
      buttonStatedo1 = buttonState;
      buttonStatedo2 = buttonState2;
      if (buttonStatedo1 == HIGH ||buttonStatedo2 ==HIGH){
        mainprogram();
        }
      
      }
    }
    lastButtonState1 = buttonState;
    lastButtonState2 = buttonState2;
}
void mainprogram(){
if(screenState == 4 && buttonState2 == HIGH && buttonState == HIGH){//switch screen 5
  screenState =0;
    x11= 0;
    x12= 0;
    x13= 0;
    x14= 0;
    x15= 0;
    x16= 0;
    x17= 0;
    x18= 0;
    x21= 0;
    x22= 0;
    x23= 0;
    x24= 0;
    x25= 0;
    x26= 0;
    x27= 0;
    x28= 0;
    x31= 0;
    x32= 0;
    x33= 0;
    x34= 0;
    x35= 0;
    x36= 0;
    x37= 0;
    x38= 0;
    x39= 0;
    x40= 0;
  lcd.clear();
  lcd.print("Click Both");
  lcd.setCursor (0,1);
  lcd.print("Buttons 2 Adv");
  lcd.noCursor();
  return;
  
  }
if(screenState == 4){//begining of brightness
if (brightness == 256)
{
brightness = 0;
}

if (buttonState == HIGH)
{
brightness = brightness + 32;

}
if (buttonState2 == HIGH)
{
  if(Contrast >= 100){
    Contrast = 0;
    }
  else{  
  Contrast = Contrast + 10;
  }
}
}//end screen 5
if(screenState == 3 && buttonState2 == HIGH && buttonState == HIGH){//switch screen 4
  screenState =4;
  lcd.clear();
  lcd.print("R-Brightnerr");
  lcd.setCursor (0,1);
  lcd.print("L-Contrast");
  lcd.noCursor();
  
  }
if(screenState == 3){

  
  
if(buttonState == HIGH){
  lcd.clear();
  lcd.print("Solution R-B L-D");
  lcd.setCursor(0,1);
  lcd.print(x39);
  lcd.print(x38);
  lcd.print(x37);
  lcd.print(x36);
  lcd.print(x35);
  lcd.print(x34);
  lcd.print(x33);
  lcd.print(x32);
  lcd.print(x31);
  lcd.noCursor();
  }
if(buttonState2 == HIGH){
  lcd.clear();
  lcd.print("Solution R-B L-D");
  lcd.setCursor(0,1);
  lcd.print(x40);
  
  }
}//end screen 4
if(screenState == 2 && buttonState2 == HIGH && buttonState == HIGH){//switch screen 3
  screenState =3;
  lcd.clear();
  lcd.print("Solution R-B L-D");
  lcd.setCursor(0,1);

   x31 = x21 + x11;
   if(x31>=2){
    x31= x31-2;
   x12= x12+1;
    }
    x32 = x22 + x12;
   if(x32>=2){
    x32= x32-2;
   x13= x13+1;
    }
    x33 = x23 + x13;
   if(x33>=2){
    x33= x33-2;
   x14= x14+1;
    }
    x34 = x24 + x14;
   if(x34>=2){
    x34= x34-2;
   x15= x15+1;
    }
    x35 = x25 + x15;
   if(x35>=2){
    x35= x35-2;
   x16= x16+1;
    }
    x36 = x26 + x16;
   if(x36>=2){
    x36= x36-2;
   x17= x17+1;
    }
    x37 = x27 + x17;
   if(x37>=2){
    x37= x37-2;
   x18= x18+1;
    }
    x38 = x28 + x18;
   if(x38>=2){
    x38= x38-2;
   x39= x39+1;
    }
    x40= 1*x31 +2*x32 + 4*x33 + 8*x34 + 16*x35 + 32*x36 + 64*x37 + 128*x38 + 256 *x39;
  lcd.print(x39);
  lcd.print(x38);
  lcd.print(x37);
  lcd.print(x36);
  lcd.print(x35);
  lcd.print(x34);
  lcd.print(x33);
  lcd.print(x32);
  lcd.print(x31);
  lcd.noCursor();
  }
if(screenState == 2){
if(buttonState == HIGH){
  if(column < 8){
    binarynumber=0;
    column++;
    lcd.setCursor(column,1);
    lcd.cursor();
    }
  else{
    column=1;
    lcd.setCursor(column,1);
    lcd.cursor();
    }      
  }
if(buttonState2 == HIGH){
    if (binarynumber==0){
    binarynumber =1;
    }else{binarynumber=0;}
    if (column==1){x28= binarynumber;}
    if (column==2){x27= binarynumber;}
    if (column==3){x26= binarynumber;}
    if (column==4){x25= binarynumber;}
    if (column==5){x24= binarynumber;}
    if (column==6){x23= binarynumber;}
    if (column==7){x22= binarynumber;}
    if (column==8){x21= binarynumber;}
   lcd.print(binarynumber);
   lcd.setCursor(column,1);
  }
}//end screen 3
if(screenState == 1 && buttonState2 == HIGH && buttonState == HIGH){//switch screen 2
  screenState =2;
  lcd.clear();
  lcd.print("2nd Binarynumber");
  column=1;
  lcd.setCursor(column,1);
  lcd.print("00000000");
  lcd.setCursor(column,1);
  }
if(screenState == 1){
if(buttonState == HIGH){
   binarynumber=0;
  if(column < 8){
    column++;
    lcd.setCursor(column,1);
    lcd.cursor();
    }
  else{
    column=1;
    lcd.setCursor(column,1);
    lcd.cursor();
    }      
  }
if(buttonState2 == HIGH){
    if (binarynumber==0){
    binarynumber =1;
    }else{binarynumber=0;}
    if (column==1){x18= binarynumber;}
    if (column==2){x17= binarynumber;}
    if (column==3){x16= binarynumber;}
    if (column==4){x15= binarynumber;}
    if (column==5){x14= binarynumber;}
    if (column==6){x13= binarynumber;}
    if (column==7){x12= binarynumber;}
    if (column==8){x11= binarynumber;}
   lcd.print(binarynumber);
   lcd.setCursor(column,1);
  }
}//end screen 2
if(screenState ==0 &&buttonState2==HIGH && buttonState==HIGH){//switch screen 1
  screenState =1;
  lcd.clear();
  lcd.print("1st Binarynumber");
  column = 1;
  lcd.cursor();
  lcd.setCursor(column,1);
  lcd.print("00000000");
  lcd.setCursor(column,1);
  }//end switch Screen 1
if(screenState == 0){//begining of brightness
if (brightness == 256)
{
brightness = 0;
}

if (buttonState == HIGH)
{
brightness = brightness + 32;

}
if (buttonState2 == HIGH)
{
  if(Contrast >= 100){
    Contrast = 0;
    }
  else{  
  Contrast = Contrast + 10;
  }
}
}//end of brightness &  Contrast
}
