

# DL_info

# 앤드류 응 선생님의 딥러닝의 AtoZ

https://www.youtube.com/playlist?list=PLkDaE6sCZn6Ec-XTbcX1uRg2_u4xOEky0


# 정보를 찾다가 유용한 것이 있으면 기록하는 습관을 들이자

- In image data EDA, PCA of dimensionality reduction using
 
1. PCA는 데이터에 있는 정보들을 대부분 유지하면서 차원을 줄이는 통계방법이다. 인간은 3차원이 넘어가는 데이터로부터 시각적으로 유용한 정보를 찾기가 어렵다. 따라서, PCA를 이용하여 고차원의 데이터를 3차원으로 줄이고 이것을 시각화해보면 각 데이터마다 어떤 특징이 있는지 알아볼 수 있다.
 
2. PCA말고 t-SNE라는 기법도 있다. 이것 역시 고차원의 데이터의 차원을 줄이는 기법이고 원본 데이터를 가장 잘 표현하도록 한다. 하지만 많은 계산이 요구된다. 따라서, 엄청난 고차원의 경우, 1차로 차원을 축소한 후 TSNE를 적용하는 것을 추천한다. 실제로 PCA보다 TSNE의 결과를 시각화해보면 분류를 해내는 능력이 훨씬 더 뛰어나다는 것을 알 수 있을 것이다.
링크: https://skyeong.net/284


- gradient descent

1. ![image](https://user-images.githubusercontent.com/43164589/110793059-8a8c2b00-82b7-11eb-8ce5-958f24656d01.png)
![image](https://user-images.githubusercontent.com/43164589/110793152-a394dc00-82b7-11eb-9313-2dffdfd11bce.png)
