# adduser

> เครื่องมือเพิ่มผู้ใช้ในระบบ.
> ข้อมูลเพิ่มเติม: <https://manpages.debian.org/latest/adduser/adduser.html>.

- สร้างผู้ใช้ใหม่ด้วยโฮมไดเรกทอรีแบบปริยายและให้ผู้ใช้ตั้งรหัสผ่าน:

`adduser {{username}}`

- สร้างผู้ใช้ใหม่โดยไม่ต้องมีโฮมไดเรกทอรี:

`adduser --no-create-home {{username}}`

- สร้างผู้ใช้ใหม่โดยกำหนดที่อยู่โฮมไดเรกทอรี:

`adduser --home {{path/to/home}} {{username}}`

- สร้างผู้ใช้ใหม่โดยกำหนดล็อกอินเชล:

`adduser --shell {{path/to/shell}} {{username}}`

- สร้างผู้ใช้ใหม่ในกลุ่มที่กำหนด:

`adduser --ingroup {{group}} {{username}}`
