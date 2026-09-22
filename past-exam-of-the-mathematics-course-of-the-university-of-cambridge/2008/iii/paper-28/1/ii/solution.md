<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $t=q+1-\#E(\mathbb F_q)$. The stated characteristic equation for the [Frobenius isogeny](../../../../../../frobenius-isogeny-of-an-elliptic-curve.md) is

$$
\pi^2-[t]\pi+[q]=0.
$$

Take $\alpha,\beta$ to be the complex roots of $T^2-tT+q$. They satisfy $\alpha+\beta=t$ and $\alpha\beta=q$. By the [Hasse bound](../../../../../../hasse-s-theorem-on-elliptic-curves.md), $t^2\le4q$. If the inequality is strict, the roots are complex conjugates and have squared modulus $q$. In the equality case both roots are the same real number $\pm\sqrt q$. Thus in every case

$$
|\alpha|=|\beta|=\sqrt q,\qquad \beta=q/\alpha.
$$

To obtain every extension-field count without assuming distinct roots, set $t_n=\operatorname{tr}(\pi^n)$ and $t_0=2$. The [dual isogeny](../../../../../../dual-isogeny.md) satisfies $\widehat\pi\pi=[q]$ and $\pi+\widehat\pi=[t]$. Consequently the sums $\pi^n+\widehat\pi^{\,n}=[t_n]$ satisfy

$$
t_n=t\,t_{n-1}-q\,t_{n-2},\qquad t_0=2,\quad t_1=t.
$$

Alternatively, apply additivity of the [trace of an elliptic-curve endomorphism](../../../../../../trace-of-an-elliptic-curve-endomorphism.md) directly to the characteristic equation multiplied by $\pi^{n-2}$. The sequence $\alpha^n+\beta^n$ has the same recurrence and initial values, so $t_n=\alpha^n+\beta^n$ by induction. This is the [Frobenius trace recurrence](../../../../../../frobenius-trace-recurrence.md), valid also at a repeated root.

The fixed points of $\pi^n$ are $E(\mathbb F_{q^n})$, and $1-\pi^n$ is again separable. Since $\deg\pi^n=q^n$, the trace-degree identity gives

$$
\#E(\mathbb F_{q^n})=\deg(1-\pi^n)=1+q^n-t_n
=1+q^n-\alpha^n-\beta^n.
$$

Factoring and using $\beta=q/\alpha$ yields

$$
\boxed{\#E(\mathbb F_{q^n})=(1-\alpha^n)(1-q^n\alpha^{-n}),
\qquad |\alpha|=\sqrt q\quad(n\ge1).}
$$

This is the [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) formula and the [Riemann hypothesis for an elliptic curve over a finite field](../../../../../../riemann-hypothesis-for-an-elliptic-curve-over-a-finite-field.md). In particular the powers on both factors are necessary; they are damaged in the converted TeX but present in the original PDF.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
