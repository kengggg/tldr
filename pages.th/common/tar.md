# tar

> เครื่องมือช่วยจัดระเบียบไฟล์
> บ่อยครั้งใช้ร่วมกับการบีบอัดไฟล์ เช่น gzip หรือ bzip
> ข้อมูลเพิ่มเติม: <https://www.gnu.org/software/tar>.

- สร้างแฟ้มเก็บถาวรจากไฟล์:

`tar cf {{target.tar}} {{file1}} {{file2}} {{file3}}`

- สร้างแฟ้มเก็บถาวรที่บีบอัดด้วย gzip:

`tar czf {{target.tar.gz}} {{file1}} {{file2}} {{file3}}`

- สร้างแฟ้มเก็บถาวรแล้วบีบอัดด้วย gzip จากโฟลเดอร์ที่กำหนด

`tar czf {{target.tar.gz}} -C {{path/to/directory}} .`

- แตกแฟ้มเก็บถาวรที่บีบอัดไว้ที่โฟลเดอร์ปัจจุบัน:

`tar xf {{source.tar[.gz|.bz2|.xz]}}`

- แตกแฟ้มเก็บถาวรที่บีบอัดไว้ที่โฟลเดอร์ที่กำหนด:

`tar xf {{source.tar[.gz|.bz2|.xz]}} -C {{directory}}`

- สร้างแฟ้มเก็บถาวรโดยการระบุนามสกุลของไฟล์เพื่อระบุโปรแกรมการบีบอัดไฟล์:

`tar caf {{target.tar.xz}} {{file1}} {{file2}} {{file3}}`

- แสดงรายการแฟ้มที่อยู่ใน tar:

`tar tvf {{source.tar}}`

- แตกไฟล์ที่ตรงกับรูปแบบ:

`tar xf {{source.tar}} --wildcards "{{*.html}}"`

- แตกไฟล์ที่กำหนดโดยไม่ต้องใส่ใจถึงโครงสร้างโฟลเดอร์เดิม:

`tar xf {{source.tar}} {{source.tar/path/to/extract}} --strip-components={{depth_to_strip}}`
