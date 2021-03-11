

# DL_info

# 1. 앤드류 응 선생님의 딥러닝의 AtoZ

https://www.youtube.com/playlist?list=PLkDaE6sCZn6Ec-XTbcX1uRg2_u4xOEky0




# 2. 정보를 찾다가 유용한 것이 있으면 기록하는 습관을 들이자

# In image data EDA, PCA of dimensionality reduction using
 
1. PCA는 데이터에 있는 정보들을 대부분 유지하면서 차원을 줄이는 통계방법이다. 인간은 3차원이 넘어가는 데이터로부터 시각적으로 유용한 정보를 찾기가 어렵다. 따라서, PCA를 이용하여 고차원의 데이터를 3차원으로 줄이고 이것을 시각화해보면 각 데이터마다 어떤 특징이 있는지 알아볼 수 있다.
 
2. PCA말고 t-SNE라는 기법도 있다. 이것 역시 고차원의 데이터의 차원을 줄이는 기법이고 원본 데이터를 가장 잘 표현하도록 한다. 하지만 많은 계산이 요구된다. 따라서, 엄청난 고차원의 경우, 1차로 차원을 축소한 후 TSNE를 적용하는 것을 추천한다. 실제로 PCA보다 TSNE의 결과를 시각화해보면 분류를 해내는 능력이 훨씬 더 뛰어나다는 것을 알 수 있을 것이다.
링크: https://skyeong.net/284


# gradient descent

![image](https://user-images.githubusercontent.com/43164589/110793059-8a8c2b00-82b7-11eb-8ce5-958f24656d01.png)    ![image](https://user-images.githubusercontent.com/43164589/110793152-a394dc00-82b7-11eb-9313-2dffdfd11bce.png)

cost(w) = (1/2M)*sum(Wx(i)-y(i))^2

- repeat: W:= W-alpha(learning rate)(d/dW)cost(W)

 Thus, W:= W - alpha(1/M) * sum(Wx(i)-y(i))*x(i)

- 만약, (W,cost(W))가 미분계수(기울기)가 양의 값을 가질때, W-alpha(learning rate)(d/dW)cost(W)에 의해 update된 W는 왼쪽방햐으로 한 단계 이동하는 것이다.

여기서 update 되는 횟수는 mini batch가 1 에폭을 도달하기까지와 전체 에폭이 달성될떄까지 update 되는 것이다.


# Vectorization

- Numpy.dot(w,x)를 활용해서 연산 시간을 단축시키자
- 벡터라이즈는 병렬화의 장점을 이용하는 것!
