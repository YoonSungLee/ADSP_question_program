# ADSP_question_program

해당 repository는 ADSP 자격증을 준비하면서 주관식 문제에 대한 대비를 하기 위해 만든 프로그램이다. 간단하게 구성된 프로그램이고 내가 필요로 하거나 헷갈린 문제로만 구성이 되어있지만, 혹여나 이러한 프로그램을 만들 시간이 없어서 필요로 하는 유저에게 도움이 되고자 소스를 공개한다.

# Requriements

numpy==1.18.1


# Implement

ADSP_question_program.ipynb 파일을 실행한다. 크게 exam() 함수와 exam_all() 함수로 구성되어 있다.

### exam()

<img src="https://i.imgur.com/O4lp8Rc.png" width="100%">
exam() 함수는 모든 문제에서 복원추출로 문제를 뽑아 무한적으로 문제를 푸는 형식으로 코드를 구현했다.
<br>

### exam_all()

<img src="https://i.imgur.com/DtBHew6.png" width="100%"> exam_all() 함수는 모든 문제에서 비복원추출로 문제를 뽑아 한 번씩 문제를 푸는 형식으로 코드를 구현했다.
<br>

### Implement

<img src="https://i.imgur.com/xsJBHgA.png" width="100%"> 해당 문제를 맞추면 위 그림과 같이 '정답'으로 표기되고 다음 문제로 넘어간다.
<br>

<img src="https://i.imgur.com/3cwTTfG.png" width="100%"> 해당 문제를 못맞추면 위 그림과 같이 '오답, 다시 입력하세요'로 표기되고 다시 문제를 풀 기회를 준다.
<br>

<img src="https://i.imgur.com/Nsd32k5.png" width="100%"> 해당 문제에 대한 정답을 모른다면, 'pass'를 입력할 수 있다. pass를 입력하면 위 그림과 같이 정답을 알려주고 문제가 넘어간다(have to check 아래에서 확인 가능). 특히 exam_all() 함수를 실행할 경우, pass로 넘어간 문제는 해결한 문제에 카운트되지 않으며 나중에 다시 랜덤으로 문제가 등장한다.
<br>

<img src="https://i.imgur.com/nRcGNnN.png" width="100%"> exam_all()은 문제를 모두 통과하면 자동으로 프로그램이 종료된다. 만약 exam()을 사용하거나 또는 문제를 종료하고 싶다면 'exam'을 입력할 수 있다. exam을 입력하면 위 그림과 같이 프로그램이 종료된다.
<br>

### Modification

<img src="https://i.imgur.com/44LnYOU.png" width="100%"> 만약 문제를 추가, 수정, 삭제를 하고 싶다면 프로그램의 'question_answer' 딕셔너리를 통해 수정할 수 있다. 이 때 추가할 문제의 형식은 '문제':'답' 과 같이 딕셔너리 형태로 구성되어야 하고, 문제와 문제 사이에 콤마(,)를 잊지 않도록 주의하도록 한다.
<br>

<img src="https://i.imgur.com/BQTyacs.png" width="100%"> 만약 pycharm 환경에서 프로그램을 실행시키고 싶다면 ADSP_question_program.py 파일을 실행한다. 위의 그림과 같이 프로그램을 실행시킬 수 있으며, 원하는 함수의 주석(#)을 풀고 프로그램을 실행시키면 된다.
<br>

### Comments

만약 해당 프로그램에 관하여 문의사항이 있으면, 해당 repository의 Issue 또는 이메일(nowhere3070@naver.com)로 문의해주길 바란다.
