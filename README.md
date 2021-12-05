# homework2_-vimgolf-

## 주로 사용한 vim 명령어
### 이동
|종류|설명|
|:---:|:---|
|G|파일의 마지막 줄로 이동|
|W|단어 단위 앞으로 이동(첫 공백까지 이동함)|
|End키|라인 끝으로 이동|
|/어떤 단어|예)/hello : hello가 적힌 곳을 찾음. n키와 N키로 이동할 수 있음|

### 입력
|종류|설명|
|:---:|:---|
|O|현재 라인의 앞쪽에 라인추가 후 입력모드 변환|
|i|현재 커서위치에서 입력모드 변환|
|a|현재 커서위치의 다음 커서 위치에서 입력모드 변환|
|cw|커서 뒤의 단어를 제거 후, 입력모드로 전환|
|Esc키|입력모드나 비주얼모드에서 명령어모드로 돌아올 때 사용|

### 복사,붙여넣기,수정,저장
|종류|설명|
|:---:|:---|
|yw|커서 뒤의 한 단어만 복사|
|Y|한 라인 복사(3Y처럼 nY꼴로 사용시, 현재 라인부터 n개의 라인 복사)|
|p|현재 라인 뒤에 복사한 내용 붙여넣음|
|P|현재 라인 앞에 복사한 내용 붙여넣음|
|x|커서 뒤의 한 문자를 지움(3x처럼 nx꼴로 사용시, 커서를 기준으로 n개의 문자 삭제)|
|r|한 문자를 수정(입력모드로 바뀌지 않음)|
|:%s/str/replace/g| 파일 전체에서 str을 replace로 수정("%"가 파일전체를 의미하는 듯. %이외에 라인 넘버를 입력하면, str을 찾는 범위가 그 라인넘버로 제한됨.)|
|ZZ|편집된 내용을 저장 후 종료|


#### %% 제가 보고 입력하기 편한대로 단계를 나눠놓았습니다 %%
## 문제1 ( vimgolf put 5f0f5fbe280fbf000c233304 ), 최고점: 8, 내 점수: 9
### <풀이>
<img src="https://github.com/baeg0pa/homework2_-vimgolf-/blob/main/solution_1.gif?raw=true" width="800" height="400">

1) G
2) W
3) i
4) "
5) [End키]
6) "
7) [Esc키]
8) ZZ


## 문제2 ( vimgolf put 603ba26a01b4d00009c10a49 ), 최고점: 19, 내 점수: 25
### <풀이>
<img src="https://github.com/baeg0pa/homework2_-vimgolf-/blob/main/solution_2.gif?raw=true" width="800" height="400">

1) W
2) cw
3) vim
4) [Esc키]
5) :%s/emacs/vim/g[엔터키]
6) ZZ
  
  
## 문제3 ( vimgolf put 5f1063aa8361810006e73210 ), 최고점: 20, 내 점수: 29
### <풀이>
<img src="https://github.com/baeg0pa/homework2_-vimgolf-/blob/main/solution_3.gif?raw=true" width="800" height="400">

1) 4G
2) yw
3) O
4) //[스페이스바]
5) Esc키
6) p
7) a
8) TODO 
9) [Esc키]
10) Y
11) 아래 방향키[DOWN]
12) p
13) 아래 방향키[DOWN]
14) yw
15) 위 방향키[Up]
16) W
17) P
18) 8x
19) ZZ
  
## 문제4 ( vimgolf put 9v0060da5177000000000209 ), 최고점: 34, 내 점수: 61
### <풀이>
<img src="https://github.com/baeg0pa/homework2_-vimgolf-/blob/main/solution_4.gif?raw=true" width="800" height="400">

1) :%s/y1/abs(y1)/g[엔터키]
2) :3s/1/2/g[엔터키]
3) :4s/1/3/g[엔터키]
4) :5s/1/4/g[엔터키]
5) /k[엔터키]
6) rgn
7) nrb
8) nrr
9) ZZ

## 문제5 ( vimgolf put 6013804df3308e0009368f1c ), 최고점: 19, 내 점수: 27
### <풀이>
<img src="https://github.com/baeg0pa/homework2_-vimgolf-/blob/main/solution_5.gif?raw=true" width="800" height="400">

1) 5G 
2) yw
3) [PageDown] 아니면 G
4) 위 방향키 [Up]
5) [End키]
6) P
7) a
8) ,name,age,score
9) [Esc키]
10) ZZ
