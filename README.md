## 전국 청소년 모의해킹 대회 Write Up 
2018년 6월 17일 디미고에서 주최하는 CTF 해킹 대회가 있다. </br>
이 글의 작성자는 예선을 통과를 하든 안하든 Github에 Write UP을 작성할것이다. 

## EZPZ
EZPZ는 hex로 뜯어서 하는 문제 이다. 문제파일이 .exe 형식이여서 비주얼로도 해보고 윈도우도 해봤지만 hex가 정답이다. </br>
hex에서 dimi라고 적힌 글자를 찾아보면 아마 아래와 같은 부분이 나올것이다. </br>
<pre>
  #Welcome_reversing dimi{ }  button1 GO INPUT EZ3EZPZ.Properties.Resources
</pre>
사실 이거는 그냥 속임수 알고 넘겼는데 사실 여기서 답이 있었다. </br>
위에 dimi 라고 적힌것 위에 #Welcome_reversing이 나와있고 아래에는 GO INPUT 이라고 적혀 있는것을 확인하고 #Welcome_reversing을 dimi{ } 안에 넣어서 최종적인 flag를 얻을수가 있었다. ~~개빡치는문제중하나..~~ </br>
이게 좀 빡친 이유가, 진짜 보기에는 별거 없고 문제도 exe파일 이여서 윈도우 파일로 뜯어야 할거 같아서 이거저거 해봤는데 아니 그냥 진짜 애초에 차분히 보면 되는 문제 였음; 아무튼 결론적으로 Flag는 <strong> dimi{#Welcome_reversing} </strong> 입니다.

## init
init은 문제에서 nc 주소를 제공을 해준다. 이에 접속 접속으로 하면 <strong> [W]rite / [R]ead / [E]xit </strong> 이 나온다. </br>
init은 솔직히 노가다 입니다. 이거저거 다 입력해보면서 알아가야 합니다. ~~근데 이거 작년에 다 해야했는데 다 못해서 올해 까지 작성중이다;;~~ </br>
<strong> [W]rite </strong> 으로 들어가서 100을 입력해주면 어느순간 우엑 하면서 오버플로우 때문인지 답을 보여줍니다. </br>
그래서 놀랍게도 Flag는 </br>
<strong> dimi{A110cAt3_1s_$o_1mp0rt@n7} </strong> 입니다. </br>

## WINrps
이 문제 내 기억 맞으면 진짜 시간 얼마 안남았을때 풀었던 걸로 기억을 하는데, 이거도 은근 빡치는 문제. </br>
Google Drive 링크를 하나 준다. 링크에는 rsp.apk 파일을 제공해줌. 자 이게 문제인데 </br>
일단 첫번째로 안드로이드 기기 (가상 기기 포함) 있어야 한다. 나는 안드로이드 기기가 없었기에 <a href="https://kr.bignox.com/">Nox</a>를 이용해서 가상 머신으로 돌렸다. </br>
이 apk는 가위바위보 게임인데 게임에 980414을 이겨야지 Flag을 얻을수 있음 </br>
그러고 과거에 사용해봤던 CheatEngine 라는 툴을 이용해서 rsp.apk 안에 있는 함수 값 혹은 변수 값을 980414 이상으로 올리고 나서 확인을 했다. </br>
후 결론적으로 Flag는 Flag{Are_you_Genius_or_Stupid?} 이라는 것을 받았다. </br>
<strong> flag{Are_you_Genius_or_Stupid?} </strong> </br>
아 참고로 이 문제 같은 경우에는 플래그 형식이 
<pre>
  flag{ }
</pre> 
로 되었다. 


## Contact me
----------------------------------------
If you have problem about this code, then contect me. </br>
Email : insung.park123@gmail.com </br>
Facebook : https://www.facebook.com/insung.bahk </br>
</br>
If you want to give me some money... Please money send here! </br>
Bitcoin : 17qKUu57aUBcvx9T1ea8Ga87EPnDdmwAEP </br>
Ether : 0xdFE8D1536deE8F839Ede7c1f3A0c44116287D931  
Bitcoin Cash : qp90gf09r3y3h06czmtnsfhz9w7s90se4s72vd9pam </br> 
</br>
🙇‍♀️👾🤩Thank you! 🤩👾🙇‍♂️ 
----------------------------------------
