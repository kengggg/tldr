# reboot

> เริ่มระบบใหม่
> ข้อมูลเพิ่มเติม: <https://manned.org/reboot.8>.

- เริ่มระบบใหม่:

`reboot`

- ปิดระบบ (ทำงานเหมือน `poweroff`):

`reboot --poweroff`

- หยุดระบบ (หยุดทุกโปรแกรมและปิด CPU ทำงานเหมือนกับ `halt`):

`reboot --halt`

- บังคับเริ่มระบบใหม่ทันที:

`reboot --force`

- เขียนบันทึก wtmp โดยไม่ต้องเริ่มระบบใหม่:

`reboot --wtmp-only`
