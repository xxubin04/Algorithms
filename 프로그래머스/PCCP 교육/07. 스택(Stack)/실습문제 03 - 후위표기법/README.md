## 문제 설명

우리가 일반적으로 사용하는 계산방식은 중위표기법(Infix Notation)이라 하는데,

A + B와 같이 피연산자 'A'와 'B' 중간에 연산자 '+'가 위치하여 이렇게 불린다.

컴퓨터공학에서는 후위표기법 (Postfix Notation)을 많이 사용하는데,

후위표기법은 A B + 와 같이 피연산자 'A'와 'B'의 뒤에 연산자 '+'가 위치한 표기법을 말한다.

중위표기법에서 (5+8)2 와 같은 수식은 ''가 '+'보다 연산자 우선순위가 높으므로

앞의 수식 에서처럼 5+8 을 먼저 계산해야한다면 괄호를 사용해야한다.

하지만 수식 (5+8)*2 을 후위표기법으로 바꾸면 5 8 + 2 * 와 같이 되어,

후위표기법은 괄호가 없이도 연산자의 우선 순위 를 명확히 할 수 있다는 장점이 있다.

이런 이유로 소프트웨어로 구현되는 계산기들은 후위표기법을 많이 사용한다.

그럼 후위표기법의 수식을 입력 받아 계산하는 프로그램을 작성해 보자.

0으로 나누는 경우는 주어지지 않는다.

<br>
<br>

## 입력 설명

입력의 첫 줄에는 총 입력되는 연산자와 피연산자의 개수의 합 M(3 ≤ M ≤ 11 )이 입력되며,

그 다음 줄에 M개의 연산자와 피연산자가 한 칸씩의 공백 을 두고 입력된다.

피연산자 X 는 0≤X≤9 의 범위를 가지는 정수이며,

연산자는 사칙연산인 '*', '/', '+', '-'의 네 가지가 입력된다.

0으로 나누는 경우는 입력되지 않는다.

<br>
<br>

## 출력 설명

피연산자나 연산자가 부족한 경우와 같이 완전하지 않은 수식은 입력되지 않는다.

나눗셈 연산의 경우, 소수점 이하는 버리고 몫만 계산되며 정수로 나타난다.

예를 들어 10 3 / 은 3이 된다.

<br>
<br>

### 입력1 예시

```
3
2 3 +
```

<br>


### 출력1 예시

```
5
```

<br>

### 입력2 예시

```
5
5 8 + 2 *
```


<br>

### 출력2 예시

```
26
```

<br>

### 입력3 예시

```
5
1 8 1 / +
```

<br>

### 출력3 예시

```
9
```
