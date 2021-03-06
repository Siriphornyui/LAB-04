#ใบงานที่ 4
เรื่อง การใช้งานคำสั่งเกี่ยวกับการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C#
##วัตถุประสงค์
1. เพื่อให้นักศึกษาบอกชื่อ method ที่ใช้ในการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C# ได้
2. เพื่อให้นักศึกษาสามารถใช้คำสั่งแสดงผลทางหน้าจอ เบื้องต้นได้

##ลำดับขั้นการทดลอง
###การเตรียมการก่อนการทดลอง
  * เปิดโปรแกรม Visual Studio 
  *  เลือก File >>New Project >> เลือก Console Application 
![P1](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P1.png)
  *  ช่อง Name ใส่ชื่อของ project (ในที่นี้คือ Lab4)
  *  ช่อง Location ใส่ชื่อ folder ที่เป็นที่ตั้งของ Project (ในที่นี้ สมมติเป็น E:\vslab)
  *  ช่อง Solution name ให้ใส่ชื่อ Solution โดยปกติก็ให้ปล่อยไว้อย่างนั้น 
  *  กดปุ่ม OK โปรแกรม Visual Studio จะสร้าง project ชื่อ “lab4”ภายใต้ solution “lab4” และไฟล์ lsb4.cs ซึ่งมี source code ดังรูป 

![P2](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P2.png)

ส่วนสำคัญของโปรแกรม lab4.cs  คือบรรทัดที่ 1 “using System” และเมธอด Main(string[] args)


 *  ให้ลบ source code ในบรรทัดที่ 2-5 ออกไปก่อน เนื่องจากเป็น assembly ที่ไม่จำเป็นต่อการทำงานของโปรแกรม 

## 1. การทดลองเมดธอด Console.Write()
* ให้เพิ่ม บรรทัดต่อไปนี้ลงไปในในเมธอด Main()
```csharp 
    Console.Write(“Hello”);
```
ดังปรากฏในบรรทัดที่ 9 ของรูปด้านล่าง 

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P3.png)
 
 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

####บันทึกผลการทดลอง
<hr>จากการทดลองโปรแกรมจะแสดงผล 

<img src= "https://github.com/Siriphornyui/LAB-04/blob/master/41.jpg">
<hr>

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้    

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P4.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
<hr>จากการทดลองโปรแกรมจะแสดงผล 

 <img src = "https://github.com/Siriphornyui/LAB-04/blob/master/42.jpg">
<hr>


### คำถาม 4.1 

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย
<hr>
คิดว่าผลของข้อมูลที่แสดงออกมาของคำสั่ง Console.Write("") เป็นการแสดงเฉพาะข้อมูลที่อยู่ใน ("") ซึ่งเป็นไปตามที่คิดไว้
แต่มีมีสองคำสั่งต่อกัน ผลของข้อมูลที่แสดงออกมาไม่ได้เป็นไปตามที่คิดไว้ ซึ่งคิดว่าผลจะออกมา hello กับ Word คนละบรรทัดกัน
<hr>


## 2. การทดลองเมดธอด Console.WriteLine()

แก้โปรแกรมในเมดธอด Main() ให้เป็นดังรูปต่อไปนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P5.png)

 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

บันทึกผลที่ได้จากการรันโปรแกรม
<hr>
<hr>จากการทดลองโปรแกรมจะแสดงผล 

<img src= "https://github.com/Siriphornyui/LAB-04/blob/master/41.jpg">
<hr>

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P6.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
<hr>
จากการทดลองโปรแกรมจะแสดงผล

<img src = "https://github.com/Siriphornyui/LAB-04/blob/master/43.jpg">
<hr>

###คำถาม 4.2

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย
<hr>
 ผลการทดลองคำสั่ง   Console.WriteLine(""); 1 หรือ 2 คำสั่งเป็นไปอย่างที่ คิดไว้
<hr>

### คำถาม 4.3 

จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()
<hr>
Console.Write() ถ้ามีคำสั่งนี้ต่อกันหลายๆคำสั่ง ข้อความที่อยู่ใน ("") เมื่อแสดงผลออกมาข้อความจะยาวต่อกัน

Console.WriteLine() คำสั่งนี้จะแสดงผลตามข้อความที่อยู่ ("") แต่เมื่อมีคำสั่งนี้ต่อกันหลายๆบรรทัด

ผลที่แสดงออกมาข้อความจะไม่ยาวติดกัน จะแสดงผล Console.WriteLine() ต่อ 1 บรรทัด
<hr>

##สรุปผลการทดลอง

<hr>
 Console.Write() และ Console.WriteLine() เป็นคำสั่งที่ใช้ในการแสดงผลข้อความออกมา
 
สามารถเลือกใช้ในกรณีที่แตกต่างกันออกไป
<hr>

