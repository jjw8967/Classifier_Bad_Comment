# FFP를 이용한 악플 분류기

## FFP
> FFP의 featrure을 각 문장의 자질길이를 선정하여 문장을 쪼갠 단어들로 선정하였다.
> * EX)
> 연애하는 거 꼴보기 싫다.
> ['연애', "애하","하는","는거","거꼴","꼴보","보기","기싫","싫다"]

> 현대 인터넷 댓글의 초성 사용으로 인한 언어파괴를 처리하기 위하여
> 분리된 단어들에서 빈도수가 높은 글자를 초성을 변화하였다.
>  * EX) 빈도수 높은 글자 : '하', '는', '기' ,'다' 라고 했을 때 
> ['연애', "애ㅎ","ㅎㄴ","ㄴ거","거꼴","꼴보","보ㄱ","ㄱ싫","싫ㄷ"]

> 해당 문장의 feature들은 각 자질의 빈도 값으로 하였다.

## FFP-Parameter
* __K__ : 자질의 길이
* __P__ : p% 이상의 빈도수를 초성으로 변환


## Model

* __SVM__

## Model Parameter

* __gamma__

## Cross-validation

> k,p,gamma를 파라미터로 하여 5-fold cross-validation하였다.

## TODO

> 데이터 전처리에 대해 생각을 해봐야할것 같다.
