# Linear Boolean function

↑ **Parent:** [Boolean function](boolean-function.md)

A [linear Boolean function](linear-boolean-function.md) is a [linear map](linear-map.md) from $\mathbb F_2^n$ to $\mathbb F_2$. Here $\mathbb F_2$ is the two-element [finite field](finite-field.md), whose [addition](addition.md) is [exclusive or](exclusive-or.md). Every such function has a unique coefficient [binary string](binary-string.md) $a$ and takes the form

$$
f_a(x)=a\cdot x=\bigoplus_{j=1}^{n}a_jx_j.
$$

The dot is the [binary inner product](binary-inner-product.md). To prove the representation, expand $x=\sum_jx_je_j$ in the [standard basis](standard-basis.md) and use [linearity](linearity.md), obtaining $f_a(x)=\sum_jx_jf_a(e_j)$; thus $a_j=f_a(e_j)$. For example, $a=101$ gives $f_a(x)=x_1\oplus x_3$. Adding a nonzero constant produces an [affine map](affine-map.md), not a [linear map](linear-map.md).

## ↑ Ancestors (7)

1. [Boolean function](boolean-function.md)
2. [Boolean hypercube](boolean-hypercube.md)
3. [Analysis of Boolean functions](analysis-of-boolean-functions-split.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Bernstein-Vazirani algorithm](bernstein-vazirani-algorithm.md)
- [Classical query complexity of linear Boolean function identification](classical-query-complexity-of-linear-boolean-function-identification.md)
- [Hadamard-conjugated linear oracle](hadamard-conjugated-linear-oracle.md)
- [Linear Boolean function](linear-boolean-function.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/1/solution.md)
- [Solution](past-exam-of-the-laser-science-and-quantum-information-processing-course-of-the-university-of-oxford/2010/6/3/solution.md)
