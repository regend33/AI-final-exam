# AI Part 6-3

## 계층적 계획 수립(Hierarchical Planning)

## ABSTRIPS(ABstract specification for STRIPS)
계층적으로 계획을 수립하고 하위 단계들의 전제조건이나 세부 계획을 무시하고 추상공간에서 상위 계획을 수립한 다음 세부적인 것들을 나중에 채워가는 방식
- 중요도가 가장 큰 문제의 전제조건만을 먼저 생각하여 (하위 목표들에 대한 전제조건의 고려 없이) STRIPS 방식으로 계획을 수립하고, 다음 단계로 내려가면서 같은 방식으로 계획을 수립
- 처음에는 대략적으로 전체적인 계획이 수립되고, 이후 차츰차츰 세분화 되어 가며 전체 계획이 완성됨

- ABSTRIPS 시스템은 목표에 포함 된 논리곱인자에 한계 값(Criticality Number)를 부여하여 부 목표들의 난이도를 표시
- 계층적 계획 수립의 한계 값을 결정하는 것은 매우 중요함

ABSTRIPS의 한계 값을 사용한 단계적 계획 수립 방식
- 가장 달성하기 어려운(한계 값이 가장 큰) 목표를 설정
- 한계 값을 하나 낮추어 그 한계 값을 찾는 (부)목표를 달성하기 위한 계획을 수립
- 이를 반복