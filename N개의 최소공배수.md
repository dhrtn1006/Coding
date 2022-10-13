문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/12953

사용 언어 : Javascript

풀이 내용 :

```
function solution(arr) {
    let calc = arr[0];
    for (i=1;i<arr.length;i++) {
        let numA = calc;
        let numB = arr[i];
        while (numB > 0) {
            const r = numA % numB;
            numA = numB;
            numB = r;
        }
        calc = arr[i] * calc / numA;
    }
    return calc;
}
```