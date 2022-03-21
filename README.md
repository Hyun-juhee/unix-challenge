# unix-challenge
유닉스 명령어 너무 모르는 내 자신... 열받아 
매일 15분 공부 챌린지 시작 +_+

| No  | 명령어                                      | 역할                             | ex                                                                                 | 
|-----|------------------------------------------|--------------------------------|------------------------------------------------------------------------------------|
| 1   | `where 파일`                               | 위치 찾기                          | `where kubectl`                                                                    |
| 2   | `cp 대상_파일 생성할_파일`                        | copy                           | `cp Image.png ./test/img.png`                                                      |
| 3   | `mv 대상_파일 생성할_파일`                        | move                           | `mv Image.png ./test/img.png `                                                     |
| 4   | `rm 대상_파일`                               | remove                         | `rm img.png`                                                                       | 
| 5   | `mkdir 경로`                               | directory 생성                   | `mkdir ./testdir`                                                                  |
| 6   | `pwd`                                    | 현재 경로                          |                                                                                    |
| 7   | `find 경로 -name 파일명`                      | 파일 검색                          | `find ./testdir -name 'b.*' -size 0 ` <br/>testdir 디렉토리에서 이름이 b, 확장자는 전체, size는 0인 파일 검색 |
| 8   | [`greb [옵션] 이거_찾아 파일`](./detail/grep.md) | 파일 내에 원하는 부분 찾기                |                                                                                    |
| 9   | `ls -al`                                 | -a : 숨은 파일까지 보기<br/> -l : 상세보기 |                                                                          |
| 10  |                                          | 파이프, 결과를 다음 명령어의 입력으로 넘김       | `ifconfig / grep "inet"`                                                   |
| 11  | `alias 단축명령어='명령어'`                      | 명령어 단축해서 사용하기                  | `alias ls='ls -al'`              |
| 12  | [`chmod 옵션 대상_파일`](./detail/chmod.md)    | 파일에 대한 접근 권한 변경                | `chmod 755 hosts`              |