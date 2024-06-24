# lsusb

> แสดงข้อมูลทั้งหมดของ bus และอุปกรณ์ USB ทั้งหมดที่เชื่อมต่อกับระบบ
> ข้อมูลเพิ่มเติม: <https://manned.org/lsusb>.

- แสดงรายการอุปกรณ์ USB ทั้งหมดที่มี:

`lsusb`

- แสดงรายการลำดับอุปกรณ์ USB ทั้งหมดเป็นแผนภูมิต้นไม้:

`lsusb -t`

- แสดงข้อมูลอุปกรณ์ USB แบบละเอียด:

`lsusb --verbose`

- แสดงข้อมูลของอุปกรณ์ USB ที่ระบุอย่างละเอียด:

`lsusb --verbose -s {{bus}}:{{device number}}`

- แสดงอุปกรณ์ตาม vendor และ product ID ที่ระบุ:

`lsusb -d {{vendor}}:{{product}}`
