<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

A general [feedback shift register](../../../../../feedback-shift-register.md) of length $d$ over an alphabet $A$ stores $(s_n,\ldots,s_{n+d-1})$, outputs $s_n$, and shifts to $(s_{n+1},\ldots,s_{n+d-1},F(s_n,\ldots,s_{n+d-1}))$ for a fixed function $F:A^d\to A$. When the alphabet is a field $K$, it is a [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) if $F$ is linear over $K$, equivalently $s_{n+d}=\sum_{j=0}^{d-1}a_js_{n+j}$ for fixed coefficients in $K$. The binary case uses the [finite field](../../../../../finite-field.md) $K=\mathbb F_2$; the examples and counterexamples below are binary.

For a genuinely nonlinear example take length three and $F(a,b,c)=a+bc$. Its values at $(0,1,0)$ and $(0,0,1)$ are both zero, but its value at their sum $(0,1,1)$ is one, violating additivity. Thus **this general register is not linear**. It even has an invertible state update: from $(b,c,d)$ the old leading bit is $a=d+bc$, so the counterexample does not rely on allowing singular registers.

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
