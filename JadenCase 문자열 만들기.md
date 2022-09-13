문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/12951

사용 언어 : Javascript

풀이 내용 :

```
function solution(s) {
    return s.split(" ").map(e => e.charAt(0).toUpperCase() + e.substr(1).toLowerCase()).join(" ");
}
```