#include <SoftwareSerial.h>
#include <SPI.h>
#include <MFRC522.h>
#include <Wire.h>
#include <Servo.h>
Servo servoMain;
#include<LiquidCrystal_I2C.h>
LiquidCrystal_I2C lcd(0x3F, 16, 2);
#define SS_PIN 10
#define RST_PIN 9
MFRC522 mfrc522(SS_PIN, RST_PIN);
String page = "";
char input[12];
int count = 0;
int a = 5;
int pl = 0, p2 = 0, p3 = 0, p4 = 0, p5 = 0, p6 = o, p7 = 0, p8 = 0;
int cl = 0, c2 = 0, c3 = 0, c4 = 0, c5 = 0, c6 = 0, c7 = 0, c8 = 0;
double total = 0;
int led1 = 15;
int led2 = 14;
int buzzer = 16;
int state;

void setup()
{
  SPI.begin();
  mfrc522.PCD_Init();
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(buzzer, OUTPUT);
  pinMode(a, INPUT_PULLUP)
  pinMode(6, INPUT);
  servoMain.attach(4);
  Serial.begin(115200);
  Serial.begin(9600);
  Serial.printin();

  lcd.init();
  lcd.backlight();
  lcd.clear()
  lcd.setCursor(0, 0);
  lcd.print("GROUP 1");
  lcd.setCursor(0, 0);
  lcd.print("SMART TROLLEY");
  delay(2000)
  lcd.clear();
  lcd.setCursor(0, 0);
  lcd.print("  PLZ ADD ITEM");
  lcd.setCursor(0, 1);
  lcd.print("    TO CART");
  delay(2000);
  servoMain.write(0);


  
}
void loop()
{
  int status ;
  int a = digitalRead(5);
  state = digitalRead(6);
  if (state == 1)
  {

    lcd.clear();
    lcd.setCursor(0, 0);
    lcd.print("Total Price :-");
    lcd.setCursor(0, 1);
    lcd.print(total);
    delay(5000);
    lcd.clear();
    lcd.setCursor(0, 0);
    lcd.print("  THANKS FOR  ");
    lcd.setCursor(0, 1);
    lcd.print("  VISTING  ");
    Serial.println(total);
    Serial.println("message sent.");
    delay(2000);


    
  }
  else {
    delay(10);
  }
  if ( ! mfrc522.PICC_IsNewCardPresent())
  {
    return;
  }

  else if ((content.substring(1) == "4D 80 8D 37") && (a == 1))
  {
    lcd.clear();
    Serial.println("lays added");
    lcd.setCursor(0, 1);
    lcd.print("price(Rs):120.00");
    total = total + 120.00;
    digitalWrite(led1, HIGH);
    digitalWrite(buzzer, HIGH);
    delay(2000);
    p2++;
    count_prod++;
    digitalWrite(led1, LOW);
    digitalWrite(buzzer, LOW);
    servoMain.write(0);

  }

  else if ((content.substring(1) == "4D 80 8D 37") && (a == 0)) {
    if (p2 > 0)
    {
      lcd.clear();
      Serial.println("
    }
    
  }
}
