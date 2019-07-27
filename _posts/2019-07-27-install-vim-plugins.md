---
layout: post
title: Install Plugins for Vi/Vim
author: Rangsiman Ketkaew
date: "2019-07-27 23:26:00 +0700"
category:
  - Vi-Vim
  - text-editor
summary: How to install plugins and examples for vi/vim editor
thumbnail: posts/vim-logo.png
permalink: content/7
comments: true
---

## เกริ่นนำ

สวัสดีครับ โพสต์นี้ผมจะอธิบายวิธีการติดตั้งโปรแกรมเสริมให้กับ Vi หรือ Vim โปรแกรมแก้ไขข้อความยอดฮิตกันนะครับ โดยความสามารถที่เราจะเพิ่มให้กับ Vim สามารถทำได้หลายวิธี จากการที่ผมได้ลองเครื่องมือที่ต่าง ๆ แล้วผมพบว่าการติดตั้ง

<br>

## ติดตั้งไลบรารี่ Plug

ไลบรารี่ที่ผมพบว่าสามารถติดตั้ง plugin หรือ extension เสริมตัวอื่น ๆ สำหรับ vim ได้นั่นก็คือ Plug ซึ่งสามารถดาวน์โหลดใช้งานได้ฟรี

1. เปิด terminal

2. ติดตั้ง Plug
```sh
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

1. เปิดไฟล์ ~/.vimrc
```sh
vi ~/.vimrc
```

1. เพิ่มคำสั่งเพื่อเรียกใช้งาน plugin หรือ extension ที่ต้องการ ซึ่งคำสั่งจะขึ้นต้นด้วยคีเวิร์ด **Plug** ดังตัวอย่างต่อไปนี้ 
```
Plug 'junegunn/vim-easy-align'
```

1. อัพเดทการตั้งค่าของไฟล์ .vimrc โดยการ activate ไฟล์ด้วยคำสั่งต่อไป
```sh
source ~/.vimrc
```

1. เปิด vi ขึ้นมา
```sh
vi
```

1. กดปุ่ม **Esc** และกด **shift** + **;**
   (สังเกตว่าด้านล่างซ้ายของหน้าต่าง vi จะปรากฎ **:** ขึ้นมา)

2.  รันคำสั่งต่อไปนี้เพื่อติดตั้ง plugin ทั้งหมดที่ระบุในไฟล์ .vimrc ด้วย plug แล้ว Enter
```
:PlugInstall
```

1. รอสักครู่จนกระทั่งการติดตั้งเสร็จเรียบร้อย

<br>

## ตรวจสอบการติดตั้ง

- เราสามารถตรวจสอบได้ว่าโปรแกรมเสริมได้ถูกติดตั้งเรียบร้อยหรือไม่โดยการรันคำสั่งต่อไปนี้ใน vim
```
:PlugStatus
```

- นอกจากนี้เราอาจจะทดสอบโดยการเรียกใช้ plugin บางตัวขึ้นมาทดสอบ เช่น NERDTree
```
:NERDTree
```

<br/>

---

ด้านล่างคือตัวอย่างไฟล์ .vimrc ของผมครับ

<script src="https://gist.github.com/rangsimanketkaew/ac5e705540fd1feeeda5866e32073deb.js"></script>
