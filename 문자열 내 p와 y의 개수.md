문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/12916

사용 언어 : Javascript

풀이 내용 :

```
function solution(s){
    return s.replace(/(?!Y|y)./g, "").length === s.replace(/(?!P|p)./g, "").length ? true : false;
}
```