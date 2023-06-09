---
title: Virtual Substitution
emoji: 😸
type: tech
topics: [math, qe]
published: false
---

- virtual (term) substitution
- 仮想置換法 [QE本]


$\alpha \in \R$, $0 \neq f(x) = \sum_{i=0}^n a_i x^i \in \R[x]$, $\varphi_\rho \equiv f(x) \rho 0$ ($\rho \in \{=, \neq, <, \leq \}$) とする.

$f(x // t)$ を $x$ に $t$ を仮想置換したものとする.

### $\epsilon$

$\epsilon$ を正の無限小数 (infinitesimal number) とする.
$\epsilon$ は以下を満たすような数である．

1. $f(\alpha + \epsilon) \neq 0$,
2. $f(\alpha) \neq 0 \rightarrow f(\alpha)f(\alpha + \epsilon) > 0$,
3. $0 = f(\alpha) = f'(\alpha) = \cdots = f^{(k-1)}(\alpha) \neq f^{(k)}(\alpha) \rightarrow f^{(k)}(\alpha) f^{(k)}(\alpha+\epsilon) > 0$.

### $\nu(f)$

$$
\nu(f) = \left\{ \begin{array}{lcl}
f < 0 && (\deg(f) = 0 \ のとき) \\
f < 0 \lor (f = 0 \land \mu(f')) && (\deg(f) > 0 \ のとき)
\end{array} \right.
$$

と定義する.

$$
\begin{align*}
\varphi_{=}(x // x+\epsilon) &\equiv  \land_i a_i = 0, \\
\varphi_{\neq}(x // x+\epsilon) &\equiv \lor_{i} a_i \neq 0, \\
\varphi_{<}(x // x+\epsilon) &\equiv \nu(f), \\
\varphi_{\leq}(x // x+\epsilon) &\equiv \varphi_{<} \lor \varphi_{=}. \\
\end{align*}
$$

例：線形の場合、

$$
\begin{align*}
a (x // x + \epsilon) + b = 0 &\equiv a = 0 \land b = 0, \\
a (x // x + \epsilon) + b < 0 &\equiv ax+b < 0 \lor ax+b=0 \land a < 0 \\
&\equiv a < 0 \land a x+b \leq 0 \lor a \geq 0 \land ax+b < 0 \\
\end{align*}
$$

### $\mu(f)$

無限大の取り扱い. ここで，$n := \deg(f)$ とする.

$$
\mu(f) = \left\{ \begin{array}{lcl}
a_0 < 0 && (n = 0 \ のとき) \\
(-1)^n a_n < 0 \lor a_n = 0 \land \mu(\sum_{i=0}^{n-1} a_i x^i) && (n > 0 \ のとき)
\end{array} \right.
$$

例：線形の場合

$$
\begin{align*}
a (x // -\infty) + b = 0 &\equiv a = 0 \land b = 0, \\
a (x // -\infty) + b < 0 &\equiv a > 0 \lor a = 0 \land b < 0. \\
\end{align*}
$$

