---
title: content1
nav_order: 2
---
<script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script> <script> MathJax = { tex: { inlineMath: [['$', '$'], ['\\(', '\\)']], displayMath: [['$$', '$$'], ['\\[', '\\]']] } }; </script>
# How to build Automatic Differentiation script with just python
let's say we have 

$$
f(x,y) = x^2 + xy + 1
$$

and we can rewrite it as 

$$
f(x,y) = (x \cdot x) + (x \cdot y + 1)
$$

$$
f(x,y) = Sum[(x \cdot x), (x \cdot y + 1)]
$$

$$
f(x,y) = Sum[(x \cdot x), Sum[x \cdot y, 1]]
$$

$$
f(x,y) = Sum[Mul[x, x], Sum[Mul[x, y], 1]]
$$

$$
\frac{d}{d\psi} Sum[a, b] = \frac{da}{d\psi} + \frac{db}{d\psi}
$$

$$
\frac{d}{d\psi} Mul[a, b] = a\frac{db}{d\psi} + b\frac{da}{d\psi}
$$

$$
\frac{da}{d\psi}=
    \begin{cases}
        1 & \text{if } \psi = a\\
        0 & \text{if } \psi \neq a
    \end{cases}
$$

$$
\frac{d (constant)}{d\psi} = 0
$$
