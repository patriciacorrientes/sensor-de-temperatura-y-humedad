# sensor-de-temperatura-y-humedad
proyect

#include <DHT11.h> //cargamos la librería DHT
int pin=2; //Seleccionamos el pin en el que se //conectará el sensor
DHT11 dht11(pin); //Se selecciona el DHT11 (hay //otros DHT)
 
void setup()
Serial.begin(9600); //Se inicia la comunicación serial

void loop() {
float temp, hum;   

void loop() {
float temp, hum;   
int err;
if((err=dht11.read(hum, temp))==0
    Serial.print("Temperatura: ");
    Serial.print(temp);
    Serial.print(" Humedad: ");
    Serial.print(hum);
    Serial.println();
  }
       else
          {
             Serial.println();
             Serial.print("Error Num :");
             Serial.print(err);
             Serial.println();
          }
          delay(1000); 
}
}
