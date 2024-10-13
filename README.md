# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
* https://github.com/marioyokim/SWE_2021_41_2024_2_week_4/tree/main
/

```python
def isHappy(n):

  arr = set()

  while n != 1 and n not in arr:
    arr.add(n)
    n = sum(int(digit) ** 2 for digit in str(n))

  return n == 1

number = int(input())

if isHappy(number):
  print("True")
else:
  print("False")
```
1. arr = set() : 이미 계산된 수를 저장하는 집합을 만듬.
2. while n != 1 and n not in arr : n이 1이 아니고, 이전에 계산한 적이 없는 수일 때까지 반복.
3. n = sum(int(digit) ** 2 for digit in str(n)) : 각 자릿수를 제곱 후 그 합을 다시 n에 저장.

---
##Week 5 Assignment
1. __docker exec <container_name> cat /etc/os-release__
: 지정된 컨테이너 안에서 /etc/os-release 파일을 읽어와 출력함.


2. __docker exec <container_name> git --version__
: 지정된 컨테이너 안에서 git 명령을 실행, 설치된 git의 버전을 출력함.


3. __docker exec <container_name> python3 --version__
: 지정된 컨테이너 안에서 python3 명령을 실행, 설치된 Python 3의 버전을 출력함.


4. __docker inspect --format="{{ .HostConfig.Binds }}" <container_name>__
: 컨테이너의 설정 정보를 확인함. 컨테이너의 "Bind Mount"를 확인함.

---
