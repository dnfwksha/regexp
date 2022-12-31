# 정규표현식(RegExp)

정규식, Regular Expression

## 역할

- 문자검색(search)
- 문자 대체(replace)
- 문자 추출(extract)

## 테스트 사이트
1. https://regex101.com/
2. https://regexr.com/
3. https://regexper.com/

## 정규식 생성
//생성자
```js
//생성자
new RegExp('표현','옵션')
new RegExp('[a-z]','gi')

//리터럴
/표현/옵션
/[a-z]/gi

g -> 모든 곳에서 단어 찾기
i -> 대소문자 구분 없이 단어 찾기
```

## 예제 문자

```js
const str = `
010-1234-5678
thesecon@gmail.com
https://www.omdbapi.com/?apikey=7035c60c&s=frozen
The quick brown fox jumps over the lazy dog.
abbcccdddd
`
```

## 메소드

메소드 | 문법 | 설명
---|---|---
test|`정규식.test(문자열)`|일치 여부(Boolean) 반환
match|`문자열.match(정규식)`|일치하는 문자의 배열(Array) 반환
replace|`문자열.replace(정규식, 대체문자)`|일치하는 문자를 대체

## 플래그(옵션)

플래그|설명
--|--
g|모든 문자 일치(global)
i|영어 대소문자를 구분 않고 일치(ignore case)
m|여러 줄 일치(multi line)