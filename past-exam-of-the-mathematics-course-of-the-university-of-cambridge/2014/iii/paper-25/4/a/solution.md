<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $Z=\lfloor N^{2/5}\rfloor$ and $S=\sum_{N<n\le N+M}n^{-it}$. For any positive integer shift $h\le Z^2$, translating the interval changes its sum by at most $2h$. Averaging the shifts $h=xy$ gives the [bilinear shift averaging for a logarithmic phase](../../../../../../bilinear-shift-averaging-for-a-logarithmic-phase.md) identity

$$
S=\frac1{Z^2}\sum_{N<n\le N+M}\sum_{x,y\le Z}(n+xy)^{-it}+O(Z^2).
$$

Since $xy/n\le N^{-1/5}$, the alternating [Taylor expansion](../../../../../../taylor-expansion.md) of the logarithm has remainder at most $(xy/n)^{r+1}/(r+1)$. Thus

$$
-t\log(1+xy/n)=\sum_{j=1}^r\frac{(-1)^jt}{jn^j}x^jy^j+O\bigl(tN^{-(r+1)/5}\bigr).
$$

For $r=\lfloor5.01\log t/\log N\rfloor$, we have $r+1>5.01\log t/\log N$, hence the error is at most $t^{-1/500}$. The [exponential function](../../../../../../exponential-function.md) on an imaginary argument changes by at most the change in that argument. Therefore

$$
\sum_{x,y\le Z}(n+xy)^{-it}=n^{-it}U(n)+O(Z^2t^{-1/500}).
$$

Use $Z^2\asymp N^{4/5}$ and $N<n\le N+M\le2N$. Taking absolute values proves

$$
\boxed{|S|\ll M\max_{N\le n\le2N}\frac{|U(n)|}{N^{4/5}}+N^{4/5}+Mt^{-1/500}.}
$$

The boundary error comes from integer shifts, so this argument also covers intervals shorter than a shift. Here $x,y$ range over positive integers; no zero term is needed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
