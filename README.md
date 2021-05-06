# Markdown-tutorial 프로젝트 시나리오

https://github.com/pppqqq99/Markdown-tutorial

*하나의 markdown-tutorial을 두 명의 플레이어가 git과 GitHub를 활용하여 함께 만들기로 하였다. 최종 산출물은 하나의 md파일에 Markdoen tutorial 문서이다.


1. 첫 번째 플레이어(git을 잘못 이해한 플레이어)의 첫 번째 작업 - markdown tutorial을 만들기 위해 목차를 세우고 각 목차의 내용을 다른 파일에 담아서 마지막에 통합하려고 한다.

2. 두 번째 플레이어(git을 올바르게 이해한 플레이어)의 작업 - 첫 번째 플레이어가 git을 잘못 이해하여 여러 개의 산출물이 나오는 방향으로 흘러간다는 사실을 깨닫고 master branch를 clone하여 하나의 통합 파일로 수정하여 markdown tutorial을 완성한다.

3. 첫 번째 플레이어의 두 번째 작업 - 첫 번째 플레이어가 pull하여 변경된 파일을 읽게 된다. 자신이 잘 못 만들었다는 것을 깨닫게 되고 이 프로젝트에 기여한기 위해 GFM부분을 수정하여 완성한다.

4. 두 번째 플레이어의 두 번째 작업 - 두 번째 플레이어가 다른 pc로 player1's final을 확인하고 GFM부분을 분리하는 수정을 하였다가 파일을 하나로 만들어야 하기 때문에 다시 reset을 한 후 player1's final에 tag를 붙이며 프로젝트를 마친다.


* 첫 번째 플레이어의 첫 번째 작업
* https://github.com/pppqqq99/Markdown-tutorial/issues/1#issue-877675173
1. markdown tutorial이라는 폴더를 생성 한 후 내용이라는 파일 생성 후 commit
2. master branch에서 contents-detail이라는 branch를 생성 한 후 heading이라는 파일을 commit
3. master branch에 contents-detail을 merge함
4. master branch에서 contents-linebreaks라는 branch 생성 후 linebreaks라는 파일을 commit
5. master branch로 다시 checkout한 후 pragraphs라는 파일을 commit
6. master branch에 contenst-linebreaks를 rebase함
7. 이후 github의 원격 repository인 origin에 master branch를 push함


|    명령어    |    사용여부    |              링크             |
| :---------: | :----------:   | :---------------------------: |
|  add        | O | |
|  branch | O | |
|checkout| O | |
|clone| O | |
|config| O | |
|init | O |https://github.com/pppqqq99/Markdown-tutorial/issues/1#issue-877675173 |
|log| O | |
|merge| O | |
|pull| O| |
|push| O| |
|rebase| O | |
|remote|O| |
|reset --hard|O| |
|status| O | |
|tag| O | |
