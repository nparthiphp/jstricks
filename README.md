# JS Tricks
Javascript behaves differently oppose to our understanding.

## Numbers
```
var a = 10;
a.toFixed(2); // "10.00"
```
### Tricky Benahviour 
```
10.toFixed(2); // Syntax error
```
Reason is, when javascript compiles the above code differently. 
```
var a = 10.0;
var b = 10;
a === b //true
```
Therefore 10. will consider as a 10 only. So . property operator will not be available. 

### Soultion
```
10..toFixed(2);
10 .toFixed(2);
```



 
