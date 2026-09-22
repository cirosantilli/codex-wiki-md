# Deterministic calibration of an autoregressive short rate

↑ **Parent:** [Exponential-affine bond pricing](exponential-affine-bond-pricing.md)

For an [affine autoregressive process](affine-autoregressive-process.md) $r_T=\beta r_{T-1}+\xi_T$, suppose its initial [zero-coupon bond](zero-coupon-bond.md) prices $q(T)$ are positive and finite. A deterministic shift $h_T$ of the rate changes the bond price to $q(T)\exp(-\sum_{s=1}^Th_s)$. To fit any positive curve $p(T)$ with $p(0)=1$, put $d_T=\log q(T)-\log p(T)$, $d_0=0$, $h_T=d_T-d_{T-1}$ and $h_0=0$. Adding the deterministic drift $\alpha_T=h_T-\beta h_{T-1}$ to the rate recursion realizes precisely this shift, and telescoping gives the desired curve. No stationary autoregression assumption is needed.

## ↑ Ancestors (8)

1. [Exponential-affine bond pricing](exponential-affine-bond-pricing.md)
2. [Zero-coupon bond](zero-coupon-bond.md)
3. [Fixed-income security](fixed-income-security.md)
4. [Mathematical finance](mathematical-finance-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39/1/c/solution.md)
