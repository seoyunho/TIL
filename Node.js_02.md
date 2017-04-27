# 로그 간단하게 살펴보기

### 1.콘솔에 로그 뿌리기

>  js파일에는 console 객체가 사용된다.
>
>  여기서 console 객첸느 전역 객체라고 부르며 말 그대로 필요하면 코드의 어느 부분에서나 사용할 수 있다.

#### -전역 객체

>  노드에서 쓸 수 있는 전역 객체는 다음과 같다.

```
1.console : 콘솔 창에 결과를 보여주는 객체
2.process : 프로세스의 실행에 대한 정보를 다루는 객체
3.exports : 모듈을 다루는 객체
```

##### 1.console 객체

>  이 중에서도 console 객체는 가장 많이 쓰이는 것 중 하나이다. console 객체는 콘솔 화면에 결과를 보여주기 위해서 어디에서나 사용할 수 있으며 console 객체에 정의된 log() 메소드를 호출하면서 문자열을 파라미터로 전달하면 그대로 출력된다.
>
>  console 객체에는 log() 메소드 말고도 메소드가 있다.

```
1.dir(object) : 자바스크립트 객체의 속성들을 한꺼번에 출력해 주는 메소드
2.time(id) : 실행 시간을 측정하기 위한 끝시간을 기록하는 메소드
3.timeEnd(id) : 실행 시간을 측정하기 위한 끝시간을 기록하는 메소드
```

##### 2.process 객체

>  process 객체는 프로그램을 실행했을 때 만들어지는 프로세스 정보를 다루는 객체이다. process 객체의 주요 속성과 메소드는 다음과 같다

```
1.argv : 프로세스를 실행할 때 전달되는 파라미터 정보
2.env : 환경변수 정보
3.exit() : 프로세스를 끝내는 메소드
```

> argv 속성은 프로세스를 실행할 때 전달되는 파라미터 정보를 가지고 있다.  이러한 process 객체에 들어있는 argv 속성은 배열 객체이며 파일을 실행하기만 해도 node 명령과 파일 패스가 파라미터 값으로 들어간다.
>
> env 속성은 환경변수 정보를 가지고 있다. env 속성을 이용해서 환경 변수의 값을 확인할 수 있다. 윈도우의 시스템 환경변수로는 OS환경 변수가 있다. env 속성을 사용해서 이러한 환경변수의 정보를 얻을 수 있다.  하지만 OS환경 변수로 접근을 하면 오류가 발생하는데 이유는 env 속성에는 사용자 정의 환경 변수만 들어 있고, OS환경 변수와 같은 시스템 환경변수는 없기 때문이다.