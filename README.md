# 디미고 청소년 CTF 해킹 대회 Write Up 문서
2018년 6월 17일 디미고에서 주최하는 CTF 해킹 대회가 있다. </br>
이 글의 작성자는 예선을 통과를 하든 안하든 Github에 Write UP을 작성할것이다. 

# EZPZ
EZPZ는 hex로 뜯어서 하는 문제 이다. 문제파일이 .exe 형식이여서 비주얼로도 해보고 윈도우도 해봤지만 hex가 정답이다. </br>
hex에서 dimi라고 적힌 글자를 찾아보면 아마 아래와 같은 부분이 나올것이다. </br>
<pre>
  #W e l c o m e _ r e v e r s i n g  d i m i {  }    b u t t o n 1  G O  I N P U T  E Z  3E Z P Z . P r o p e r t i e s . R e s o u r c e s
</pre>
사실 이거는 그냥 속임수 알고 넘겼는데 사실 여기서 답이 있었다. </br>
위에 dimi 라고 적힌것 위에 #W e l c o m e _ r e v e r s i n g이 나와있고 아래에는 G O  I N P U T 이라고 적혀 있는것을 확인하고 #W e l c o m e _ r e v e r s i n g을 dimi{ } 안에 넣어서 최종적인 flag를 얻을수가 있었다. ~~개빡치는문제중하나..~~ </br.

