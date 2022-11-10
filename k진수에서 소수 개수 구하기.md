문제 링크 : https://school.programmers.co.kr/learn/courses/30/lessons/92335

사용 언어 : Javascript

풀이 내용 :

```
function solution(n, k) {
    const number = n.toString(k);
    const numberArr = number.split("0");
    
    return numberArr.reduce((acc, cur) => setPrimeNumber(cur * 1) ? acc + 1 : acc, 0);
}

function setPrimeNumber(num) {
    let isPrime = true;
    for (i=2;i<=Math.floor(Math.sqrt(num));i++){
        if (num % i === 0) isPrime = false;
    }
    return num && num !== 1 ? isPrime : false;
}
```