# Multi_Thread_Count
## 멀티쓰레드를 이용한 카운터

**프로그램 요구 사항**

1. 프로그램이 시작되면 사용자는 카운터의  Max값(정수)을 입력한다. 그리고 입력된  Max값은 공유 객체의 필드인 count의 초기값으로 사용된다.
2. 메인스레드는 2개의 스레드(threadA,threadB)를 생성하고, 생성된 2개의 스레드들은 공유 객체의 필드인 count를 번갈아가면서 1씩 감소시킨다.
3. 각 스레드가 count를 1감소시킬때 마다 어떤 스레드가 값을 감소시켰는지를 감소된 count값과 함꼐 출력시킨다.
4. 각 스레드는 count값이 0에 도달 하면 종료된다.
5. 각 스레드가 종료될때 스레드의 종료를 알리는 메세지가 출력된다.
6. 메인스레드는 두 스레드가 모두 종료되면 현재 공유 객체의 count값을 출력시키고 프로그램을 종료한다.
