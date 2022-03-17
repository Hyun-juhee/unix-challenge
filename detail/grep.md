# grep

```
$ grep [OPTION] [PATTERN] [FILE]
```

```
$ 내용을_출력하는_명령어 | grep [OPTION] [PATTERN] [FILE]
```

### 사용 예시

| grep 사용 예                                           | 명령어 옵션 |
|--------------------------------------------------| ---------|
| 대상 파일에서 문자열 검색                                      | `grep "STR" [FILE]` |
| 현재 디렉토리 모든 파일에서 문자열 검색     |`grep "STR" * `             |
| 특정 확장자를 가진 모든 파일에서 문자열 검색     |`grep "STR" *.ext`       |
| 대소문자 구분하지 않고 문자열 검색 |   `grep -i "STR" [FILE] `        |
| 매칭되는 PATTERN이 존재하지 않는 라인 선택     |`grep -v "STR" [FILE]` |
| 단어(Word) 단위로 문자열 검색     |`grep -w "STR" [FILE]`         |
| 검색된 문자열이 포함된 라인 번호 출력     |`grep -n "STR" [FILE]`       |
| 하위 디렉토리를 포함한 모든 파일에서 문자열 검색     |`grep -r "STR" *`      |
| 최대 검색 결과 갯수 제한     |`grep -m 100 "STR" FILE`            |
| 검색 결과 앞에 파일 이름 표시     |`grep -H "STR" * `               |
| 문자열 A로 시작하여 문자열 B로 끝나는 패턴 찾기     |`grep "A.*B" *`       |
| 0-9 사이 숫자만 변경되는 패턴 찾기 |    `grep "STR[0-9]" * `         |

### grep 활용
grep은 옵션도 많고 활용도 많은데, 다 쓸거 같지는 않다. 
평소에 쓰이는 몇가지만 외워두고 활용하자
```
ifconfig | grep "inet"
```

ifconfig로 출력된 내용 중, inet 찾기 

```
 kubectl get no | grep data-app
```
`kubectl get no`로 출력한 내용 중, data-app 관련 내용 찾기 
