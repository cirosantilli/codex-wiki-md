# Arcsine distribution on a bounded interval

↑ **Parent:** [Arcsine distribution](arcsine-distribution.md)

Specify whether two parameters mean endpoints or location and width. With endpoints $a<b$, define $Y=a+(b-a)X$ for a standard [arcsine distribution](arcsine-distribution.md) variable $X$. Then

$$
f_Y(y)=\frac1{\pi\sqrt{(y-a)(b-y)}},\quad a<y<b,
\qquad F_Y(y)=\frac2\pi\arcsin\sqrt{\frac{y-a}{b-a}}.
$$

This is a [location-scale family](location-scale-family.md) with location $a$ and width $b-a$. Its [mean](expected-value-split.md) is $(a+b)/2$ and its [variance](variance-split.md) is $(b-a)^2/8$. A convention using parameters $a,w$ for location and width instead has right endpoint $a+w$, so it must not be read as having endpoints $a,w$.[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Arcsine Distribution, Definition, Distribution Functions and Moments: location-plus-width convention and alternative endpoint parametrization](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-arcsine-distribution.md)

For example, a chosen interval $[-2,6]$ gives [mean](expected-value-split.md) $2$ and [variance](variance-split.md) $8$, while its density still concentrates toward both endpoints. It is a bounded [probability distribution](probability-distribution-split.md); its endpoint singularities do not make its support infinite.

## ↑ Ancestors (8)

1. [Arcsine distribution](arcsine-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
