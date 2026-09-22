<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\delta=1-m\downarrow0$. This is the [complete elliptic integral of the first kind](../../../../../../complete-elliptic-integral-of-the-first-kind.md) in parameter notation; the modulus used in some definitions is $\sqrt m$. Near the endpoint, $s=\pi/2-\vartheta$ gives

$$
1-m\sin^2\vartheta=\delta+s^2+O(\delta s^2+s^4).
$$

Use [matched asymptotic expansion](../../../../../../matched-asymptotic-expansion.md) with an intermediate cutoff $b$ satisfying $\sqrt\delta\ll b\ll1$. Away from the endpoint the leading integral is

$$
\int_0^{\pi/2-b}\frac{d\vartheta}{\cos\vartheta}=\log\frac2b+O(b^2),
$$

while the endpoint integral is

$$
\int_0^b\frac{ds}{\sqrt{\delta+s^2}}
=\operatorname{arsinh}\frac b{\sqrt\delta}
=\log\frac{2b}{\sqrt\delta}+o(1).
$$

Adding them removes the arbitrary cutoff and gives the [logarithmic endpoint asymptotic of the complete elliptic integral](../../../../../../logarithmic-endpoint-asymptotic-of-the-complete-elliptic-integral.md)

$$
\boxed{K(m)=\log\frac4{\sqrt{1-m}}+
O\!\left((1-m)\log\frac1{1-m}\right)}.
$$

The order of the next term is therefore $(1-m)\log(1/(1-m))$, rather than merely $1-m$. More explicitly, if $L=\log(4/\sqrt\delta)$,

$$
K(m)=L+\frac\delta4(L-1)+O(\delta^2L).
$$

The logarithmic correction arises from the next terms integrated through the overlap. Its coefficient can also be found by substituting $L+\delta(aL+b)$ into the [Gauss hypergeometric equation](../../../../../../gauss-hypergeometric-equation.md) satisfied here, $m(1-m)K_{mm}+(1-2m)K_m-K/4=0$, giving $a=1/4$, $b=-1/4$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
