# (PdOOPschool) ไลบรารี่สำหรับใช้เรียน Python OOP by Pd Soft.


โปรแกรมนี้ได้จากการเรียนออนไลน์ในเพจเฟสบุ๊ก ลุงวิศวะสอนคำนวน เป็นเพจที่สอนได้ดีมากๆ


### วิธีติดตั้ง

เปิด CMD / Terminal

```python
pip install pdoopschool
```

### วิธีใช้งานแพ็กเกจนี้

- เปิด IDLE ขึ้นมาแล้วพิมพ์...

```python
import pdoopschool import Student,Tesla,SpecialStudent,Teacher
# Day 0

allstudent = []

teacher1 =Teacher('Ada Lovelace')
teacher2 =Teacher('Bill Gates')
print(teacher1.students)

# Day 1
print('======== DAY 1 ========')
st1 = Student('Albert','Einstein')
allstudent.append(st1)
print(st1.fullname)
teacher2.AddStudent(st1)


# Day 2
print('======== DAY 2 ========')
st2 = Student('Steve','Jobs')
allstudent.append(st2)
print(st2.fullname)
teacher2.AddStudent(st2)

# Day 3
print('======== DAY 3 ========')
for i in range(3):
	st1.Coding()
st2.Coding()

st1.ShowEXP()
st2.ShowEXP()


# Day 4
print('======== DAY 4 ========')
stp1 = SpecialStudent('Thomas', 'Edison','Hitler')
allstudent.append(stp1)
teacher1.AddStudent(stp1)
print(stp1.fullname)
print('ขอคะแนนเพิ่มหน่อยครับครู..!')
stp1.exp = 20  # แก้ไขค่าใน class ได้  
stp1.Coding()
stp1.ShowEXP()


# Day 5
print('======== DAY 5 ========')

print('นักเรียนกลับบ้านยังไงกันเหรอ..?')

print(allstudent)

for st in allstudent:
	print('ผม {} กลับบ้านด้วย {} ครับ'.format(st.name,st.vehicle))
	if isinstance(st,SpecialStudent):
		st.vehicle.SelfDriving(st)


# Day 6
print('======== DAY 6 ========')

teacher1.CheckStudent()
teacher2.CheckStudent()

print('รวมพลังของนักเรียน 2 คน',st1 + st2)



สอนโดย: ลุงวิศวกร สอนคำนวณ
FB: https://www.facebook.com/UncleEngineer
YouTube: https://www.youtube.com/UncleEngineer
