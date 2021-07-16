# arduino-experience
Use a potentiometer to control the steering gear
#include <Servo.h>//导入arduino函数库

Servo myservo1;//设定舵机
int val1;//设定变量

void setup()
{
  myservo1.attach(9);//舵机连9端口（你连的是几端口就attach几）
}

void loop()
{
  val1=analogRead(A0);//电位器连的端口赋值给变量
  val1=map(val1,0,1023,0,180);//map函数映射，模拟取值范围，把电位器区间映射到角度
  myservo1.write(val1);//舵机依靠变量旋转相应角度

  delay(5);//延时
}
