@snap[north span-100 text-white]
### Docker คืออะไร  
@snapend

@snap[west span-50]
**Docker** มันก็คือ Virtualization อย่างนึง โดยมันจะสร้าง Containers เพื่อจำลองสภาพแวดล้อมการทำงานอยู่บนระดับ OS เลย ซึ่งจะต่างกับ VMs ที่ต้องจำลอง Guest OS โดยใช้ Hypervisor (VMware, Virtual Box) ขึ้นมาก่อน  
@snapend

@snap[east span-50]
![](assets/img/1_hmLHrf5_STV98PvOr2ydzA.png)
@snapend

#HSLIDE

### ข้อดีของ Docker เมื่อเทียบกับ VMs  

1. Docker ไม่ต้องเสียเวลาในสร้าง OS ใหม่ และการ config แต่ละ OS เลย
2. Docker เบาและเร็วกว่ามาก ไม่ว่าจะเป็น start stop และ restart เพราะมันใช้ OS, CPU และ RAM ร่วมกันกับ Host OS
3. Docker สามารถรัน container ได้มากกว่า VMs ในเครื่องที่มีทรัพยากรที่เท่ากัน
4. Docker มีระบบ Registry ทำให้สามารถเคลื่อนย้าย หรือติดตั้ง Container ได้สะดวก และรวดเร็วกว่ามาก
5. Containers มันรันอยู่บน Docker Engine ทำให้ไม่ต้องสนใจว่า Infrastructure หรือ Host OS ว่าจะเป็นอะไรยังไง ทำให้หมดปัญหาว่าเครื่อง Dev รันได้ แต่เครื่อง Production มันรันไม่ได้บ้าง หรือเครื่อง Dev แต่ละคนติดตั้งเครื่องมือคนละเวอร์ชันกัน เราก็ build container เป็น image แล้วส่งในคนในทีมใช้ ก็หมดปัญหาแล้ว
