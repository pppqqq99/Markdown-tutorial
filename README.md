# Markdown-tutorial 프로젝트 시나리오

https://github.com/pppqqq99/Markdown-tutorial

* 하나의 markdown-tutorial을 두 명의 플레이어가 git과 GitHub를 활용하여 함께 만들기로 하였다. 최종 산출물은 하나의 md파일에 Markdoen tutorial 문서이다.


1. 첫 번째 플레이어(git을 잘못 이해한 플레이어)의 첫 번째 작업 - markdown tutorial을 만들기 위해 목차를 세우고 각 목차의 내용을 다른 파일에 담아서 마지막에 통합하려고 한다.

2. 두 번째 플레이어(git을 올바르게 이해한 플레이어)의 작업 - 첫 번째 플레이어가 git을 잘못 이해하여 여러 개의 산출물이 나오는 방향으로 흘러간다는 사실을 깨닫고 master branch를 clone하여 하나의 통합 파일로 수정하여 markdown tutorial을 완성한다.

3. 첫 번째 플레이어의 두 번째 작업 - 첫 번째 플레이어가 pull하여 변경된 파일을 읽게 된다. 자신이 잘 못 만들었다는 것을 깨닫게 되고 이 프로젝트에 기여한기 위해 GFM부분을 수정하여 완성한다.

4. 두 번째 플레이어의 두 번째 작업 - 두 번째 플레이어가 다른 pc로 player1's final을 확인하고 GFM부분을 분리하는 수정을 하였다가 파일을 하나로 만들어야 하기 때문에 다시 reset을 한 후 player1's final에 tag를 붙이며 프로젝트를 마친다.


## 첫 번째 플레이어의 첫 번째 작업  


1. markdown tutorial이라는 폴더를 생성 한 후 contents라는 파일 생성 후 commit
- init : 빈 git 저장소가 만들어짐 – 이 폴더가 git의 관리 하에 들어감
![init](https://user-images.githubusercontent.com/64363668/117330796-0332f080-aed1-11eb-8716-d2abe8cdab42.PNG)
- config : 현재 설정된 Git 설정 확인하기 
config —global : 이름과 이메일 등록- git 저장소를 제어하는데 필요한 정보
![config --global](https://user-images.githubusercontent.com/64363668/117330886-1ba30b00-aed1-11eb-99eb-677b587a1dac.PNG)
- status : 현재 폴더에서 파일들의 상태들을 알려주는 명령어
- ![status](https://user-images.githubusercontent.com/64363668/117331000-43926e80-aed1-11eb-9dc9-ac30a2f98221.PNG)
- add : 작업 디렉토리 상의 변경 내용을 스테이징 영역에 추가하는 명령어
add -A : commit되지 않은 파일들을 commit가능하게 변경  
![add -A](https://user-images.githubusercontent.com/64363668/117331055-51e08a80-aed1-11eb-8589-4cbfc70380b3.PNG)
- commit : 작업한 파일의 변경사항을 하나의 시점에서 캡슐화 시키는 명령어
commit -m "A" : "A"이라는 이름의 commit을 생성  
![commit -m](https://user-images.githubusercontent.com/64363668/117331102-5e64e300-aed1-11eb-87fc-f3180a2c9464.PNG)


2. master branch에서 contents-detail이라는 branch를 생성 한 후 heading이라는 파일을 commit
- branch : 한 시점에서 분기하여 독립적으로 어떤 작업을 할 수 있게 만드는 명령어
branch A : A라는 이름의 branch를 생성
![branch](https://user-images.githubusercontent.com/64363668/117331149-6e7cc280-aed1-11eb-8ced-ca3ad57828b9.PNG)

3. master branch에 contents-detail을 merge함
- merge : 병합
merge A : 현재 위치한 branch에 A라는 이름의 branch를 병합
![merge](https://user-images.githubusercontent.com/64363668/117331283-93713580-aed1-11eb-8c58-41a4132bc3a0.PNG)

4. master branch에서 contents-linebreaks라는 branch 생성 후 linebreaks라는 파일을 commit
checkout : branch 목록을 보여줌
checkout A : A라는 이름의 branch로 이동
![checkout](https://user-images.githubusercontent.com/64363668/117331224-82c0bf80-aed1-11eb-858f-5184bc578b91.PNG)


5. master branch로 다시 checkout한 후 pragraphs라는 파일을 commit

6. master branch에 contenst-linebreaks를 rebase함
- rebase A : 현재 위치한 branch에 A라는 이름의 branch를 병합. merge와 같이 branch를 병합하는 명령어 이지만 Merge는 branch를 통합하는 것이고 Rebase는 branch의 base를 옮긴다는 개념의 차이가 있음.
![rebase](https://user-images.githubusercontent.com/64363668/117331326-9e2bca80-aed1-11eb-8f49-5a4eceb31200.PNG)

7. 이후 github의 원격 repository인 origin에 master branch를 push함
- remote : 현 폴더의 원격 repository를 확인하는 명령어
remote add origin '주소' : '주소'의 repository를 origin이란 이름의 원격 저장소로 설정하겠다는 의미. 
![github에 업로드 remote push-u](https://user-images.githubusercontent.com/64363668/117331414-b1d73100-aed1-11eb-9ef3-8fad67e04192.PNG)



## 두 번째 플레이어의 첫 번째 작업  

1. repository의 내용을 clone 함
- clone : 원격 repository에 있는 branch를 복사하여 다른 곳에서 사용하는 명령어

![clone](https://user-images.githubusercontent.com/64363668/117331557-d59a7700-aed1-11eb-893b-814683656a30.PNG)

2. integrate file이라는 파일 생성하여 분할되어 있던 파일들을 하나의 file로 만들고 그 과정에서 여러번의 commit을 하여 기록을 남김

3. push하여 본인의 작업 내용을 업로드 함 
- push : 원격 repository에 변경된 사항들을 업로드
![push 2](https://user-images.githubusercontent.com/64363668/117331619-e814b080-aed1-11eb-91ef-c0cc7808d052.PNG)



## 첫 번째 플레이어의 두 번째 작업

1. pull하여 본인의 작업 파일에 두 번째 플레이어가 작업한 내용을 최신화 시킴
- pull : git서버에서 최신화된 파일들을 가져와 병합하는 명령어
![pull](https://user-images.githubusercontent.com/64363668/117331675-f662cc80-aed1-11eb-8f56-5614c61c6f24.PNG)

2. 두 번째 플레이어가 작성한 파일에 내용을 추가함

3. push하여 본인의 작업 내용을 업로드 함



## 두 번째 플레이어의 두 번째 작업

1. 다른 pc에서 작업한다고 가정하여 repository의 내용을 clone함

2. GFM파일을 만들어서 commit함

3. 파일을 분할하면 안된다는 사실을 깨닫고 log를 통해 본인의 작업을 확인한 후 되돌리기 위해 reset함
- log : commit 히스토리 
log --graph --all --decorate : 프로젝트의 commit들과 branch의 관계도를 나타냄
 ![log --graph --all --decorate](https://user-images.githubusercontent.com/64363668/117331879-24e0a780-aed2-11eb-82d4-31590e042dcb.PNG)

- reset : 이전 commit으로 되돌리기
reset 일련번호 --hard : 일련번호에 해당하는 commit으로 되돌리고 그 이후의 commit들은 삭제한다.
![reset](https://user-images.githubusercontent.com/64363668/117331820-15615e80-aed2-11eb-9f19-5959e0cbf6aa.PNG)

4. tag를 붙여 첫 번째 플레이어의 두 번째 작업 파일이 최종 산출물이라는 내용을 tag함
- tag : commit에 이름을 붙여주는 명령어
![tag](https://user-images.githubusercontent.com/64363668/117331861-1e523000-aed2-11eb-9ed1-f8cd5ed72980.PNG)

|    명령어    |    사용여부    |              링크             |
| :---------: | :----------:   | :---------------------------: |
|  add        | O | |
|  branch | O | |
|checkout| O | |
|clone| O | |
|commit| O | |
|config| O | |
|init | O | |
|log| O |[log](#log) |
|merge| O | |
|pull| O| |
|push| O| |
|rebase| O | |
|remote|O| |
|reset --hard|O| |
|status| O | |
|tag| O | |
