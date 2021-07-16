# arduino-experience
it can help you to learn arduino 
const int ledPin = 2;//定义LED正极接Arduino的2号引脚
void setup () {
pinMode (ledPin，OUTPUT);//将单片机的2号引脚设置为输出模式oUTPUT}
void loop () {
digitalwrite (ledPin,HIGH);//将单片机的2号引脚置于高电平（亮)delay(500); //持续5oo毫秒,也就是o.5秒
digitalwrite (ledPin，LOW);//将单片机的2号引脚置于低电平（灭)delay (500); //持续5oo毫秒，也就是o.5秒
}
