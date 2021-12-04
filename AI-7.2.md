# AI Part 7-2

## 귀납적 학습의 예

귀납적 학습은 일반화된 패턴이나 규칙, 법칙 또는 조직적 형태 등을 기존의 데이터나 경험, 예제 등으로부터 얻어내는 과정을 포함한다.

## 일반화와 개념공간
개념공간을 정의하는데 있어서 가장 일반적으로 적용되는 연산은 일반화와 세부화이다.

Weights = {light, heavy}
Heights = {tail, short}

도메인 내의 개체는 body_type(Weights, Heights)라는 술어로 표현할 수 있다.

## 일반화를 위한 연산

상수를 변수로 바꾼다.
- weight(john, heavy) -> weight(X, heavy)로 일반화

결합(Conjunctive)문장에서 조건을 제거한다.
- weight(X, heavy) ^ height(X, tail) ^ hobby(X, basketball)을
- weight(X, heavy) ^ height(X, tail)로 일반화

문장에 이접(Disjunction) 조건을 추가한다.
- weight(X, heavy) ^ height(X, tail) ^ hobby(X, basketball)을
- weight(X, heavy) ^ height(X, tail) ^ hobby(X, basketball) V hobby(X, volleyball)로 일반화

특성의 유형을 유형계층(Type Hierarchy)에서 상위 유형으로 바꾼다.
(만약 유형계층에 sports가 basketball의 상위 유형이라면)
- hobby(X, basketball)을 hobby(X, sports)로 일반화


