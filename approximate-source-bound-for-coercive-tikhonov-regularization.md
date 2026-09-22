# Approximate source bound for coercive Tikhonov regularization

↑ **Parent:** [Tikhonov regularization with a coercive penalty operator](tikhonov-regularization-with-a-coercive-penalty-operator.md)

Let $K$ be injective, $u^\dagger=K^\dagger f$, $z=\beta^{-2}B^*Bu^\dagger$, and $\eta_r=\inf_{\|w\|\leq r}\|z-K^*w\|$. Since $\overline{\mathcal R(K^*)}=\mathcal N(K)^\perp=U$, $\eta_r\to0$. For $e=R_\alpha f-u^\dagger$ the [normal equation for coercive Tikhonov regularization](normal-equation-for-coercive-tikhonov-regularization.md) gives $\|Ke\|^2+\alpha\|Be\|^2=-\alpha\beta^2\langle z,e\rangle$. Insert an approximate $K^*w$ and complete the square in $\|Ke\|$ to obtain $\|e\|^2\leq\|z-K^*w\|\|e\|+\alpha\beta^2r^2/4$. This implies the displayed bound, even with coefficient $1/2$ on its last term, and proves consistency without a fixed exact [source condition for quadratic regularization](source-condition-for-quadratic-regularization.md).

## ↑ Ancestors (8)

1. [Tikhonov regularization with a coercive penalty operator](tikhonov-regularization-with-a-coercive-penalty-operator.md)
2. [Tikhonov regularization](tikhonov-regularization.md)
3. [Regularization of an inverse problem](regularization-of-an-inverse-problem.md)
4. [Inverse problem](inverse-problem-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/2/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/2/4/b/solution.md)
