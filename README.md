# pyHSK (Personal Python Study Group)

## Member
Heo , jin seong
Seo , jun yong
Kang, hong seok

## Mission 1. Basic data manipulation using str, float, list type. (Due date 09-Nov-2018)

### **To Seo**

> Mission : 다음 os 명령을 수행하여 생성된 txt 파일을 읽어 파일 size가 가장 큰 파일명과 파일 사이즈를 출력하시오.
    (파일 사이즈는 KB 단위로 출력할 것)

```bash
Linux 에서 수행할 것
 # cd
 # ls -al /etc > out.txt
```

### **To Heo**
> Mission : 다음 os 명령을 수행하여 생성된 txt 파일을 읽어 평균 응답 속도(ms)를 계산하여 출력하시오.

```bash
 # ping www.google.com > out.txt

```

### **Mission 해결 Hint**

> Hint 1 : File io  ( 읽기 전용으로 특정 파일을 열어서 한줄씩 읽어 변수에 저장한다)
```python
with open("out.txt","r") as f:
        mylines = f.readlines()

        for line in mylines:
            # To do
```

> Hint 2 : String split (string 변수를 특정 deliminater 단위로 나누어 List type 변수로 저장한다.)
```python
>>> mystr="aaa bbb ccc"
>>> print(mystr)
aaa bbb ccc
>>> mylist = mystr.split(" ")
>>> print(mylist)
['aaa', 'bbb', 'ccc']
>>> print(mylist[1])
bbb
```

> Hint 3 : String 변수를  int(정수형)이나 float(실수형) 변수로 변환(type cast) 한다.
```python
>>> aaa = "111"
>>> bbb = "222"
>>> print(aaa + bbb)
111222
>>> faaa = float(aaa)
>>> fbbb = float(bbb)
>>> print(faaa + fbbb)
333.0
```
> Hint 4 : String 변수에서 특정 문자 제거(또는 대체)  한다.
```python
>>> aaa = "32ms"
>>> bbb = aaa.replace("ms","")
>>> print(bbb)
32
```

# 참고할 사이트
- [Jump to Python](https://wikidocs.net/book/1)