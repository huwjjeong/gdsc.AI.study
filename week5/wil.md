### 역전파
역전파는 인공 신경망을 학습시키기 위한 알고리즘이다. 
목표값과 모델의 출력값의 차이를 계산한 후, 이 오차를 네트워크를 통해 뒤로 전파하면서 각 노드의 가중치를 갱신한다.

### 계산, 그래프
역전파는 미분 연쇄 법칙을 사용하여 가중치에 대한 그레디언트를 효율적으로 계산한다. 
이를 위해 연산을 순차적으로 처리하는 계산 그래프를 사용한다.
만약 역전파가 없다면 각 가중치에 대해 손실 함수를 따로 계산해야 하므로 매우 많은 계산이 필요한다.

### 순전파
순전파는 입력 데이터를 신경망을 통해 출력으로 변환하고, 손실 함수 값을 계산하는 과정이다.

### 역전파
역전파는 손실 함수의 기울기를 구하여 가중치를 조정하는 과정으로, 미분 연쇄 법칙을 사용해 모든 가중치의 기울기를 동시에 구한다.


### 확장
ReLU 계층에서의 역전파 및 CNN(합성곱 신경망)으로의 확장 가능성에 대해 설명
역전파는 기본적으로 '파라미터 값이 오르면 최종 손실(Loss)에 어떤 영향을 미치는가'를 미분값을 통해 계산하는 과정이다.