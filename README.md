# scikit-learn-package

Olivetti faces 라는 Dataset을 가지고 얼굴 이미지를 분석하여 동일 인물끼리 매칭시키는 머신 러닝을 진행해보았다.

training dataset 에는    Classes                                40
                         Samples total                         400
                         Dimensionality                       4096
                         Features            real, between 0 and 1   가 포함되어있고 
                         
scikit learn pagckage 에서 perceptron algorithm 을 사용하였다.

perceptron algorithm 의 hyperparameter 중 penalty, alpha, l1_ratio, eta0 을 바꿔주면서 best model를 찾았다.

penalty는 elasticnet를 선택하고 l1,l2 규제항의 비율을 0.15->0.11 로 감소시키고 , 학습율을 1.0->1.4 로 늘려 속도를 증가시켰다 
최종 결과로 학습의 정확도가 86%가 출력되었다.
