# การทดลองที่4 การเขียนโปรแกรมอินพุตสัญญาณดิจิตอล

## วัตถุประสงค์
* 1.ทดสอบการทำงานของโปรแกรมอินพุตสัญญาณดิจิตอล
* 2.ทดสอบการทำงานของเซนเซอร์แสง

## อุปกรณ์
* 1.ไมโครคอนโทรเลอร์ ESP01
* 2.ซีเรียลพอร์ตUSB
* 3.คอมพิวเตอร์
* 4.สายแปลงUSB
* 5.อะแดปเตอร์
* 6.เซ็นเซอร์แสง
* 7.ตัวต้านทาน

## ศึกษาข้อมูลเบื้องต้น
* 1.ศึกษาข้อมูลของไมโครคอนโทรเลอร์ที่ใช้(https://docs.platformio.org/en/latest/boards/espressif8266/esp01_1m.html)
* 2.ศึกษาโค้ดของโปรแกรมที่ต้องการรันบนไมโครคอนโทรเลอร์(https://github.com/choompol-boonmee/lab63b/blob/master/examples/04_Input-Port/src/main.cpp)


## วิธีการทำการทดลอง
* 1.เชื่อมต่อสายแปลงUSBด้านหนึ่งเข้ากับคอมพิวเตอร์และอีกด้านเข้ากับซีเรียล
<img width="383" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 20 24 26" src="https://user-images.githubusercontent.com/80879658/112157248-a083df00-8c19-11eb-939e-3b619d448f6d.png">

* 2.ต่ออะแดปเตอร์เข้ากับซีเรียล
<img width="376" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 18 58 45" src="https://user-images.githubusercontent.com/80879658/112157322-ad083780-8c19-11eb-985d-a7a86c03be7c.png">

* 3.ต่อไมโครคอนโทรเลอร์เข้ากับอะแดปเตอร์
<img width="378" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 18 59 45" src="https://user-images.githubusercontent.com/80879658/112157336-b1345500-8c19-11eb-9692-e132ce1a56ab.png">

* 4.เรียกโฟรเดอร์ที่เราบันทึกโปรแกรมเก็บไว้ โดยในการทดลองนี้โปรแกรมของเราอยู่ในโฟรเดอร์pattani โดยใช้คำสั่ง'cd pattani'
* 5.เรียกโปรแกรมที่เราต้องการ โดยในการทดลองนี้เราจะใช้โปรแกรมที่1ในโฟรเดอร์pattani โดยใช้คำสั่ง'cd 04_Input-Port'
* 6.รันโปรแกรมลงบนไมโครคอนโทรเลอร์ โดยใช้คำสั่ง'pio run -t uplond'
* 7.ขณะรันโปรแกรมให้กดปุ่มสีดำก่อนแล้วกดปุ่มสีแดงบนซีเรียล
* 8.จากนั้นทดสอบโปรแกรมที่รันสำเร็จ โดยใช้คำสั่ง'pio device monitor'
* 9.ทดลองนำสายสีขาว(พอร์ต0)มาสัมผัสกับสายสีดำ(พอร์ต0)และสัมผัสกับสายสีแดง(พอร์ต1)
* 10.ทดลองกดปุ่มสีดำของซีเรียล
* 11.นำเซ็นเซอร์แสงต่อเข้ากับอะแดปเตอร์ โดยต่อขาด้านหนึ่งของตัวต้านทานต่อเข้ากับพอร์ตสายสีแดง นำขาอีกด้านของต้วต้านทานและเซ็นเซอร์แสงต่อเข้ากับพอร์ตตรงกลางระหว่างพอร์ตสายสีแดงและดำ และนำขาอีกด้านของเซ็นเซอร์แสงต่อเข้ากับพอร์ตสายสีดำ(พอร์ต0) และนำสายสีขาวมาต่อเข้ากับพอร์ตที่ทำการต่อขาของตัวต้านทานและเซ็นเซอร์แสง
<img width="384" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 22 04" src="https://user-images.githubusercontent.com/80879658/112157423-c610e880-8c19-11eb-8d62-d71781972eb8.png">

* 12.ทดลองบังแสงที่เซ็นเซอร์และให้แสงกับเซ็นเซอร์


## การบันทึกผลการทดลอง
* เมื่อไมโครคอนโทรเลอร์รันโปรแกรมสำเร็จ ได้ผลดังนี้
<img width="804" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 13 28" src="https://user-images.githubusercontent.com/80879658/112157729-16884600-8c1a-11eb-9c68-db726b0d0fa7.png">
<img width="802" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 14 30" src="https://user-images.githubusercontent.com/80879658/112157746-18eaa000-8c1a-11eb-8d27-6f67944332ec.png">
<img width="800" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 15 27" src="https://user-images.githubusercontent.com/80879658/112157756-1ab46380-8c1a-11eb-9887-a778885f50dd.png">
<img width="802" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 15 54" src="https://user-images.githubusercontent.com/80879658/112157770-1be59080-8c1a-11eb-9bd8-f9059fb80c71.png">

* ผลการทำงานของโปรแกรมที่รันสำเร็จ ได้ผลดังนี้
<img width="1164" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 16 42" src="https://user-images.githubusercontent.com/80879658/112157801-23a53500-8c1a-11eb-8723-ad9fb5b1fae6.png">

* ผลการทดลองนำสายสีขาว(พอร์ต0)มาสัมผัสกับสายสีดำ(พอร์ต0)
<img width="1179" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 18 33" src="https://user-images.githubusercontent.com/80879658/112157815-2869e900-8c1a-11eb-9a55-59a5505776c3.png">

* ผลการทดลองนำสายสีขาว(พอร์ต0)มาสัมผัสกับสายสีแดง(พอร์ต1)
<img width="1183" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 19 28" src="https://user-images.githubusercontent.com/80879658/112157857-328be780-8c1a-11eb-9b03-1749f243ec65.png">

* ผลการทดลองกดปุ่มสีดำของซีเรียล
<img width="1187" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 20 21" src="https://user-images.githubusercontent.com/80879658/112157922-446d8a80-8c1a-11eb-9606-6904850822ee.png">

* ผลการทำงานของเซ็นเซอร์เมื่อบังแสงที่เซ็นเซอร์และให้แสงกับเซ็นเซอร์
<img width="1186" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 23 01" src="https://user-images.githubusercontent.com/80879658/112158003-551e0080-8c1a-11eb-9961-3d71f63e4fba.png">

* ผลการทำงานของเซ็นเซอร์เมื่อให้แสงกับเซ็นเซอร์
<img width="1186" alt="ภาพถ่ายหน้าจอ 2564-03-23 เวลา 19 22 36" src="https://user-images.githubusercontent.com/80879658/112157963-4cc5c580-8c1a-11eb-919e-c705641f3dae.png">

## อภิปรายผลการทดลอง
จากการผลการทดลองแสดงให้เห็นว่าโปรแกรมอินพุตสัญญาณดิจิตอลที่ทำการรันบนไมโครคอนโทรเลอร์สามารถใช้งานได้ จากผลการทดลองจะเห็นว่า เมื่อทำการทดสอบโปรแกรมที่รันสำเร๊จโดยการนำสายสีขาว(พอร์ต0)มาสัมผัสกับสายสีดำ(พอร์ต0)เราจะเห็นไฟLEDสว่างขึ้นและมีสถานะเป็น0 แต่เมื่อนำสายสีขาว(พอร์ต0)มาสัมผัสกับสายสีแดง(พอร์ต1)เราจะไม่เห็นไฟLEDสว่างขึ้นและมีสถานะเป็น1 และเมื่อเรากดปุ่มสีดำบนซีเรียลเราจะเห็นไฟLEDสว่างขึ้นและมีสถานะเป็น0 แต่เมื่อเรากดปุ่มสีแดงบนซีเรียลเราจะไม่เห็นไฟLEDสว่างขึ้นและมีสถานะเป็น1 จากนั้นเมื่อเราทำการต่อเซ็นเซอร์แสงเมื่อเราบังแสงที่เซ็นเซอร์ไฟLEDจะไม่สว่าง แต่เมื่อเราไม่บังแสงที่เซ็นเซอร์ไฟLEDจะสว่างขึ้น เนื่องจากโปรแกรมจะรับอินพุตเข้ามาที่พอร์ต0 เมื่ออินพุตที่รับมามีค่าเป็น1โปรแกรมจะส่งเอาต์พุตLOWไปยังพอร์ต2ทำให้ไฟLEDไม่สว่างขึ้นหรือดับลง แต่เมื่ออินพุตที่รับมามีค่าเท่ากับ0โปรแกรมจะส่งเอาต์พุตHIGHไปยังพอร์ต2ทำให้ไฟLEDสว่างขึ้น

## คำถามหลังการทดลอง
1.เหตุใดเมื่อเราไม่นำสายสีขาวมาสัมผัสกับสายใดๆไฟLEDจึงไม่สว่างขึ้น(เนื่องจากเมื่อเราไม่นำสายสีขาวมาสัมผัสกับสายใดๆค่าอินพุตที่ได้รับจะมีค่าเป็น1)



