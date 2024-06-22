# kill

> ส่งสัญญาณไปยัง process โดยทั่วไปแล้วจะเกี่ยวข้องกับการหยุด process
> Process จะตรวจจับทุกสัญญาณยกเว้น SIGKILL และ SIGSTOP เพื่อให้ process หยุดการทำงานอย่างเรียบร้อย
> ข้อมูลเพิ่มเติม: <https://manned.org/kill>.

- หยุดโปรแกรมโดยใช้สัญญาณ SIGTERM (terminate):

`kill {{process_id}}`

- แสดงค่าและชื่อของสัญญาณโดยไม่ต้องมีคำว่า `SIG` นำหน้า:

`kill {{-L|--table}}`

- หยุดงานที่อยู่เบื้องหลัง:

`kill %{{job_id}}`

- หยุดโปรแกรมโดยใช้สัญญาณ SIGHUP (hang up) หลายๆ โปรแกรมจะเริ่มทำงานตั้งแต่ต้นแทนที่จะหยุดทำงาน:

`kill -{{1|HUP}} {{process_id}}`

- หยุดโปรแกรมโดยใช้สัญญา SIGINT (interupt) ได้ผลเช่นเดียวกับผู้ใช้กดปุ่ม `Ctrl + C`:

`kill -{{2|INT}} {{process_id}}`

- ส่งสัญญาณให้ระบบหยุดโปรแกรมโดยทันทีโดยไม่ต้องสนใจอะไร:

`kill -{{9|KILL}} {{process_id}}`

- ส่งสัญญาณให้ระบบหยุดโปรแกรมชั่วคราว (pause) จนกว่าจะได้รับสัญญาณ SIGCONT (continue):

`kill -{{17|STOP}} {{process_id}}`

- ส่งสัญญาณ `SIGUSR` ไปยังทุก process ใน GID (group id):

`kill -{{SIGUSR1}} -{{group_id}}`
