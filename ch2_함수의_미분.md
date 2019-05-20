## 함수의 미분 
# THE DERIVATIVE OF A FUNCTION 

## Contents
1. introduction  
2. 접선  
2.1 접선  
2.2 접선의 기울기를 구하기   
2.3 delta notation 1  
2.4 미분의 정의   
2.5 delta notation 2  
2.6 임의의 점에서 미분이 가능하지 않을 때  
2.7 속도와 변화율  
2.8Last 극한과 연속 함수  

## introduction  
`calculus`는 보통 크게 두 파트로 나뉜다. 첫 째는 `미분differential calculus`이고, 둘 째는 `적분integral calculus`이다.  

두 파트 모두 자신들만의 용어와 난해한 기호들 그리고 자신들만의 연산법이 있다. 그래서 이들을 배울 땐, 마치 각각의 새로운 언어를 배우는 것과 유사하다.  
하지만, `calculus`의 기초 영역과 응용 영역을 아우르는 핵심적인 질문은 다음 두가지 문제로 기술할 수 있다.

> **PROBLEM 1** 미분의 기저 문제는 *기울기의 문제* 이다. 그래프의 임의의 점 **P** 에 접하는 선의 기울기를 연산하는 것이다.  
> **PROBLEM 2** 적분의 기저 문제는 *넓이의 문제* 이다. 두 점 **x = a, x = b** 사이의 넓이를 연산하는 것이다.  

# 2. 도함수 
## 2.1 접선

원에 대한 접선은 비교적 이해하기 쉽다. 원에 존재하는 단 하나의 점과 교차하는 접선이다. 두 점에 교차하거나 아예 교차하지 않으면 접선이 아니다.  
단, 곡선에 대해서는 위 표현이 달갑지 않을 수 있다. 왜냐하면 임의의 곡선 위의 점 P에 대한 접선이 곡선의 다른 점과 만날 수도 있기 때문이다.  

따라서, 접선을 설명하기 위한 비교적 적절한 표현은 다음과 같다.  

> 곡선 <img src="/tex/f673b75871a86bab338f2f9feb5a9417.svg?invert_in_darkmode&sanitize=true" align=middle width=62.56467194999998pt height=24.65753399999998pt/> 가 있다고 하자. 곡선 위의 점 P에 대한 접선을 구한다고 하자. 곡선 위의 임의의 점 Q와 P를 가로지르는 선분을 긋자. 이 선분을 <img src="/tex/6fbc176ce9ff34475832a5ff858b7ddd.svg?invert_in_darkmode&sanitize=true" align=middle width=25.832197049999987pt height=27.725679300000007pt/> 라 하자. 이때, Q를 곡선을 따라 P로 가까이 이동 시킬 때, 곡선 P에 접하는 접선을 구할 수 있다.  

## 2.2 접선의 기울기를 구하기  

곡선 위의 점 P가 다음을 만족한다고 하자. <img src="/tex/12d0ceffb3db9300f7b8af2ac568ece7.svg?invert_in_darkmode&sanitize=true" align=middle width=87.04905824999999pt height=24.65753399999998pt/>    
그리고, 곡선 위의 다른점 Q가 다음을 만족한다고 하자. <img src="/tex/177cbeed7678f0a9149fe5d25b55740b.svg?invert_in_darkmode&sanitize=true" align=middle width=87.20771069999998pt height=24.65753399999998pt/>  

이 때, 선분 <img src="/tex/6fbc176ce9ff34475832a5ff858b7ddd.svg?invert_in_darkmode&sanitize=true" align=middle width=25.832197049999987pt height=27.725679300000007pt/>는 다음을 만족한다.  

<p align="center"><img src="/tex/9ad454d5176973ddacf4d7db8901668d.svg?invert_in_darkmode&sanitize=true" align=middle width=239.42859764999997pt height=34.45133834999999pt/></p>

점 Q를 움직여, <img src="/tex/277fbbae7d4bc65b6aa601ea481bebcc.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>을 <img src="/tex/e714a3139958da04b41e3e607a544455.svg?invert_in_darkmode&sanitize=true" align=middle width=15.94753544999999pt height=14.15524440000002pt/>에 근접한다고 하자. 선분은 접선 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>와 닮아 가는 것을 직관적으로 알 수 있다. 이러한 행위를 다음과 같이 표현할 수 있다.

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

## 2.3 delta notation 1 

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

따라서,  

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

<p align="center"><img src="/tex/61ada5a03faea4e7b244643f2f57546b.svg?invert_in_darkmode&sanitize=true" align=middle width=250.54577129999998pt height=34.7253258pt/></p>

## 2.4  도함수의 정의  

함수 <img src="/tex/7997339883ac20f551e7f35efff0a2b9.svg?invert_in_darkmode&sanitize=true" align=middle width=31.99783454999999pt height=24.65753399999998pt/>가 주어졌을 때, 그것의 도함수 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>가 정의역 <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>에서 갖는 값은 다음과 같다.    

<p align="center"><img src="/tex/d85e1177b444e987b04f3d6fd8c38ff9.svg?invert_in_darkmode&sanitize=true" align=middle width=228.42239145pt height=34.7253258pt/></p>

도함수를 설명할 때 곡선의 임의의 점에 대한 접선의 기울기의 집합이라고 표현할 수 있다. 그러나 반드시 곡선과 같은 그래프를 머리에 떠올려 접선을 그어보지 않아도 된다.  
여전히 기하학을 이용한 사고방식이 도함수의 이해에 큰 도움이 되지만, 다음 챕터에서는 또 다른 접근법을 알아볼 것이다.

도함수 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>를 구하는 데엔 다음 세가지 방식을 따른다. 이 것을 `three-step rule`이라 하겠다. 앞서 다루었던 내용이므로 다시 한번 기억을 다듬어보는 것도 좋겠다.  

>STEP 1 변화율을 구한다. <img src="/tex/c7614b9d270128341f65cc0b8188ca64.svg?invert_in_darkmode&sanitize=true" align=middle width=127.27171049999998pt height=24.65753399999998pt/>   
>STEP 2 <img src="/tex/3919bbc84b8079e27194efe99a1f6a80.svg?invert_in_darkmode&sanitize=true" align=middle width=23.09366069999999pt height=22.465723500000017pt/>로 나누어 평균 변화율을 구한다. <img src="/tex/cc978f0a9435c602f7d4f82f85032c09.svg?invert_in_darkmode&sanitize=true" align=middle width=89.47544265pt height=33.20539859999999pt/>  
>STEP 3 <img src="/tex/f24f315a0766ef5a65c0907abc789ca4.svg?invert_in_darkmode&sanitize=true" align=middle width=60.742260149999986pt height=22.831056599999986pt/>을 이용하여 평균 변화율의 극한값을 구한다.  

**Example 1** Find <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/> if <img src="/tex/cd45989378bd32cf1227ffcccb9ed8c4.svg?invert_in_darkmode&sanitize=true" align=middle width=69.86299979999998pt height=26.76175259999998pt/>  

**STEP 1**

<p align="center"><img src="/tex/5bf82832cc8a9de96ad3d0d2726abf46.svg?invert_in_darkmode&sanitize=true" align=middle width=257.96779964999996pt height=18.312383099999998pt/></p>
 <p align="center"><img src="/tex/d21fb6e7e1c42d0508902854a48e3d9e.svg?invert_in_darkmode&sanitize=true" align=middle width=282.63690015000003pt height=18.312383099999998pt/></p>
 <p align="center"><img src="/tex/19d76b3bc0d7e3c4db2db644a2e831ab.svg?invert_in_darkmode&sanitize=true" align=middle width=208.91562284999998pt height=18.312383099999998pt/></p>
 <p align="center"><img src="/tex/8c66ca08adc7012f3fbb11018d321ebf.svg?invert_in_darkmode&sanitize=true" align=middle width=202.3630752pt height=18.312383099999998pt/></p>

**STEP 2**

<p align="center"><img src="/tex/605e68046043dbd99e819e6f2358037b.svg?invert_in_darkmode&sanitize=true" align=middle width=299.47238474999995pt height=34.7253258pt/></p>

**STEP 3**

<p align="center"><img src="/tex/d048c58bb970c657e384da326b76b858.svg?invert_in_darkmode&sanitize=true" align=middle width=304.44068159999995pt height=24.805529099999998pt/></p>

함수 <img src="/tex/bed39cc142caec73dd26ebf7cb3356a7.svg?invert_in_darkmode&sanitize=true" align=middle width=63.342435749999986pt height=27.77565449999998pt/> 와 <img src="/tex/ac95dfbba07837bc60d1bd101cd4a439.svg?invert_in_darkmode&sanitize=true" align=middle width=77.00912505pt height=24.995338500000003pt/>에 대해서 도함수도 구하는 절차는 독자에게 맡긴다.   
각각의 도함수는 <img src="/tex/f1193304c9a9cab050a4a1ae7304b356.svg?invert_in_darkmode&sanitize=true" align=middle width=87.15533474999998pt height=27.77565449999998pt/>과 <img src="/tex/bd35de8ca9ff4917f371f7f89cd5c581.svg?invert_in_darkmode&sanitize=true" align=middle width=85.30599164999998pt height=27.77565449999998pt/>이다. 

결과 도함수의 이해를 돕기위해 간략히 쓴다. 도함수 <img src="/tex/f1193304c9a9cab050a4a1ae7304b356.svg?invert_in_darkmode&sanitize=true" align=middle width=87.15533474999998pt height=27.77565449999998pt/>는 <img src="/tex/fabb70be53704ed7e6095eca25e82d82.svg?invert_in_darkmode&sanitize=true" align=middle width=70.84469699999998pt height=24.65753399999998pt/>에서 항상 음수이다. 그리고 <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>가 <img src="/tex/29632a9bf827ce0200454dd32fc3be82.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>에 근접할 수록 도함수 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>의 매우 큰 수로 발산하는 것을 알 수 있다. 이는 <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>가 <img src="/tex/29632a9bf827ce0200454dd32fc3be82.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>에 근접할수록 접선이 매우 가팔라 진다는 것이다. <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>의 절대값이 커질수록 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>는 <img src="/tex/29632a9bf827ce0200454dd32fc3be82.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>에 수렴하며, 접선이 수평선에 가까워진다는 것이다.   

## 2.5 delta notation 2  

수학에 있어 표기법은 굉장히 중요한 역할을 한다. 좋은 표기법은 좋은 방향성을 제시해주며, 나쁜 표기법은 쉬운 표현도 어렵게 만드는 법이다.  

우리는 함수 <img src="/tex/7997339883ac20f551e7f35efff0a2b9.svg?invert_in_darkmode&sanitize=true" align=middle width=31.99783454999999pt height=24.65753399999998pt/>의 도함수를 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>라고 표기하였다. 도함수는 함수 <img src="/tex/7997339883ac20f551e7f35efff0a2b9.svg?invert_in_darkmode&sanitize=true" align=middle width=31.99783454999999pt height=24.65753399999998pt/>에서 도출되었지만 정의역 <img src="/tex/332cc365a4987aacce0ead01b8bdcc0b.svg?invert_in_darkmode&sanitize=true" align=middle width=9.39498779999999pt height=14.15524440000002pt/>에 대해선 새로운 함수임을 강조하기 위해 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>라는 표기를 쓰므로, 그 의미를 표현하는데 적절하다고 할 수 있다. 종종, 함수의 치역 변수인 <img src="/tex/deceeaf6940a8c7a5a02373728002b0f.svg?invert_in_darkmode&sanitize=true" align=middle width=8.649225749999989pt height=14.15524440000002pt/>를 써서 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>를 <img src="/tex/15f93b25ba881e5829e8fc647b680fb2.svg?invert_in_darkmode&sanitize=true" align=middle width=12.43916849999999pt height=24.7161288pt/>로 쓰기도 한다.  

도함수를 표현하는데에 <img src="/tex/9ce3fa8c71f5905e328dcae5b1d69e2d.svg?invert_in_darkmode&sanitize=true" align=middle width=36.60970994999999pt height=24.7161288pt/>의 사용은 단점도 있다. 도함수가 변화율을 기반으로 도출되었는지 명확하게 드러내주지 않는다. 

앞으로 소개할 수학자 `Leibniz`의 표기법은 도함수를 이해하는데 적절히 도움이 된다. 

도함수의 분자인 <img src="/tex/deceeaf6940a8c7a5a02373728002b0f.svg?invert_in_darkmode&sanitize=true" align=middle width=8.649225749999989pt height=14.15524440000002pt/>의 변화율을 다음과 같이 표현하자.  

<p align="center"><img src="/tex/e53c7b009bf484747de2a671428b01ad.svg?invert_in_darkmode&sanitize=true" align=middle width=171.53721915pt height=16.438356pt/></p>

이 때, 도함수는 다음과 같이 표현한다.  

<p align="center"><img src="/tex/7b2feca9bf489c470565b2c971db023a.svg?invert_in_darkmode&sanitize=true" align=middle width=130.9650672pt height=33.81208709999999pt/></p>

<img src="/tex/f673b75871a86bab338f2f9feb5a9417.svg?invert_in_darkmode&sanitize=true" align=middle width=62.56467194999998pt height=24.65753399999998pt/>이므로 다음과 같이 표현할 수 있다.  

<p align="center"><img src="/tex/fa46ef07d62e56cfb58a7c9549224230.svg?invert_in_darkmode&sanitize=true" align=middle width=217.93925174999998pt height=34.7253258pt/></p>

<img src="/tex/24a7d013bfb0af0838f476055fc6e1ef.svg?invert_in_darkmode&sanitize=true" align=middle width=14.297449649999997pt height=30.648287999999997pt/>는 <img src="/tex/b9c2ca43d254d796a226779c529f4b2d.svg?invert_in_darkmode&sanitize=true" align=middle width=22.831119299999987pt height=22.831056599999986pt/>표현과 <img src="/tex/7e9fe18dc67705c858c077c5ee292ab4.svg?invert_in_darkmode&sanitize=true" align=middle width=13.69867124999999pt height=22.465723500000017pt/>을 생략하는 대신 <img src="/tex/2103f85b8b1477f430fc407cad462224.svg?invert_in_darkmode&sanitize=true" align=middle width=8.55596444999999pt height=22.831056599999986pt/>로 대체한 것이다.   
읽는 사람으로 하여금 <img src="/tex/a68ec5ebaa4ef77691bb5703206cce98.svg?invert_in_darkmode&sanitize=true" align=middle width=53.660747249999986pt height=24.65753399999998pt/> 변화율에서 <img src="/tex/28e60f8855c12248cc740b7cda4138fc.svg?invert_in_darkmode&sanitize=true" align=middle width=56.88346949999999pt height=22.465723500000017pt/>를 수행한다는 것을 빠르게 이해할 수 있어 이점이 있다.  

결론적으로, 정의역 위의 임의의 점 <img src="/tex/4d74936f278565f42f4bb42d6534712a.svg?invert_in_darkmode&sanitize=true" align=middle width=40.001773349999986pt height=14.15524440000002pt/>에서의 도함수 값은 다음과 같이 표현할 수 있다.

<p align="center"><img src="/tex/d9796def010540d6da483b626aa8fbfc.svg?invert_in_darkmode&sanitize=true" align=middle width=198.81965399999999pt height=34.0431762pt/></p>

## 2.6 임의의 점에서 미분이 가능하지 않을 때

임의의 점에서 미분은 가능하지 않다. 그러면 그 점에서 접선은 존재하지 않는다는 것이다. 접선을 구하는 방식이 기억이 나는가?  

곡선 위의 점 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>와 <img src="/tex/1afcdb0f704394b16fe85fb40c45ca7a.svg?invert_in_darkmode&sanitize=true" align=middle width=12.99542474999999pt height=22.465723500000017pt/>가 있을 때, <img src="/tex/1afcdb0f704394b16fe85fb40c45ca7a.svg?invert_in_darkmode&sanitize=true" align=middle width=12.99542474999999pt height=22.465723500000017pt/>를 점점 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>로 가까이 곡선 위로 움직였다. `three-step rule`에서는 <img src="/tex/5dc642f297e291cfdde8982599601d7e.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>번째 동작이다.

이 때, <img src="/tex/1afcdb0f704394b16fe85fb40c45ca7a.svg?invert_in_darkmode&sanitize=true" align=middle width=12.99542474999999pt height=22.465723500000017pt/>를 점점 <img src="/tex/df5a289587a2f0247a5b97c1e8ac58ca.svg?invert_in_darkmode&sanitize=true" align=middle width=12.83677559999999pt height=22.465723500000017pt/>로 가까이 움직일 때 평균변화율의 좌극한과 우극한이 같지 않다. 아래 함수를 보자.

<p align="center"><img src="/tex/98cbb170d1a4d0c961706a5444cd86de.svg?invert_in_darkmode&sanitize=true" align=middle width=100.75330154999999pt height=16.438356pt/></p>

위 절대값을 조건 방정식으로 표현하면 다음과 같다.  

<p align="center"><img src="/tex/e717addd32463514950da3cce0c562a1.svg?invert_in_darkmode&sanitize=true" align=middle width=203.52704625pt height=49.315569599999996pt/></p>

V 형태의 그래프가 된다. 아래는 <img src="/tex/d343a5beaabde2410ecf9f826344ed83.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=24.65753399999998pt/> 함수의 도함수이다. 

<p align="center"><img src="/tex/880901fee25c0114a00ffcb1b7f6fc80.svg?invert_in_darkmode&sanitize=true" align=middle width=323.63467454999994pt height=34.7253258pt/></p>

아래는 평균변화율의 우극한이다.  

<p align="center"><img src="/tex/ad0cba3567648d6b3ccb041d1a67211d.svg?invert_in_darkmode&sanitize=true" align=middle width=216.74880974999996pt height=35.422053149999996pt/></p>

아래는 좌극한이다. <img src="/tex/3919bbc84b8079e27194efe99a1f6a80.svg?invert_in_darkmode&sanitize=true" align=middle width=23.09366069999999pt height=22.465723500000017pt/>는 음수의 값에서 부터 <img src="/tex/29632a9bf827ce0200454dd32fc3be82.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>으로 다가오니, 절대값 기호를 벗음과 동시에 음수 기호를 붙여줘야한다.

<p align="center"><img src="/tex/f9786d57fc02a1b559fa65cd19e05faf.svg?invert_in_darkmode&sanitize=true" align=middle width=242.68492874999998pt height=35.422053149999996pt/></p>

이로써 <img src="/tex/f41f51aeb9528548f1409a3a0ec61640.svg?invert_in_darkmode&sanitize=true" align=middle width=39.53182859999999pt height=21.18721440000001pt/>에서의 접선 기울기가 왼쪽에서 좁혀질 때와 오른쪽에서 좁혀질 때가 다르므로 <img src="/tex/034d0a6be0424bffe9a6e7ac9236c0f5.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/>에서의 미분은 가능하지 않다.  

함수 하나를 더보자.  

<p align="center"><img src="/tex/cde420a092762ad4052fece7695602e4.svg?invert_in_darkmode&sanitize=true" align=middle width=101.92907999999998pt height=16.438356pt/></p>

이때, <img src="/tex/2f3c8b04b987706450f80c5b0c2619d4.svg?invert_in_darkmode&sanitize=true" align=middle width=39.53182859999999pt height=21.18721440000001pt/>에서 미분 가능하지 않음을 보일 수 있겠는가?  

<p align="center"><img src="/tex/76625d214d11d21d199d0d2dc1b0f77a.svg?invert_in_darkmode&sanitize=true" align=middle width=366.81952559999996pt height=34.7253258pt/></p>

나머지 증명은 독자들에게 맡긴다.   


## 2.8Last 극한과 연속 함수

아래 표현식을 보자. 

<p align="center"><img src="/tex/d6546e43eb99945b3ccefd9d287032e4.svg?invert_in_darkmode&sanitize=true" align=middle width=95.53215209999999pt height=22.1917806pt/></p>

<img src="/tex/3993c02cec53cc98f949aaaf2660c48e.svg?invert_in_darkmode&sanitize=true" align=middle width=43.65474299999999pt height=14.15524440000002pt/>로 갈 때, 함수 <img src="/tex/7997339883ac20f551e7f35efff0a2b9.svg?invert_in_darkmode&sanitize=true" align=middle width=31.99783454999999pt height=24.65753399999998pt/>의 값은 <img src="/tex/ddcb483302ed36a59286424aa5e0be17.svg?invert_in_darkmode&sanitize=true" align=middle width=11.18724254999999pt height=22.465723500000017pt/>이라는 것이다. 이는 <img src="/tex/886d8745cc716220e2963fa72ced709e.svg?invert_in_darkmode&sanitize=true" align=middle width=64.39687319999999pt height=24.65753399999998pt/>을 뜻하는 것은 아니다.  
처음 접선의 기울기 값을 구할 때 평균 변화율 <img src="/tex/7df4fe65623bdea4c58bf07cff4218d9.svg?invert_in_darkmode&sanitize=true" align=middle width=53.660747249999986pt height=24.65753399999998pt/>에서 <img src="/tex/64dadaf5586e074754ccb8a3a4027bb1.svg?invert_in_darkmode&sanitize=true" align=middle width=56.88346949999999pt height=22.465723500000017pt/>을 수행할 때에도 <img src="/tex/3919bbc84b8079e27194efe99a1f6a80.svg?invert_in_darkmode&sanitize=true" align=middle width=23.09366069999999pt height=22.465723500000017pt/>와 <img src="/tex/29632a9bf827ce0200454dd32fc3be82.svg?invert_in_darkmode&sanitize=true" align=middle width=8.219209349999991pt height=21.18721440000001pt/> 간에는 여전히 구별할만한 어떤 것이 있다고 하였다.  
또, 다음 절대값 함수 <img src="/tex/18077011250e633f523b93a29c0595af.svg?invert_in_darkmode&sanitize=true" align=middle width=49.09427324999999pt height=24.65753399999998pt/>의 <img src="/tex/8436d02a042a1eec745015a5801fc1a0.svg?invert_in_darkmode&sanitize=true" align=middle width=39.53182859999999pt height=21.18721440000001pt/>에서의 평균 변화율 <img src="/tex/7ecefac5f7fd3977519dcb49d96c4f86.svg?invert_in_darkmode&sanitize=true" align=middle width=63.53897714999999pt height=24.65753399999998pt/>에서 <img src="/tex/64dadaf5586e074754ccb8a3a4027bb1.svg?invert_in_darkmode&sanitize=true" align=middle width=56.88346949999999pt height=22.465723500000017pt/>가 하나의 값으로 결정할 수 없는 것과도 상관이 있다. <img src="/tex/05dfe2f6f8e76bbd4b2a244a2b5b4c98.svg?invert_in_darkmode&sanitize=true" align=middle width=32.22610874999999pt height=24.65753399999998pt/>가 음수 또는 양수 방향에서 구별할만한 어떤 것을 가지는가에 따라 절대값 기호가 달라지기 때문이다.   

더 적극적인 설명을 돕기 위해 다음 함수를 제시해 본다.  

<p align="center"><img src="/tex/e2bc5087150da94338164603f41b91c9.svg?invert_in_darkmode&sanitize=true" align=middle width=87.0142713pt height=35.77743345pt/></p>

위 식은 다음과 같이 쓸수 있다.

<p align="center"><img src="/tex/eed747b2b151ce32a0c39284d69bb774.svg?invert_in_darkmode&sanitize=true" align=middle width=170.86342514999998pt height=14.611878599999999pt/></p>

<img src="/tex/a9ef45be1cd9cd2165b8ebbb2a779178.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=24.65753399999998pt/>에서 분모가 0이 될 수없으므로, <img src="/tex/cf330257519e06f13c2ecab5e25c6d2a.svg?invert_in_darkmode&sanitize=true" align=middle width=21.00464354999999pt height=24.65753399999998pt/>은 적절한 변환이다. <img src="/tex/863fe9d743c4a80a527803b7229ae3ad.svg?invert_in_darkmode&sanitize=true" align=middle width=43.184798249999986pt height=21.18721440000001pt/>일 때, <img src="/tex/deceeaf6940a8c7a5a02373728002b0f.svg?invert_in_darkmode&sanitize=true" align=middle width=8.649225749999989pt height=14.15524440000002pt/>의 값은 어떻게 변하겠는가?  

<p align="center"><img src="/tex/8283e55704086c0f16183bdbb1b67ab8.svg?invert_in_darkmode&sanitize=true" align=middle width=217.5690561pt height=32.990165999999995pt/></p>

<p align="center"><img src="/tex/4290d930b6c6325e1c36649003a37c70.svg?invert_in_darkmode&sanitize=true" align=middle width=234.00746985pt height=32.990165999999995pt/></p>

<p align="center"><img src="/tex/d7ae2b4eb17532e2f6ef6c80e8e639c1.svg?invert_in_darkmode&sanitize=true" align=middle width=250.44588194999997pt height=32.990165999999995pt/></p>

<p align="center"><img src="/tex/0e33747f7a0b2185dcd42160d33f4b54.svg?invert_in_darkmode&sanitize=true" align=middle width=31.963567349999998pt height=1.7351598pt/></p>


<p align="center"><img src="/tex/9e5c5e064944b8944939f6689fe5b144.svg?invert_in_darkmode&sanitize=true" align=middle width=89.4861231pt height=16.438356pt/></p>

