<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The nonzero [quadratic residues](../../../../../../quadratic-residue.md) modulo five are $1,4$. The values of $x^3+x+1$ and the numbers of possible $y$ are

$$
\begin{array}{c|ccccc}
x&0&1&2&3&4\\\hline
x^3+x+1\pmod5&1&3&1&1&4\\
\#\{y\}&2&0&2&2&2
\end{array}
$$

There are eight affine points and one point at infinity. Thus $\#E(\mathbb F_5)=9$ and part(ii) gives $\boxed{\operatorname{tr}(\phi)=5+1-9=-3}$. The curve is nonsingular, since its short-Weierstrass discriminant $-16(4+27)$ is nonzero modulo five.

The dual operation reverses products, so $\widehat{\phi^2}=(\widehat\phi)^2$. Also $\phi\widehat\phi=[5]$ and $\phi+\widehat\phi=[-3]$. Squaring the latter identity gives

$$
\phi^2+\widehat\phi^2=[(-3)^2-2\cdot5]=[-1].
$$

Therefore $\boxed{\operatorname{tr}(\phi^2)=-1}$. Over $\mathbb F_{25}$ the Frobenius is $\phi^2$, of degree $25$, so

$$
\boxed{\#E(\mathbb F_{25})=25+1-(-1)=27.}
$$

More generally the [Frobenius trace recurrence](../../../../../../frobenius-trace-recurrence.md) has $t_0=2$, $t_1=t$ and $t_j=t\,t_{j-1}-q\,t_{j-2}$; the square calculation is its first nontrivial case.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 19](../../../paper-19-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
