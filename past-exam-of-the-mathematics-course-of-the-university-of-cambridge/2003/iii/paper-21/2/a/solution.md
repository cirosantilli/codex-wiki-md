<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For each $x\in\mathbb F_p$, count the roots of $y^2=x^3+x^2+x+1$, and add the identity at infinity. A nonzero [quadratic residue](../../../../../../quadratic-residue.md) gives two roots, zero gives one, and a nonsquare gives none. Equivalently, with the [Legendre symbol](../../../../../../legendre-symbol.md) extended by $\chi_p(0)=0$,

$$
\#\widetilde E_p(\mathbb F_p)=p+1+\sum_{x\in\mathbb F_p}\chi_p(x^3+x^2+x+1).
$$

The numbers of affine $y$ values, in increasing $x$ order starting at zero, are

$$
\begin{array}{c|l|c}
p&\text{root counts for }x=0,\ldots,p-1&\#\widetilde E_p(\mathbb F_p)\\\hline
3&(2,2,1)&6\\
5&(2,2,1,1,1)&8\\
7&(2,2,2,0,2,2,1)&12\\
11&(2,2,2,0,0,0,0,2,0,0,1)&10
\end{array}
$$

so the answer is

$$
\boxed{(\#\widetilde E_3,\#\widetilde E_5,\#\widetilde E_7,\#\widetilde E_{11})=(6,8,12,10).}
$$

All four reductions are [smooth algebraic curves](../../../../../../smooth-algebraic-curve.md): the original PDF gives the [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) $-2^8$, so these odd primes are primes of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../b/solution.md)
