# Arduino-HC-05-interface-code
interafced android phone with arduino
code=
#define leftmotorfwd 8
#define rightmotorfwd 5
#define leftmotorrev 2
#define rightmotorrev 4
#define liftmotorfwd 7
#define liftmotorrev 12
#define basearmmotorfwd A0
#define basearmmotorrev A1
#define higharmmotorfwd A2
#define higharmmotorrev A3
#define clawmotorfwd A4
#define clawmotorrev A5
void setup() {
  // put your setup code here, to run once:
Serial.begin(9600);
pinMode(leftmotorfwd,OUTPUT);
pinMode(leftmotorrev,OUTPUT);
pinMode(rightmotorfwd,OUTPUT);
pinMode(rightmotorrev,OUTPUT);
pinMode(liftmotorfwd,OUTPUT);
pinMode(liftmotorrev,OUTPUT);
pinMode(basearmmotorfwd,OUTPUT);
pinMode(basearmmotorrev,OUTPUT);
pinMode(higharmmotorfwd,OUTPUT);
pinMode(higharmmotorrev,OUTPUT);
pinMode(clawmotorfwd,OUTPUT);
pinMode(clawmotorrev,OUTPUT);
Serial.println("Connection Successful!");
}
void moveforward()
{
  digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,HIGH);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,HIGH);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void movebackward()
{

  digitalWrite(leftmotorrev,HIGH);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void moveright()
{
   digitalWrite(leftmotorrev,LOW);
 digitalWrite(leftmotorfwd,HIGH);
  digitalWrite(rightmotorrev,HIGH);
 digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void moveleft()
{
   digitalWrite(leftmotorrev,HIGH);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,HIGH);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void liftup()
{
   digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,HIGH);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void liftdown()
{
   digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,HIGH);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void barmup()
{
digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,HIGH);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void barmdown()
{
  digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,HIGH);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void uarmup()
{
  digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,HIGH);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void uarmdown()
{
  digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,HIGH);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}
void clawin()
{
  digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,HIGH);
digitalWrite(clawmotorrev,LOW);
}
void clawout()
{
  digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,HIGH);
}
void movestop()
{
digitalWrite(leftmotorrev,LOW);
  digitalWrite(leftmotorfwd,LOW);
  digitalWrite(rightmotorrev,LOW);
  digitalWrite(rightmotorfwd,LOW);  
digitalWrite(liftmotorfwd,LOW);
digitalWrite(liftmotorrev,LOW);
digitalWrite(basearmmotorfwd,LOW);
digitalWrite(basearmmotorrev,LOW);
digitalWrite(higharmmotorfwd,LOW);
digitalWrite(higharmmotorrev,LOW);
digitalWrite(clawmotorfwd,LOW);
digitalWrite(clawmotorrev,LOW);
}

void loop() {
  // put your main code here, to run repeatedly:
if(Serial.available()>0)
{
  int data = Serial.read();
  switch(data)
  {
    case 'F' : moveforward(); break;
    case 'B' : movebackward(); break;
    case 'R' : moveright(); break;
    case 'L' : moveleft(); break;
    case 'N' : liftup(); break;
    case 'n' : liftdown(); break;
    case 'x' : barmup(); break;
    case 'X' : barmdown(); break;
    case 'I' : uarmup(); break;
    case 'J' : uarmdown(); break;
    case 'G' : clawin(); break;
    case 'H' : clawout(); break;
    case 'S' : movestop(); break;
 
    default : break;
  }
}
}
