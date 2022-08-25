문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/12954

사용 언어 : Javascript

풀이 내용 :

```
function solution(x, n) {
    return Array(n).fill(x).map((val, index) => val += x * index);
    
    // 재귀를 이용한 풀이
    // const arr = String(x).split(",");
    // return arr.length === n ? arr.map(Number) : solution(x + "," + (arr[0] * (arr.length + 1)), n);
}
```