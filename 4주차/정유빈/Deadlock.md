<h1> Deadlock </h1> 

- <b> blocked / asleep state </b>
  - 프로세스가 특정 이벤트를 기다리는 상태
  - 프로세스가 필요한 자원을 기다리는 상태

- <b> deadlock state </b>
  - 프로세스가 발생 가능성이 없는 이벤트를 기다리는 경우
    - 프로세스가 deadlock 상태에 있음
  - 시스템 내에 deadlock에 빠진 프로세스가 있는 경우
    - 시스템이 deadlock 상태에 있음

![image](https://github.com/youbeen2798/Deep-CS-study_for_interview/assets/62228401/4b29dcab-7220-43e5-af7a-25c5315f7b65)
- DeadLock vs Starvation
  - DeadLock : blocked 상태에서 <b> 가능성이 zero </b> 인 자원 혹은 event를 기다리는 상태
  - Starvation : ready 상태(cpu로부터 자원을 할당받기를 기다리는 상태)에서 운이 없어서, 우선순위가 계속 밀리는 상태

<h1> 자원의 분류 </h1>

 - 일반적 분류
   - Hardware resources vs Software resources
 - 다른 분류 법
   - 선점 가능 여부에 따른 분류
   - 할당 단위에 따른 분류
   - 동시 사용 가능 여부에 따른 분류
   - 재사용 가능 여부에 따른 분류

<h3> 선점 가능 여부에 따른 분류 </h3>

- <b> Preemptible resources </b>
  - 선점 당한 후, 돌아와도 문제가 발생하지 않는 자원
  - Processor, memory 등
- <b> Non-preemptible resources </b>
  - 선점 당하면, 이후 진행에 문제가 발생하는 자원
  - Rollback, restart 등 특별한 동작이 필요
  - ex) disk drive 등
