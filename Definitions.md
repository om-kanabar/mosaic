# Definitions

### Symbol : Meaning

$D$ : TokaMark Dataset

$D'$ : Dataset of synthesized data

$N$ : Number of samples in $D$

$x^{(i)}$ : Sample $i$ in $D$

$x^{(j)}$ : Sample $j$ in $D$

$U$ : List of already used pairs of $\{i,j\}$.

$s^{(i)}$ : The starting state of sample $x^{(i)}$

$x_m^{(i)}$ :  the $m$ᵗʰ observation in $x^{(i)}$

$T$ : The fixed sample length in terms of amount of observations .

$k$ : Split index in the first sample

$r$ : Split index in the second sample

$w$ : Comparison window length used by Mosaic to determine $r$

$z^{(i)}$ : the $i$ᵗʰ synthetic sample made by Mosaic

$z_m^{(i)}$ : The $m$ᵗʰ observation in synthetic sample $z^{(i)}$

$L$ : Number of generated samples the user wants

# Example Data

### Example Dataset

$$
D = \{x^{(1)},x^{(2)},...,x^{(N)}\}
$$

### Example Sample

$$
x^{(i)} = (x_1^{(i)},x_2^{(i)},...,x_T^{(i)})
$$

### Example Synthetic Dataset

$$
D'= \{z^{(1)},z^{(2)},...,z^{(L)}\}
$$

### Example Synthetic Sample

$$
z^{(i)} = (z_1^{(i)},z_2^{(i)},...,z_T^{(i)})
$$

### Example list of already used pairs of $\{i,j\}$

$$
U=\{\{i_1,j_1\},\{i_2,j_2\},...\}
$$

## Constraints

$$
w \le k < T-w
$$

$$
w \le r \le k+1
$$

$$
w<0.5T
$$

$$
\{i,j\} = \{j,i\}
$$

$$
\{i,j\} \notin U
$$

# How Mosaic Works

### Random Sampling

$$
i \sim \{1,2,...,N\}

$$

$$
j \sim \{1,2,...,N\} \setminus \{i\}

$$

# The actual function

$$
D' = \text{Mosaic}(D,L)
$$