문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/42747

사용 언어 : Javascript

풀이 내용 :

```
function solution(citations) {
    let HIndex = 0;
    citations.sort((a, b) => b - a);
    
    for (i=0;i<citations.length;i++) {
        if (HIndex >= citations[i]) break;
        HIndex++;
    }
    return HIndex;
}
```