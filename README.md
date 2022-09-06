# RNN-LSTM-GRU-TRANSFORMER

### Word2vec

"단어를 고정된 크기의 벡터로 변환해준다."

<br>**[문제점]**<br>
feed forward 신경망으로서 한 뱡향으로만 신호가 전달됨<br> 
-> 시계열 데이터 학습 잘 못함
# RNN
![image.png](attachment:899cc0be-cb39-4cd8-b1b8-854db68e56c4.png)!

[장점] 과거의 정보를 현재로 흘려주면서 과거의 정보(은닉상태)를 인코딩해 저장할 수 있음

[단점] 시간적으로 멀리 떨어진 long term 의존 관계를 잘 학습할 수 없음. -> 기울기 손실, 폭발