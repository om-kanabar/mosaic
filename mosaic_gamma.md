```math
D = \{x^{(1)}, x^{(2)},...,x^{(n)}\}
```
```math
x_m = [x^{(1)}_m, x^{(2)}_m,...,x^{(n)}_m]
```
```math
m = 2, 3,...,T-1
```
```math
x^{(i)}_m \sim \text{Uniform}(x_m)
```
```math
a_m = \left[ x^{(j)}_{m+1} - x^{(i)}_m \;\middle\vert{}\; j = 1, 2, \dots, n \right]
```

```math
a^{(m)} \sim \text{Uniform}(a_m)
``` 
```math
z^{(i)}_1 = x^{(i)}_1
```
```math
z^{(i)}_{m+1} = a^{(m)}+z^{(i)}_m
```
```math
z^{(i)} = [z^{(i)}_1,...,z^{(i)}_m, z^{(i)}_{m+1},...,z^{(i)}_T]
```