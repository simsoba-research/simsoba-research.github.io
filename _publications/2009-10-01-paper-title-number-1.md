---

## Hessian (Curvature) Analysis

The second derivative (curvature) of the loss with respect to $\hat{y}_i$ is given by

\[
\frac{\partial^2 \mathcal{L}_{\mathrm{MLC}}}{\partial \hat{y}_i^2}
=
p(p-1)\big[\log(\cosh(\varepsilon_i))\big]^{p-2}\tanh^2(\varepsilon_i)
+
p\big[\log(\cosh(\varepsilon_i))\big]^{p-1}\operatorname{sech}^2(\varepsilon_i).
\]

For $p<2$, the curvature remains bounded for large residuals, which explains the
robust behavior of the loss under outlier contamination, while $p>1$ guarantees
strict convexity and stable optimization.
