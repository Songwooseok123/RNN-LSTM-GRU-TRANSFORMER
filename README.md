# RNN-LSTM-GRU-TRANSFORMER

### Word2vec

"단어를 고정된 크기의 벡터로 변환해준다."

<br>**[문제점]**<br>
feed forward 신경망으로서 한 뱡향으로만 신호가 전달됨<br> 
-> 시계열 데이터 학습 잘 못함
# RNN
![image](https://user-images.githubusercontent.com/80091008/189818771-485c3585-9cc2-452b-a9d1-f00396b0cb4c.png)


[장점] 과거의 정보를 현재로 흘려주면서 과거의 정보(은닉상태)를 인코딩해 저장할 수 있음

[단점] 시간적으로 멀리 떨어진 long term 의존 관계를 잘 학습할 수 없음. -> 기울기 손실, 폭발 

# LSTM

![image](https://user-images.githubusercontent.com/80091008/189818871-79d3b64f-7d75-46b2-bc3b-36091775a01d.png)

게이트 구조를 더해서 RNN의 단점을 보안함.
1. forget gate layer
2. input gate layer
3. updatae cell state
4. output gate layer

[단점] : 메모리가 덮어씌어질 가능성이 있음. 연산속도가 느림

## GRU : 계산시간을 줄이기 위해 LSTM의 구조를 단순화한 모델(hidden state vector만 사용, gate 갯수 2개로 줄임- reset gate, update gate) 
