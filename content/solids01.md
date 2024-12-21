---
title: Einstein Summation Convention
parent: Solid Mechanics
nav_order: 1
math: true
---

<!-- Load MathJax explicitly with delimiters -->
<script type="text/javascript" id="MathJax-script" async
  src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
</script>
<script>
  MathJax = {
    tex: {
      inlineMath: [['$', '$'], ['\\(', '\\)']],
      displayMath: [['$$', '$$'], ['\\[', '\\]']]
    }
  };
</script>

# **Einstein Summation Convention**

The **_Einstein Summation Convention_** is a powerful notation used to simplify expressions involving **vectors** and **tensors**. It avoids the explicit use of summation symbols and makes tensorial equations more compact and readable.

A vector **a** can be expressed in expanded form as:

$$
\mathbf{a} = \sum_{i=1}^{3} a_i = a_1 + a_2 + a_3
$$

In **Einstein Summation Convention**, the summation symbol $\sum$ is omitted, and repeated indices imply summation over those indices. Therefore, the above equation can be written as:

$$
\mathbf{a} = a_i
$$

Where:

- $a_i$ represents the components of the vector $\mathbf{a}$.  
- The index $i$ runs over the specified dimensions (e.g., \( 1, 2, 3 \) for three-dimensional space).  

This convention is widely used in **_continuum mechanics_**, **_solid mechanics_**, and **_tensor analysis_** to simplify and generalize expressions.
