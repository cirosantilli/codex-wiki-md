<h1 id="3i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Over $\mathbb F_2$, subtraction equals addition. The polynomial $X^7-1$ has the factorization

$$
\boxed{
X^7-1=(X+1)(X^3+X+1)(X^3+X^2+1).}
$$

The two cubic factors have no root in $\mathbb F_2$, so they are irreducible, and they are reciprocal to one another. Put

$$
f=X^3+X+1,
\qquad
f^*=X^3+X^2+1.
$$

Every cyclic code corresponds to one monic divisor of $X^7-1$. The complete list is

$$
\begin{array}{c|c|c}
g(X)&\text{parameters}&\text{code}\\ \hline
1 &[7,7,1]&\text{whole-space linear code}\\
X+1 &[7,6,2]&\text{even-weight binary code}\\
f &[7,4,3]&\text{Hamming code}\\
f^* &[7,4,3]&\text{reversed Hamming code}\\
(X+1)f &[7,3,4]&\text{binary simplex code}\\
(X+1)f^* &[7,3,4]&\text{reversed binary simplex code}\\
ff^*=1+X+\cdots+X^6 &[7,1,7]&\text{binary repetition code}\\
(X+1)ff^*=X^7-1 &[7,0]&\text{zero code}.
\end{array}
$$

Thus the two cubic generators give the two cyclic coordinate orientations of Hamming's $[7,4,3]$ code. Their duals have generators $(X+1)f$ and $(X+1)f^*$ and are the $[7,3,4]$ simplex codes. The remaining four are the familiar whole-space, even-weight, repetition, and zero codes. This is the [complete classification of binary cyclic codes of length seven](../../../../../../binary-cyclic-codes-of-length-seven.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3I](../../3i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
