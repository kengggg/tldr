# cat

> พิมพ์และต่อไฟล์
> ข้อมูลเพิ่มเติม: <https://www.gnu.org/software/coreutils/cat>.

- พิมพ์เนื้อหาของไฟล์ไปยัง `stdout`:

`cat {{path/to/file}}`

- รวมไฟล์หลายไฟล์เป็นไฟล์ผลลัพธ์:

`cat {{path/to/file1 path/to/file2 ...}} > {{path/to/output_file}}`

- ต่อไฟล์หลายไฟล์ไปยังท้ายไฟล์ผลลัพธ์:

`cat {{path/to/file1 path/to/file2 ...}} >> {{path/to/output_file}}`

- เขียน `stdin` ไปที่ไฟล์:

`cat - > {{path/to/file}}`

- กำหนดจำนวนบรรทัด:

`cat -n {{path/to/file}}`

- แสดงอักขระที่พิมพ์ไม่ได้และช่องว่าง (ใช้ `M-` ถ้าเป็นอักขระ non-ASCII):

`cat -v -t -e {{path/to/file}}`
