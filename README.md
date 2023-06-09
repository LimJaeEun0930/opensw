# OPEN SOURCE SW 
---
## top

cpu와 메모리 이용에 관한 정보를 표시하는 작업관리자 프로그램

PID USER PR NI ...등등을 열로서 표현한다.

맨 상단에 요약내용을 볼 수 있다.

---

## ps

Process Status의 약자. 현재 돌아가고 있는 프로세스를 확인할 수 있다.

option: 

* -e: 현재 사용자 + 다른 사용자들이 구동시킨 모든프로세스 보여줌.
* -f: 상세한 정보 보여준다.
* -l: 더 상세한 정보 보여준다.

-ef가 많이 사용된다고 한다.

---

## jobs

작업의 상태를 표시하는 명령어. 쉘에서 실행시킨 백그라운드 작업 목록이 출력된다.

option:

* -l: 프로세스 그룹ID를 state 필드 앞에 출력한다.
* -n: 프로세스 그룹중 대표 프로세스 ID를 출력한다.
* -p: 각 프로세스 ID에 대해 한 행씩 출력한다.

출력내용:
* Running 작업이 계속 진행중.
* Done    작업이 완료됨.
* Stopped 작업이 일시 중단됨.

---
## kill

프로세스를 의 동작을 제어할수 있는 명령어. kill [option] [PID]

프로세스를 죽이거나 중지하거나 로드하는 등의 액션을 취할 수 있다.
option:

* -9 프로세스아이디(PID)를 지정하여 종료시킨다.
ex) kill -9 PID
* -l 사용가능한 모든 신호목록을 가져온다. 
신호는 세가지 방법으로 지정할 수 있다.
1. 숫자 
2. SIG접두사 사용 
3. SIG접두사 비사용
ex)
* kill -1 PID
* kill -SIGHUP PID
* kill -HUP PID
