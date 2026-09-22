<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the odd congruence class $p\equiv3\pmod8$. The [congruent number elliptic curve](../../../../../../congruent-number-elliptic-curve.md) in the standard scaled coordinates is

$$
E_p:y^2=x(x^2-p^2),\qquad E'_p:y^2=x(x^2+4p^2).
$$

These are the two curves in [two-isogeny descent](../../../../../../two-isogeny-descent.md). On $E_p$, the [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md) restricts the first image to $\{1,-1,p,-p\}$. All four classes occur: the [2-torsion](../../../../../../2-torsion.md) points give $\alpha((0,0))=[-p^2]=[-1]$, $\alpha((p,0))=[p]$, and $\alpha((-p,0))=[-p]$. Thus $\#\alpha(E_p)=4$.

On $E'_p$, the equation forces $x>0$ whenever $x\ne0$. Its exceptional value is $[4p^2]=1$. The second image is therefore contained in $\{1,2,p,2p\}$. Use the [quartic covering in a two-isogeny descent](../../../../../../quartic-covering-in-a-two-isogeny-descent.md) to exclude its three nontrivial candidates.

For $d=p$, a rational solution can be written with [coprime](../../../../../../coprime-integers.md) integral $U,V$, and must satisfy

$$
W^2=p(U^4+4V^4).
$$

Then $p\mid W$, so $U^4+(2V^2)^2\equiv0\pmod p$. Since $p\equiv3\pmod4$, $-1$ is not a [quadratic residue](../../../../../../quadratic-residue.md); a sum of two squares is zero only if both are zero. This forces $p\mid U,V$, contradicting coprimality. For $d=2p$, the same reasoning applies to $W^2=2p(U^4+V^4)$ and again forces $p\mid U,V$.

For $d=2$, the equation is

$$
W^2=2U^4+2p^2V^4.
$$

It implies $W=2Z$, whence $2Z^2=U^4+p^2V^4$. Exactly one of $U,V$ odd is impossible by parity, while both even contradict coprimality. Thus both are odd. Since $p\equiv3\pmod8$ implies $p^2\equiv9\pmod{16}$, reduction modulo sixteen gives $2Z^2\equiv1+9=10$. But the possible residues of $2Z^2$ modulo sixteen are $0,2,8$. This contradiction eliminates $d=2$. Consequently $\alpha'(E'_p)=\{1\}$ and the [square-class index formula for two-isogeny descent](../../../../../../square-class-index-formula-for-two-isogeny-descent.md) gives

$$
2^r=\frac{4\cdot1}{4}=1,\qquad r=0.
$$

The reduction argument for $y^2=x^3+kx$ used earlier bounds rational torsion by four for every nonzero integer $k$: its point-count cancellation at $q\equiv3\pmod4$ does not depend on the sign of $k$, and the same prime choices apply. Here $k=-p^2$ and all four [2-torsion](../../../../../../2-torsion.md) points are rational. Hence $E_p(\mathbb Q)$ consists exactly of $O,(0,0),(p,0),(-p,0)$.

To relate this calculation to [congruent numbers](../../../../../../congruent-number.md), a [rational point](../../../../../../rational-point.md) $(x,y)$ with $y\ne0$ produces the [right triangle](../../../../../../right-triangle.md) with side lengths

$$
A=\left|\frac{x^2-p^2}{y}\right|,\quad
B=\left|\frac{2px}{y}\right|,\quad
C=\left|\frac{x^2+p^2}{y}\right|.
$$

The identities $A^2+B^2=C^2$ and $AB/2=p$ follow from $y^2=x(x^2-p^2)$. Conversely, a positive rational [right triangle](../../../../../../right-triangle.md) of area $p$ with legs $A,B$ and hypotenuse $C$ gives

$$
x=\frac{p(A+C)}B,\qquad y=\frac{2p^2(A+C)}{B^2}\ne0.
$$

Direct substitution uses $AB=2p$ and $C^2=A^2+B^2$. No such point exists here. This proves the [noncongruent primes congruent to three modulo eight](../../../../../../noncongruent-primes-congruent-to-three-modulo-eight.md):

$$
\boxed{p\equiv3\pmod8\text{ prime}\ \Longrightarrow\ p\text{ is not a congruent number}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
