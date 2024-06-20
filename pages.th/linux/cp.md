# cp

> คัดลอกไฟล์และไดเรกทอรี
> ข้อมูลเพิ่มเติม: <https://www.gnu.org/software/coreutils/cp>.

- คัดลอกไฟล์ไปที่ตำแหน่งอื่น:

`cp {{path/to/source_file.ext}} {{path/to/target_file.ext}}`

- คัดลอกไฟล์ไปยังตำแหน่งอื่นและใช้ชื่อไฟล์เดิม:

`cp {{path/to/source_file.ext}} {{path/to/target_parent_directory}}`

- คัดลอกเนื้อหาทั้งหมดในไดเรกทอรีไปยังตำแหน่งอื่น ถ้ามีตำแหน่งนั้นอยู่แล้วจะคัดลอกไดเรกทอรีไปยังตำแหน่งนั้น:

`cp -r {{path/to/source_directory}} {{path/to/target_directory}}`

- คัดลอกเนื้อหาทั้งหมดในไดเรกทอรีและแสดงชื่อไฟล์ที่กำลังดำเนินการ:

`cp -vr {{path/to/source_directory}} {{path/to/target_directory}}`

- คัดลอกหลายๆ ไฟล์ไปยังไดเรกทอรีปลายทางในครั้งเดียว:

`cp -t {{path/to/destination_directory}} {{path/to/file1 path/to/file2 ...}}`

- ใช้โหมด interactive เพื่อคัดลอกไฟล์ทั้งหมดที่มีนามสกุลเดียวกันไปยังตำแหน่งอื่น ผู้ใช้ต้องทำการยืนยันถ้าจะเขียนทับไฟล์ที่มีอยู่แล้ว:

`cp -i {{*.ext}} {{path/to/target_directory}}`

- ตาม symbolic link ก่อนที่จะคัดลอก:

`cp -L {{link}} {{path/to/target_directory}}`

- ใช้เส้นทางแบบเต็มของไฟล์ต้นฉบับ สร้างไดเรกทอรีกลางที่ขาดหายไปเมื่อคัดลอก:

`cp --parents {{source/path/to/file}} {{path/to/target_file}}`
