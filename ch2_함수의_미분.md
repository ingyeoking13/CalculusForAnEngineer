## 함수의 미분 
# THE DERIVATIVE OF A FUNCTION 

## Contents
1. introduction  
2. 접선  
2.1 접선  
2.2 접선의 기울기를 구하기   
2.3 delta notation  
2.4 미분의 정의   

## introduction  
`calculus`는 보통 크게 두 파트로 나뉜다. 첫 째는 `미분differential calculus`이고, 둘 째는 `적분integral calculus`이다.  

두 파트 모두 자신들만의 용어와 난해한 기호들 그리고 자신들만의 연산법이 있다. 그래서 이들을 배울 땐, 마치 각각의 새로운 언어를 배우는 것과 유사하다.  
하지만, `calculus`의 기초 영역과 응용 영역을 아우르는 핵심적인 질문은 다음 두가지 문제로 기술할 수 있다.

> **PROBLEM 1** 미분의 기저 문제는 *기울기의 문제* 이다. 그래프의 임의의 점 **P** 에 접하는 선의 기울기를 연산하는 것이다.  
> **PROBLEM 2** 적분의 기저 문제는 *넓이의 문제* 이다. 두 점 **x = a, x = b** 사이의 넓이를 연산하는 것이다.  

# 2. 접선 
## 2.1 접선

원에 대한 접선은 비교적 이해하기 쉽다. 원에 존재하는 단 하나의 점과 교차하는 접선이다. 두 점에 교차하거나 아예 교차하지 않으면 접선이 아니다.  
단, 곡선에 대해서는 위 표현이 달갑지 않을 수 있다. 왜냐하면 임의의 곡선 위의 점 P에 대한 접선이 곡선의 다른 점과 만날 수 있기 때문이다.  

따라서, 접선을 설명하기 위한 비교적 적절한 표현은 다음과 같다.  

> 곡선 <img src="/tex/f673b75871a86bab338f2f9feb5a9417.svg?invert_in_darkmode&sanitize=true" align=middle width=62.56467194999998pt height=24.65753399999998pt/> 가 있다고 하자. 곡선 위의 점 P에 대한 접선을 구한다고 하자. 곡선 위의 임의의 점 Q와 P를 가로지르는 선분을 긋자. 이 선분을 <img src="/tex/6fbc176ce9ff34475832a5ff858b7ddd.svg?invert_in_darkmode&sanitize=true" align=middle width=25.832197049999987pt height=27.725679300000007pt/> 라 하자. 이때, Q를 곡선을 따라 P로 가까이 이동 시킬 때, 곡선 P에 접하는 접선을 구할 수 있다.  

## 2.2 접선의 기울기를 구하기  

곡선 위의 점 P가 다음을 만족한다고 하자.   <img src="/tex/12d0ceffb3db9300f7b8af2ac568ece7.svg?invert_in_darkmode&sanitize=true" align=middle width=87.04905824999999pt height=24.65753399999998pt/>   
그리고, 곡선 위의 다른점 Q가 다음을 만족한다고 하자.<img src="/tex/177cbeed7678f0a9149fe5d25b55740b.svg?invert_in_darkmode&sanitize=true" align=middle width=87.20771069999998pt height=24.65753399999998pt/>

이 때, 선분 <img src="/tex/6fbc176ce9ff34475832a5ff858b7ddd.svg?invert_in_darkmode&sanitize=true" align=middle width=25.832197049999987pt height=27.725679300000007pt/>는 다음을 만족한다.  

<p align="center"><img src="/tex/23b474640b5e1ea9d2e56e5467d22d95.svg?invert_in_darkmode&sanitize=true" align=middle width=239.15455079999998pt height=34.45133834999999pt/></p>

점 Q를 움직여, <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>을 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>에 근접한다고 하자. 선분은 접선 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>와 닮아 가는 것을 볼 수 있다. 이러한 행위를 다음과 같이 표현할 수 있다.

<p align="center"><img src="/tex/23884bcdf5cb070bcce193784289267c.svg?invert_in_darkmode&sanitize=true" align=middle width=227.3624991pt height=34.45133834999999pt/></p>  

<img src="/tex/f6cf1f679a64c6f52a0f8a20b8736713.svg?invert_in_darkmode&sanitize=true" align=middle width=62.854261799999996pt height=22.831056599999986pt/>이란, <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>가 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>에 점점 다가간다는 뜻이다. 이에 착안하여, 단순히 <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/> 에 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>을 대입할 수는 없다. 왜냐하면 분모 <img src="/tex/901d8a70099cff0fa75662518b7dd153.svg?invert_in_darkmode&sanitize=true" align=middle width=52.808174099999995pt height=19.1781018pt/>이 <img src="/tex/29632a9bf827ce0200454dd32fc3be82.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>이 되기 때문이다.

이로써 다음을 명심해야한다. <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>이 꾸준히 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>에 가까워지지만, 여전히 <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>과 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/> 사이에는 명확한 구별이 있어야한다는 점이다. 이를 꾸준히 연산하면 분모<img src="/tex/d500e7fd1d6d1de1e6f7cc936c6ced47.svg?invert_in_darkmode&sanitize=true" align=middle width=50.13706004999999pt height=19.1781018pt/>와 분자<img src="/tex/a55fdd837b1bc94c4d1421c9fe742112.svg?invert_in_darkmode&sanitize=true" align=middle width=52.808174099999995pt height=19.1781018pt/>이 어떤 작은 수가 된다는 것은 분명하지만, 분수의 결과 값이 어떤 게 될지는 명확하지 않다.  

만약 점 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>와 <img src="/tex/1afcdb0f704394b16fe85fb40c45ca7a.svg?invert_in_darkmode&sanitize=true" align=middle width=12.99542474999999pt height=22.465723500000017pt/>가 다음 함수 <img src="/tex/e0e62234e6e08eaa90332c05ae9d55a0.svg?invert_in_darkmode&sanitize=true" align=middle width=46.514371199999985pt height=26.76175259999998pt/> 위에 있다고 하자. 그러면 다음을 따른다.

<p align="center"><img src="/tex/658ba8f972c3bf64110c43b99c9871bf.svg?invert_in_darkmode&sanitize=true" align=middle width=267.28246215pt height=38.2431621pt/></p>

따라서, <img src="/tex/bcb037123f40331d39ba394f2f25c697.svg?invert_in_darkmode&sanitize=true" align=middle width=46.514371199999985pt height=26.76175259999998pt/> 함수에서 수식 <img src="/tex/a9ef45be1cd9cd2165b8ebbb2a779178.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=24.65753399999998pt/>를 다음과 같이 표현할 수 있다.

<p align="center"><img src="/tex/2a6784b6bed5f970a87c3e78dce57364.svg?invert_in_darkmode&sanitize=true" align=middle width=389.76620264999997pt height=38.2431621pt/></p>

이 때, <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>이 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>에 근접하면 <img src="/tex/2529199970eeef09ea6d160508a1ae45.svg?invert_in_darkmode&sanitize=true" align=middle width=52.808174099999995pt height=19.1781018pt/>은 <img src="/tex/ce59d49b0bc432d8d6a3ebb4f94a25f1.svg?invert_in_darkmode&sanitize=true" align=middle width=99.71446154999998pt height=21.18721440000001pt/>과 매우 매우 근접해 질것이다.

따라서, 점 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>에서의 접선은 다음과 같다.  

<p align="center"><img src="/tex/bcb76e422d7994f5883f6e6a59dd5679.svg?invert_in_darkmode&sanitize=true" align=middle width=60.5174757pt height=13.059335849999998pt/></p>

## 2.3 delta notation  

`delta notation`은 <img src="/tex/3919bbc84b8079e27194efe99a1f6a80.svg?invert_in_darkmode&sanitize=true" align=middle width=23.09366069999999pt height=22.465723500000017pt/>과 같이 표기한다. <img src="/tex/7e9fe18dc67705c858c077c5ee292ab4.svg?invert_in_darkmode&sanitize=true" align=middle width=13.69867124999999pt height=22.465723500000017pt/>는 그리스 문자로 영어 알파벳 <img src="/tex/2103f85b8b1477f430fc407cad462224.svg?invert_in_darkmode&sanitize=true" align=middle width=8.55596444999999pt height=22.831056599999986pt/>를 뜻한다. 이 때 <img src="/tex/2103f85b8b1477f430fc407cad462224.svg?invert_in_darkmode&sanitize=true" align=middle width=8.55596444999999pt height=22.831056599999986pt/>는 `difference`를 뜻하며 두 변수간 값의 차이를 표현하기 위해 사용한다.

그러므로, 일반적으로 <img src="/tex/3919bbc84b8079e27194efe99a1f6a80.svg?invert_in_darkmode&sanitize=true" align=middle width=23.09366069999999pt height=22.465723500000017pt/>는 다음을 뜻한다.  

<p align="center"><img src="/tex/f871f2891b5b0a333dc6d2fa01e98593.svg?invert_in_darkmode&sanitize=true" align=middle width=97.81946459999999pt height=13.698590399999999pt/></p>

다음 또한 만족한다.  

<p align="center"><img src="/tex/83b903a6e64faec29585f93d9b58e8d5.svg?invert_in_darkmode&sanitize=true" align=middle width=98.64137745000001pt height=13.698590399999999pt/></p>

이를 이용해 <img src="/tex/bcb037123f40331d39ba394f2f25c697.svg?invert_in_darkmode&sanitize=true" align=middle width=46.514371199999985pt height=26.76175259999998pt/> 함수에서 임의의 정점 P에 대해 다시 한번 선분의 기울기를 표현해보자.

<p align="center"><img src="/tex/a7cf047a79d65969e6403f97472a3319.svg?invert_in_darkmode&sanitize=true" align=middle width=253.92876959999998pt height=38.2431621pt/></p>   

이 때, <img src="/tex/cf330257519e06f13c2ecab5e25c6d2a.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=24.65753399999998pt/>의 식은 다음과 같이 풀어질 수 있다.  


<p align="center"><img src="/tex/aedfa2746755b661ad5732adee6826c4.svg?invert_in_darkmode&sanitize=true" align=middle width=323.21888774999996pt height=18.312383099999998pt/></p>
<p align="center"><img src="/tex/38ad42e92b5cc487c551ac7f72cc1f72.svg?invert_in_darkmode&sanitize=true" align=middle width=121.40413395pt height=16.438356pt/></p>
Thus, 

<p align="center"><img src="/tex/e165f085df49d653af941d1334741bbe.svg?invert_in_darkmode&sanitize=true" align=middle width=123.66207149999998pt height=13.698590399999999pt/></p> 

접선의 기울기를 표현할 때 사용한 극한 <img src="/tex/f6cf1f679a64c6f52a0f8a20b8736713.svg?invert_in_darkmode&sanitize=true" align=middle width=62.854261799999996pt height=22.831056599999986pt/>는 <img src="/tex/f24f315a0766ef5a65c0907abc789ca4.svg?invert_in_darkmode&sanitize=true" align=middle width=60.742260149999986pt height=22.831056599999986pt/>와 동치이다. 

마지막으로, 접선의 기울기는 다음과 같이 표현할 수 있다.

<p align="center"><img src="/tex/d4e25999812b6561254c384fcfd3bfaf.svg?invert_in_darkmode&sanitize=true" align=middle width=201.3051315pt height=22.931502pt/></p>


이제 까지 나온 표현을 모두 정리하면 다음과 같다. 

1. 선분의 기울기 


<p align="center"><img src="/tex/1414f7287397079e4651f726cb913eca.svg?invert_in_darkmode&sanitize=true" align=middle width=156.29694135pt height=37.1910528pt/></p>
<p align="center"><img src="/tex/2117044dfdafb99a4c0cfc9d1bb97387.svg?invert_in_darkmode&sanitize=true" align=middle width=138.74182904999998pt height=34.7253258pt/></p>
2. 접선의 기울기

<p align="center"><img src="/tex/530df31971f5634215608cc8736c046b.svg?invert_in_darkmode&sanitize=true" align=middle width=180.74375385pt height=37.1910528pt/></p>
<p align="center"><img src="/tex/65b11b8b3823d8c623086bcd25f52aeb.svg?invert_in_darkmode&sanitize=true" align=middle width=179.39257214999998pt height=34.7253258pt/></p>

이 때, 미분에서는 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>에서의 접선 기울기라고 좀 더 명확하게 표현하기 위해 다음과 같이 사용한다. 

<p align="center"><img src="/tex/c74328f830bc54ea800598bdf36c814b.svg?invert_in_darkmode&sanitize=true" align=middle width=227.9428404pt height=34.7253258pt/></p>

## 2.4  도함수의 정의  

함수 <img src="/tex/7997339883ac20f551e7f35efff0a2b9.svg?invert_in_darkmode&sanitize=true" align=middle width=31.99783454999999pt height=24.65753399999998pt/>가 주어졌을 때, 그것의 도함수 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>가 정의역 <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>에서 갖는 값은 다음과 같다.    

<p align="center"><img src="/tex/3f9445f8e14d315b8e59892eb5a620c3.svg?invert_in_darkmode&sanitize=true" align=middle width=205.8195447pt height=34.7253258pt/></p>

도함수를 설명할 때 곡선의 임의의 점에 대한 접선의 기울기의 집합이라고 표현할 수 있다. 그러나 반드시 곡선과 같은 그래프를 머리에 떠올려 접선을 그어보지 않아도 된다.  
여전히 기하학을 이용한 사고방식이 도함수의 이해에 큰 도움이 되지만, 다음 챕터에서는 또 다른 접근법을 알아볼 것이다.

도함수 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>를 구하는 데엔 다음 세가지 방식을 따른다. 이 것을 `three-step rule`이라 하겠다. 앞서 다루었던 내용이므로 다시 한번 기억을 다듬어보는 것도 좋겠다.  

>STEP 1 변화율을 구한다. <img src="/tex/c7614b9d270128341f65cc0b8188ca64.svg?invert_in_darkmode&sanitize=true" align=middle width=127.27171049999998pt height=24.65753399999998pt/>   
>STEP 2 <img src="/tex/3919bbc84b8079e27194efe99a1f6a80.svg?invert_in_darkmode&sanitize=true" align=middle width=23.09366069999999pt height=22.465723500000017pt/>로 나누어 평균 변화율을 구한다. <img src="/tex/cc978f0a9435c602f7d4f82f85032c09.svg?invert_in_darkmode&sanitize=true" align=middle width=89.47544265pt height=33.20539859999999pt/>  
>STEP 3 <img src="/tex/f24f315a0766ef5a65c0907abc789ca4.svg?invert_in_darkmode&sanitize=true" align=middle width=60.742260149999986pt height=22.831056599999986pt/>을 이용하여 평균 변화율의 극한값을 구한다.  


# text


<p align="center"><img src="/tex/5985f9c02f75c34c3aa40b2cff6f9bc3.svg?invert_in_darkmode&sanitize=true" align=middle width=100.75330154999999pt height=16.438356pt/></p>

조건 방정식으로 표현하면 다음과 같다.  

<p align="center"><img src="/tex/e717addd32463514950da3cce0c562a1.svg?invert_in_darkmode&sanitize=true" align=middle width=203.52704625pt height=49.315569599999996pt/></p>

위 방정식<img src="/tex/d343a5beaabde2410ecf9f826344ed83.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=24.65753399999998pt/>을 활용하여 표현해보자. 

<p align="center"><img src="/tex/1f4cfc60d8855fdebd54c91e3e3beff2.svg?invert_in_darkmode&sanitize=true" align=middle width=329.3422341pt height=34.7253258pt/></p>

<img src="/tex/dd9e3a6635a2cbe51aa4d0f0c1ca251b.svg?invert_in_darkmode&sanitize=true" align=middle width=96.52988894999999pt height=24.65753399999998pt/>를 이해하기 위해 <img src="/tex/b82b509cf285024a5fac5c7a7b0c3e48.svg?invert_in_darkmode&sanitize=true" align=middle width=18.52743584999999pt height=24.65753399999998pt/> 함수를 표현해보자.  
