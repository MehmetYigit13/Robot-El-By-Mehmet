//Mehmet Yiğit Tarafından Oluşturulmuştur.
//Arduino Robot EL Flex Sensörlü
//Arduino Robot Hand With Flex Sensor
//mehmetyigit135798@gmail.com veya mehmetyigit13579@outlook.com dan ulaşabilirsiniz.


//Servoların Dizilimi
// Servo1(basparmak = 3. Dijital Pin)
// Servo2(isaretparmak = 5. Dijital Pin)
// Servo3(ortaparmak = 6. Dijital Pin)
// Servo4(yuzukparmak = 9. Dijital Pin)
// Servo5(serceparmak = 10. Dijital Pin)

//Flexler sırasıyla A0-A1-A2-A3-A4


//Kütüphaneler



#include <Servo.h> //Servo Kütüphanesini Ekliyoruz.

//Değişkenler
 
const int flex1=A0;
const int flex2=A1;
const int flex3=A2; // Flex Sensörleri Tanıttık
const int flex4=A3;
const int flex5=A4;

 
Servo basparmak;
Servo isaretparmak;
Servo ortaparmak; // Servoları Tanıttık
Servo yuzukparmak;
Servo serceparmak;

 
int flexdurum1=0;
int flexdurum2=0;
int flexdurum3=0; //Flex Sensörlerin Durumunu Belirledik
int flexdurum4=0;
int flexdurum5=0;

 
int pos1=0;
int pos2=0;
int pos3=0; //Servoların Posizyonunu Belirledik
int pos4=0; 
int pos5=0;


 //Robot Elin Setup Kısmı
void setup() {
 
servo1.attach(3);
servo2.attach(5);
servo3.attach(6); //Servoları Başlattık
servo4.attach(9);
servo5.attach(10);
 
}

//Robot Elin Loop Kısmı
 
void loop() {
 

//Robot Elin Çalışma Prensipleri burada aslında.
//burda map komutunu ele aldık basparmakı örnek olarak açıklayalım

 
flexdurum1=analogRead(flex1); // flex1 den gelen verileri flexdurum1 adlı değişkene kaydettik
 
pos1=map(flexdurum1,0,1023,0,180); //pos pozisyon demek bunu biz oluşturduk map komutu şöyle işler map(değişkenimiz,en küçükten.en büyükten.en küçüğe,en büyüğe) yani 0 ila 180 arasında bir değer aldık 
 
{
 
  basparmak.write(pos1);// pos1 deki değeri yukarda hesapladık ve basparmak adlı servoya yazdırdık.
 
}
 
flexdurum2=analogRead(flex2);
 
pos2=map(flexdurum2,0,1023,0,180);
 
{
 
  isaretparmak.write(pos2);
 
}
 
flexdurum3=analogRead(flex3);
 
pos3=map(flexdurum3,0,1023,0,180);
 
{
 
  ortaparmak.write(pos3);
 
}
 
flexdurum4=analogRead(flex4);
 
pos4=map(flexdurum4,0,1023,0,180);
 
{
 
  yuzukparmak.write(pos4);
 
}
 
flexdurum5=analogRead(flex5);
 
pos5=map(flexdurum5,0,1023,0,180);
 
{
 
  serceparmak.write(pos5);
 
}
 
}
