# OS
오픈소스SW개론 테스트 파일

## top 명령어

+ 서버 CPU 사용률 및 메모리 사용률을 보여주는 명령어 
+ CPU 사용이 많은 순서대로 나타내줌
+ 어플리케이션 형태

## top 명령어에 대한 설명

+ us : 사용자 레벨의 CPU 사용 비중
+ sy : 시스템 레벨의 CPU 사용 비중
+ ni : 우선순위가 낮은 프로세스의 CPU 사용 비중
+ id : 유휴 상태의 CPU 사용 비중
+ wa : I/O를 대기 중인 CPU 사용 비중
+ hi : interrupt handler에서 사용 중인 CPU 사용률, 빠르게 수행을 마쳐야 하는 작업
+ si : hi에서 오래 걸리는 작업 때문에 미뤄놓은 작업
+ st : 하이퍼바이저가 다른 가상 프로세서를 서비스하는 동안 가상 CPU가 실제 CPU를 기다리는 시간
  
## top 실행 후 명령
+ shift + p : CPU 사용률 내림차순
+ shit + m : 메모리 사용률 내림차순
+ shift + t : 프로세스가 돌아가고 있는 시간 순
+ k : kill. k 입력 후 PID 번호 작성. signal은 9
+ f : sort field 선택 화면 -> q 누르면 RES순으로 정렬
+ a : 메모리 사용량에 따라 정렬
+ b : Batch 모드로 작동
+ 1 : CPU Core별로 사용량 보여줌

## VIRT, RES, SHR

+ 현재 프로세스에서 사용하고 있는 메모리

#### VIRT
 - 프로세스가 사용하고 있는 virtual memory의 전체 용량
 - 프로세스에 할당된 가상 메모리 전체
 - SWAP + RES
#### RES
 - 현재 프로세스가 사용하고 있는 물리 메모리의 양
 - 실제 물리 메모리
 - 실제로 메모리를 쓰고 있는 RES가 핵심!
#### SHR
 - 다른 프로세스와 공유하고 있는 shared memory의 양

## ps 명령어

+ linux에서 현재 동작하고 있는 process들에 대한 정보를 보여주는 명령어

## ps 명령어 옵션
+ -e : 실행중인 모든 프로세스의 정보를 출력
+ -f : 프로세스에 대한 자세한 정보를 출력 (PPID 확인 가능)(Full format)
+ -l : -f 보다 더 자세한 정보를 출력 (Long format)
+ -u [사용자 이름] : 특정 사용자에 대한 모든 프로세스의 정보를 출력
+ -p pid : pid로 지정한 프로세스의 정보를 출력

![ps -efl](./OS ps -efl image.png)

+ a : 터미널에서 실행한 프로세스의 정보를 출력(R-실행중, S-대기, T-정지, Z-좀비프로세스)
+ u : 프로세스 소유자의 이름, CPU 사용량, 메모리 사용량 등 상세한 정보 출력 (default = present user)
+ x : 실행 중인 모든 프로세스의 정보를 출력




안녕하세요. 반갑습니다.
---

###### 안녕하세요
### 안녕하세요
## 안녕하세요

***

+ 일어나기
+ 밥먹기
+ 자기

1. 일어나기
2. 밥먹기
3. 자기

> 인용문
>> 인용문

`printf("Hello World!");`

```C
#include <stdio.h>

int main(void){
  printf("hello world!\n");
  return 0;
}
```


```git
git commit -m "my first commit"
```
