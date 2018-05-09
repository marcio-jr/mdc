# mdc
simple MDC algorithm

Recursive:
```C
  MDC (a, b){
    if (b==0) return a;
    else return MDC(b, a%b);
  }
 ```
  
Non recursive:
```C
  MDC (a, b){
    while (b!=0){
      r = a%b;
      a = b;
      b = r;
    }
    return a;
  }
```
