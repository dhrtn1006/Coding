문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/42748

사용 언어 : Javascript

풀이 내용 :

```
function solution(array, commands) {
    let answer = [];
    for (let item of commands)
        answer.push((array.slice(item[0]-1, item[1]).sort((a, b) => a - b))[item[2]-1]);
    return answer;
}
```