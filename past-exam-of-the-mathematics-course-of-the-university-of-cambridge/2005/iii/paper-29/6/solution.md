<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The [abc conjecture](../../../../../abc-conjecture.md) asserts that for every $\epsilon>0$ there is $K_\epsilon\geq1$ such that coprime positive [integers](../../../../../integer.md) $A+B=C$ satisfy

$$
\boxed{C\leq K_\epsilon\operatorname{rad}(ABC)^{1+\epsilon},}
$$

where the radical is the product of the distinct [prime](../../../../../prime-number.md) divisors.

For a primitive positive Fermat triple, the three [integers](../../../../../integer.md) are pairwise coprime. Apply the conjecture to $A=x^n,B=y^n,C=z^n$. Since $x,y<z$, $\operatorname{rad}(ABC)=\operatorname{rad}(xyz)\leq xyz<z^3$. Taking $\epsilon=1/6$ yields $z^{n-7/2}\leq K_{1/6}$. For $n\geq4$ and $z\geq2$ this simultaneously gives

$$
\boxed{z\leq K_{1/6}^2,\qquad n\leq\tfrac72+\log_2K_{1/6}.}
$$

Thus there are finitely many primitive triples and exponents. The primitivity restriction is essential to this abc argument: a nonprimitive triple is a common multiple of a primitive one, and the conjecture normalizes that factor away rather than bounding it. Consequently the intended finiteness conclusion counts primitive triples, or scaling classes. The literal unrestricted Fermat assertion is true for the independent reason that [Fermat's last theorem](../../../../../fermat-last-theorem.md) gives no positive solutions for $n>2$; it does not follow from the displayed primitive height bound alone.

There is a genuine exception to the second printed assertion. **If $a-b=c$, then $x=y=1$ solves the equation for every $n>2$**; for example $(a,b,c)=(2,1,1)$ gives an infinite family. The correct uniform finiteness statement excludes $\max(x,y)=1$.

For that corrected statement put $H=\max(x,y)\geq2$ and $d=\gcd(ax^n,by^n)$. Since their difference is $c$, $d\mid c$. Apply abc to $by^n/d+c/d=ax^n/d$. Its radical is at most $\operatorname{rad}(abc)xy$, and its largest term is at least $\min(a,b)H^n/c$. Therefore

$$
H^{n-2(1+\epsilon)}\leq\frac{cK_\epsilon\operatorname{rad}(abc)^{1+\epsilon}}{\min(a,b)}.
$$

With $\epsilon=1/4$, enlarge the fixed right side to $D\geq1$. For $n\geq3$ the exponent is at least $1/2$, so

$$
\boxed{H\leq D^2,\qquad n\leq\tfrac52+\log_2D.}
$$

This proves finiteness of all nonconstant-power solutions, without requiring $x,y$ coprime.

For an unconditional proof, the diagonal case $x=y=H\geq2$ satisfies $(a-b)H^n=c$ and is elementary. If $a=b$, the unequal-variable gap is at least $2^n-1$, also bounding $n$. In the remaining case interchange variables and coefficients, changing the sign of $c$ if necessary, to have $1\leq X<Y$ and

$$
AX^n-BY^n=\delta,\qquad |\delta|=c.
$$

The nonzero real logarithmic form $\Lambda=\log(A/B)+n\log(X/Y)$ satisfies $e^\Lambda-1=\delta/(BY^n)$. Once $BY^n>2c$, $|\Lambda|\leq2c/(BY^n)$, so $\log|\Lambda|\leq-n\log Y+O_{a,b,c}(1)$. The two-[logarithm](../../../../../logarithm.md) [Baker lower bound for a homogeneous linear form in logarithms](../../../../../baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms.md), with the fixed height of $A/B$ and height of $X/Y$ at most $\log Y$, gives

$$
\log|\Lambda|\geq-C(a,b)\log Y\log(2n).
$$

Hence $n\leq C(a,b)\log(2n)+O_{a,b,c}(1)$ because $Y\geq2$, and $n$ is bounded. The omitted case $BY^n\leq2c$ has bounded exponent and variables directly. For each of the finitely many exponents, $aX^n-bY^n$ has at least three distinct projective roots. The stronger nonzero-value [Thue theorem](../../../../../thue-theorem.md) argument from question 5 therefore gives finitely many pairs, whether or not that binomial form is irreducible. This establishes the [exponent bound for a binomial power equation](../../../../../exponent-bound-for-a-binomial-power-equation.md) and the corrected finiteness statement with no unproved hypothesis. The constant-power family remains the unavoidable exception.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 29](../../paper-29-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
