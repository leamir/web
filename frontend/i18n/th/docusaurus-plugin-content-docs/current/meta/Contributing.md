---
title: การมีส่วนร่วม
sidebar_label: การมีส่วนร่วม
description: วิธีการมีส่วนร่วมกับเอกสาร SA-MP Wiki และ open.mp
---

แหล่งที่มาของเอกสารนี้เปิดให้ทุกคนมีส่วนร่วมในการ เปลี่ยนแปลง!! พวกคุณ ต้องมีบัญชี [GitHub](https://github.com) และเวลาว่างสักเล็กน้อย คุณไม่จำเป็นต้องรู้ เกี่ยวกับ Git ด้วยซ้ำ คุณสามารถทำได้ทั้งหมดจากหน้าเว็บ!

## การแก้ไขเนื้อหา

ในแต่ละหน้า มีปุ่มที่จะพาคุณไปยังหน้า Github เพื่อทำการแก้ไข:

![มีลิงค์อยู่ในแต่ละหน้า Wiki เขียนว่า Edit this page](https://assets.open.mp/assets/images/contributing/edit-this-page.png)

ยกตัวอย่างเช่น คลิกไปที่ [SetVehicleAngularVelocity](../scripting/functions/SetVehicleAngularVelocity) มันจะพาคุณไป [หน้านี้](https://github.com/openmultiplayer/web/edit/master/docs/scripting/functions/SetVehicleAngularVelocity.md) ซึ่งจะแสดงเครื่องมือในการแก้ไขข้อความเพื่อทำการเปลี่ยนแปลง ไฟล์ (สมมติหาก คุณเข้าสู่ระบบ Github)

ทำการแก้ไขในส่วนของคุณและส่ง "Pull Request" ซึ่งหมายถึงผู้ดูแล Wiki และ สมาชิกคอมมูนิตี้คนอื่น ๆ สามารถตรวจสอบการเปลี่ยนแปลงของคุณ และพูดคุยกันว่ามันจำเป็น หรือไม่กับการเปลี่ยนแปลงนี้แล้วรวมเข้าด้วยกัน

## การเพิ่มเนื้อหาใหม่

การเพิ่มเนื้อหาใหม่มีอาจมีความยุ่งยากเล็กน้อย คุณสามารถทำได้สองวิธี:

### หน้าอินเตอร์เฟซของ GitHub

เมื่อเรียกดูไดเรกทอรีบน GitHub จะมีปุ่ม Add file อยู่ด้านบน มุมขวาของรายการไฟล์:

![ปุ่ม Add file](https://assets.open.mp/assets/images/contributing/add-new-file.png)

คุณสามารถอัปโหลดไฟล์ Markdown ที่คุณเขียนไว้แล้วหรือเขียนมันโดยตรงผ่านเครื่องมือแก้ไขข้อความของ Github

ไฟล์ _ควร_ มีสกุล `.md` และมี Markdown สำหรับข้อมูลเพิ่มเติม เกี่ยวกับ Markdown ลองดูที่ [คู่มือนี้](https://guides.github.com/features/mastering-markdown/)

เมื่อเสร็จแล้วให้กด "Propose new file" จากนั้น Pull Request จะเปิดขึ้นมาเพื่อ ตรวจสอบ

### Git

หากต้องการใช้ Git สิ่งที่คุณต้องทำคือโคลนที่เก็บ Wiki ด้วย:

```sh
git clone https://github.com/openmultiplayer/wiki.git
```

เปิดมันด้วยเครื่องมือแก้ไขไฟล์ที่คุณชอบ ผมแนะนำให้ใช้ Visual Studio Code เพราะมันมี เครื่องมือดี ๆ สำหรับการแก้ไขและจัดรูปแบบไฟล์ Markdown อย่างที่คุณเห็น ผม เขียนมันด้วย Visual Studio Code!

![ภาพตัวอย่าง Markdown จาก Visual Studio Code](https://assets.open.mp/assets/images/contributing/vscode.png)

ผมแนะนำให้ใช้ส่วนขยายสองตัวนี้เพื่อเพิ่มประสบการณ์ของคุณให้ดียิ่งขึ้น:

- [markdownlint](https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint) โดย David Anson - นี่คือส่วนขยายที่ทำให้แน่ใจว่า Markdown ของคุณ มีรูปแบบที่ถูกต้อง มันป้องกันความผิดพลาดทางไวยากรณ์และความหมาย ไม่ใช่ คำเตือนทั้งหมดจะมีความสำคัญ แต่บางคำเตือนสามารถช่วยปรับปรุงความสามารถในการอ่านได้ ใช้ วิจารณญาณที่ดีที่สุด และหากมีข้อสงสัยเพียงแค่ถามผู้วิจารณ์!
- [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) โดยทีม Prettier.js - นี่คือตัวที่สามารถจัดรูปแบบไฟล์ Markdown ของคุณโดยอัตโนมัติ ดังนั้นพวกเขา ใช้สไตล์ที่สอดค้ลองกัน ก็คือที่เก็บ Wiki มีการตั้งค่าบางอย่างใน `package.json` ที่ส่วนขยายนี้เรียกใช้โดยอัตโนมัติ อย่าลืมเปิดใช้งาน "Format On Save" ในการตั้งค่าตัวแก้ไขเพื่อให้ไฟล์ Markdown ของคุณได้รับการจัดรูปแบบโดยอัตโนมัติทุกครั้งที่คุณบันทึก!

## บันทึก เคล็ดลับ และกระบวนการ

### ลิงค์ภายใน

อย่าใช้ URL แบบเต็มสำหรับการเชื่อมต่อภายในเว็บไซต์เดียวกัน ใช้เส้นทางที่อยู่ในเครือเดียวกัน

- ❌

  ```md
  ใช้กับ [OnPlayerClickPlayer](https://www.open.mp/docs/scripting/callbacks/OnPlayerClickPlayer)
  ```

- ✔

  ```md
  ใช้กับ [OnPlayerClickPlayer](../callbacks/OnPlayerClickPlayer)
  ```

`../` ความหมายคือ "ย้อนกลับไปหนึ่งไดเรกทอรี" ดังนั้นหากไฟล์ที่คุณกำลังแก้ไขอยู่ใน ไดเรกทอรี `functions` และคุณจะเชื่อมต่อไปหา `callbacks` คุณสามารถใช้ `../` เพื่อกลับไป ยัง `scripting/` จากนั้นก็ `callbacks/` เพื่อเข้าไปยังไดเรกทอรีของ callbacks จากนั้น ชื่อไฟล์ callback (ไม่มี `.md`) ที่คุณต้องการเชื่อมต่อ

### รูปภาพ

รูปภาพจะอยู่ในไดเร็กทอรีย่อยด้านใน `/static/images` จากนั้นเมื่อคุณต้องการโยงไฟล์ รูปภาพใน `![]()` คุณแค่ใช้ `/images/` เป็นฐาน (ไม่จำเป็นต้อง `static` นั้นเป็นเส้นทางสำหรับที่เก็บ)

หากมีข้อสงสัย โปรดอ่านหน้าอื่นที่ใช้รูปภาพเหมือนกันและก๊อปปี้วิธีการทำที่นั้นมาได้เลย

### Metadata

สิ่งแรกในเอกสาร _ใด ๆ_ ที่นี่ควรเป็น metadata: (Metadata หมายถึงข้อมูลที่อธิบายถึงความเป็นมาของข้อมูลนั้น ๆ)

```mdx
---
title: เอกสารของฉัน
sidebar_label: เอกสารของฉัน
description: นี่คือหน้าเกี่ยวกับทีมงานและอะไรบางอย่างเกี่ยวกับอากะตะ
---
```

ทุก ๆ หน้าควรมี title และ description

สำหรับรายการแบบเต็มว่าใช้อะไรได้บ้างในระหว่าง `---` ลองดูที่ [เอกสาร Docusaurus](https://docusaurus.io/docs/markdown-features#markdown-headers).

### หัวเรื่อง

อย่าสร้างหัวข้อระดับ 1 (`<h1>`) ด้วย `#` ซึ่งมันจะสร้างขึ้น โดยอัตโนมัติ หัวข้อแรกของคุณ _ทุกครั้ง_ ควรเป็น `##`

- ❌

  ```md
  # หัวข้อของฉัน

  เอกสารนี้เกี่ยวกับ ...

  # หัวข้อย่อย
  ```

- ✔

  ```md
  เอกสารนี้เกี่ยวกับ ...

  ## หัวข้อย่อย
  ```

### ใช้ `โค้ด` สำหรับการอ้างอิงทางเทคนิค

เมื่อเขียนย่อหน้าที่มี ชื่อฟังก์ชัน, ตัวเลข, นิพจน์ หรืออะไรก็ตามที่ไม่ใช่ภาษาเขียนมาตรฐานให้ล้อมรอบด้วย \`pBongWeed\` แบบนี้ ทำให้ง่ายต่อการแยกภาษาสำหรับอธิบายสิ่งต่าง ๆ จากการอ้างอิงถึงองค์ประกอบทางเทคนิคเช่น ชื่อฟังก์ชั่น และส่วนของโค้ด

- ❌

  > ฟังก์ชั่น fopen จะส่งค่ากลับมาพร้อมแท็กประเภท File: มันไม่มี ปัญหาอะไรในบรรทัดนั้นเนื่องจากค่าส่งกลับจะถูกเก็บไว้ในตัวแปรนั้นพร้อม แท็กประเภท File: (กรณีนี้ก็เช่นกัน) อย่างไรก็ตามใน บรรทัดถัดไปค่า 4 ได้ถูกเพิ่มเข้าไปในตัวควบคุมไฟล์ 4 ไม่มีแท็ก [...]

- ✔

  > ฟังก์ชั่น `fopen` จะส่งค่ากลับมาพร้อมแท็กประเภท `File:` มัน ปัญหาอะไรในบรรทัดนั้นเนื่องจากค่าส่งกลับจะถูกเก็บไว้ในตัวแปรนั้นพร้อม แท็กประเภท `File:` (กรณีนี้ก็เช่นกัน) อย่างไรก็ตามใน บรรทัดถัดไปค่า `4` ได้ถูกเพิ่มเข้าไปในตัวควบคุมไฟล์ `4` ไม่มีแท็ก

ในตัวอย่างข้างต้น `fopen` คือชื่อฟังก์ชั่น ไม่ใช่ศัพท์ภาษาอังกฤษ ดังนั้นล้อมรอบด้วยเครื่องหมายตัวอย่าง `โค้ด` ช่วยแยกความแตกต่างจากเนื้อหาอื่น

นอกจากนี้ หากย่อหน้านั้นอ้างอิงถึงโค้ดตัวอย่าง สิ่งนี้ก็สามารถช่วย ให้ผู้อ่านสามารถเชื่อมโยงความเข้าใจกับโค้ดได้ง่ายขึ้น

### ตาราง

หากตารางนั้นมีหัวข้อ เขียนให้อยู่ในส่วนบนสุด:

- ❌

  ```md
  |         |                               |
  | ------- | ----------------------------- |
  | สภาพ    | สถานะเครื่องยนต์              |
  | 650     | ไม่มีความเสียหาย              |
  | 650-550 | ควันขาว                       |
  | 550-390 | ควันเทา                       |
  | 390-250 | ควันดำ                        |
  | < 250   | ติดไฟ (จะระเบิดในวินาทีต่อมา) |
  ```

- ✔

  ```md
  | สภาพ    | สถานะเครื่องยนต์              |
  | ------- | ----------------------------- |
  | 650     | ไม่มีความเสียหาย              |
  | 650-550 | ควันขาว                       |
  | 550-390 | ควันเทา                       |
  | 390-250 | ควันดำ                        |
  | < 250   | ติดไฟ (จะระเบิดในวินาทีต่อมา) |
  ```

## การย้ายจาก SA-MP Wiki

เนื้อหาส่วนใหญ่ได้ถูกย้ายแล้ว แต่หากคุณพบหน้าที่ขาดหายไป นี่คือคำแนะนำสั้น ๆ เกี่ยวกับการแปลงเนื้อหาเป็น Markdown

### รับไฟล์ HTML

1. คลิกปุ่มนี้

   (Firefox)

   ![image](https://assets.open.mp/assets/images/contributing/04f024579f8d.png)

   (Chrome)

   ![image](https://assets.open.mp/assets/images/contributing/f62bb8112543.png)

2. หากเมาส์ที่ด้านบนซ้ายของหน้าหลักใน wiki ในมุมหรือขอบด้านซ้าย จนกว่าคุณจะเห็น `#content`

   ![image](https://assets.open.mp/assets/images/contributing/65761ffbc429.png)

   หรือค้นหา `<div id=content>`

   ![image](https://assets.open.mp/assets/images/contributing/77befe2749fd.png)

3. คัดลอกองค์ประกอบภายใน HTML นั้น

   ![image](https://assets.open.mp/assets/images/contributing/8c7c75cfabad.png)

   ตอนนี้คุณมี _เพียง_ โค้ด HTML สำหรับ _เนื้อหา_ ที่เห็นของหน้านี้แล้ว เลือก สิ่งที่เราสนใจ และคุณสามารถแปลงมันเป็น Markdown ได้

### แปลง HTML เป็น Markdown

สำหรับการแปลงโค้ด HTML แบบพื้น ๆ (ไม่ใช่ตาราง) เป็น Markdown ใช้:

https://mixmark-io.github.io/turndown/

![image](https://assets.open.mp/assets/images/contributing/77f4ea555bbb.png)

^^ สังเกตได้เลยว่าตอนนี้ มันทำตารางเละหมดแล้ว...

### ตาราง HTML เป็นตาราง Markdown

เพราะเครื่องมือด้านบนไม่รองรับการแปลงตาราง ใช้เครื่องมือนี้:

https://jmalarcon.github.io/markdowntables/

และคัดลอกแค่องค์ประกอบใน `<table>`:

![image](https://assets.open.mp/assets/images/contributing/57f171ae0da7.png)

### ทำความสะอาด

การแปลงมันไม่สมบูรณ์แบบ ดังนั้นคุณจะต้องแก้ไขด้วยตัวเองเล็กน้อย ส่วนขยายที่ทำการจัดรูปแบบด้านบนจะช่วยเหลือคุณ แต่คุณ ยังคงต้องใช้เวลาทำด้วยตัวเองอีกสักเล็กน้อย

หากคุณไม่มีเวลา ไม่ต้องกังวลไป! ส่งแบบร่างที่ยังไม่เสร็จแล้วให้คนอื่นมาทำต่อ จากจุดที่คุณทำค้างไว้!
