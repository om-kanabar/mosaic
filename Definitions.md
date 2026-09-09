# Definitions

### Symbol : Meaning

$`D`$ : TokaMark Dataset

$`D'`$ : Dataset of synthesized data

$`N`$ : Number of samples in $`D`$

$`x^{(i)}`$ : Sample $`i`$ in $`D`$

$`x^{(j)}`$ : Sample $`j`$ in $`D`$

$`U`$ : List of already used pairs of $`\{i,j\}`$.

$`P`$ : $`D-U`$ : List of unused samples in $`D`$

$`s^{(i)}`$ : The starting state of sample $`x^{(i)}`$

$`x_m^{(i)}`$ :  the $m$ᵗʰ observation in $`x^{(i)}`$

$`T`$ : The fixed sample length in terms of amount of observations .

$`k`$ : Split index in the first sample

$`r`$ : Split index in the second sample

$`w`$ : Comparison window length used by Mosaic to determine $`r`$

$`z^{(i)}`$ : the $`i`$ᵗʰ synthetic sample made by Mosaic

$`z_m^{(i)}`$ : The $`m`$ᵗʰ observation in synthetic sample $`z^{(i)}`$

$`L`$ : Number of generated samples the user wants

# Example Data

### Example Dataset

```math
D = \{x^{(1)},x^{(2)},...,x^{(N)}\}
```

### Example Sample

```math
x^{(i)} = (x_1^{(i)},x_2^{(i)},...,x_T^{(i)})
```

### Example Synthetic Dataset

```math
D'= \{z^{(1)},z^{(2)},...,z^{(L)}\}
```

### Example Synthetic Sample

```math
z^{(i)} = (z_1^{(i)},z_2^{(i)},...,z_T^{(i)})
```

### Example list of already used pairs of $\{i,j\}$

```math
U=\{\{i_1,j_1\},\{i_2,j_2\},...\}
```

## Constraints

```math
w \le k < T-w
```

```math
w \le r \le k+1
```

```math
w<0.5T
```

```math
\{i,j\} = \{j,i\}
```

```math
\{i,j\} \notin U
```

# How Mosaic Works

### Random Sampling

```math
i \sim \{1,2,...,N\}

```

```math
j \sim \{1,2,...,N\} \setminus \{i\}

```

# The actual function

```math
D' = \text{Mosaic}(D,L)
```

