# lshw

> แสดงรายละเอียดเกี่ยวกับการตั้งค่า hardware
> ข้อมูลเพิ่มเติม: <https://manned.org/lshw>.

- เปิดหน้าจอ GUI:

`sudo lshw -X`

- แสดง hardware ทั้งหมดในรูปแบบตาราง:

`sudo lshw -short`

- แสดงดิสก์และ storage controller ทั้งหมดในรูปแบบตาราง:

`sudo lshw -class disk -class storage -short`

- บันทึกการตั้งค่า interfaces ทั้งหมดให้เป็นไฟล์ HTML:

`sudo lshw -class network -html > {{interfaces.html}}`
