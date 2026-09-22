# Exact late slope of an exponentially damped oscillator

↑ **Parent:** [Bessel transition for an exponentially decaying oscillator](bessel-transition-for-an-exponentially-decaying-oscillator.md)

For $y_{tt}+e^{-2\varepsilon t}(\varepsilon y_t+y)=0$, $y(0)=0$, $y_t(0)=1$, set $r=e^{-2\varepsilon t}/2$. The exact equation becomes $ry_{rr}+(1-r)y_r+y/(2\varepsilon^2)=0$. Let $m(t)=M(-1/(2\varepsilon^2),1,r)$, using the [Kummer function](confluent-hypergeometric-function-of-the-first-kind.md). It is regular at $r=0$ and tends to one. The [Wronskian](wronskian.md) $W=my_t-m_ty$ obeys $W_t=-\varepsilon e^{-2\varepsilon t}W$, with $W(0)=M(-1/(2\varepsilon^2),1,1/2)$. Integration gives the displayed exact late slope. The other local solution grows at most logarithmically in $r$, so $m_ty\to0$ and $W\to y_t$. This provides a check on a [WKB approximation](wkb-approximation.md) even near phases where its leading predicted slope vanishes.

## ↑ Ancestors (7)

1. [Bessel transition for an exponentially decaying oscillator](bessel-transition-for-an-exponentially-decaying-oscillator.md)
2. [WKB approximation for a slowly varying oscillator](wkb-approximation-for-a-slowly-varying-oscillator.md)
3. [WKB approximation](wkb-approximation.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-336/3/i/solution.md)
