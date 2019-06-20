---
layout: page
title: "Complex Analysis"
permalink: /complex/
mathjax: true
---

> Up to date as of Summer 2019.

**Inspired by [Bahran](http://www-users.math.umn.edu/~bahra004/complex_prelim.pdf).**

Complex Analysis problems that were asked in the past at IIT Kanpur. <red>It would be awesome if someone can contribute the solutions.</red>

**Contributed by:** Debashish Reang. [:pencil2: Improve this page](https://github.com/reangdeba/reangdeba.github.io/edit/master/misc/complex-analysis.markdown)

<center>De-Moivre's formula</center>

**Fall 2018, 1b.** Use De Moivre’s formula to obtain all the distinct roots of the polynomial $$z^3 - \lambda$$, for a fixed $$\lambda \in R^{>0}$$.

<center>Linear Fractional Transformation</center>

**Fall 2018, 2.** Let $$ \mathbb{H} = {z:Im(z) \geq 0}$$ denote the upper half plane. Let $$\mathbb{D} = \{z: \mid z \mid \leq 1\}$$ be the closed unit disk in $$\mathbb{C}$$.

* **(a)** Obtain a Mobius transformation $$ \phi : \mathbb{H} \to \mathbb{D}$$ such that $$0 \mapsto i, 1 \mapsto -1,i \mapsto 0$$ and such that $$\phi^{-1}$$ has a pole at $$-i$$. Also, obtain a formula for $$\phi^{-1}(z)$$.
* **(b)** Let $$f : \mathbb{H} \to \mathbb{D}$$ be an analytic function such that $$f(i) = 0$$. Let $$ \mid f(2i) \mid = \frac{1}{3}$$. Then compute $$\mid f(3i) \mid$$.

**Summer 2019, 6.** Let $$\mathbb{D}$$ be the unit disc $${z \in C: \mid z \mid \leq 1}$$ and $$\mathbb{H}$$ denote the upper half plane $${z \mid Im(z) \geq 0}$$. Find a mobius transformation $$\phi : \mathbb{H} \to \mathbb{D}$$ such that $$\phi (0) = −1; \phi (i) = 0; \phi (\infty) = 1$$.

<center>functions and polynomials</center>

**Fall 2018, 1a.** State Liouville’s theorem. Using Liouville’s theorem deduce that the image of a non- constant entire function $$h: \mathbb{C} \to \mathbb{C}$$ cannot be a finite set.<br>
<!-- **Liouville's theorem.** If a function is entire and bounded in $$\mathbb{C}$$, then the function is constant. -->

**Fall 2018, 1c.** Let $$ h:\mathbb{C} \to \mathbb{C}$$ be an analytic function such that $${h(z)}^2 = \overline{h(z)}$$ for all $$z \in \mathbb{C}$$. List all the distinct functions $$h$$ satisfying the above condition. Give sufficient justification for your answer.

**Fall 2018, 3a.** Let f be an entire function. Let $$ \mid f(z) \mid \leq a \mid z \mid ^m$$, where $$a \in \mathbb{R}^{>0}$$ and $$m \in \mathbb{N}$$. Show that $$f$$ is a polynomial of degree at most m.

**Fall 2018, 3b.** Let $$B_1(0)$$ denote the unit disc $$\{z \in \mathbb{C} : \mid z \mid < 1\}$$. Determine all the distinct analytic functions $$f : B_1(0) \to \mathbb{C}$$ satisfying the condition $$f(1/n) = n^2 \left[f(1/n) \right]^3$$ for all $$n \in \mathbb{N}$$. Give proper justification.

**Summer 2019, 1.** If $$f$$ is an entire function and $$f(x + 2\pi) = f(x)$$ for all real number $$x$$ then does $$f(z + 2\pi) =
f(z)$$, for all complex numbers $$z$$ ? Prove it or give a counterexample.

**Summer 2019, 2.** Let $$Log(z)$$ be the principal branch of complex logarithm. State whether it is true or false **with justification** that $$Log(z^n) = nLog(z)$$ for every positive integer $$n$$.

<center>taylor and laurent series</center>

**Fall 2018, 4a.** Find the Laurent series of $$\frac{1}{2-3z+z^2}$$ in the annulus $$\sqrt{2} < \mid z + i \mid < \sqrt{5}$$.

**Fall 2018, 4c.** Let **R** be **1**. Let $$f(z)=\sum_{n=0}^{\infty}2^n z^{n^2}$$ for all $$z \in B_R(0)={z \in \mathbb{C}:\mid z \mid < R}$$. Obtain the Taylor series around $$0$$ of an antiderivative of $$f(z)$$.

**Summer 2019, 4.** Give a power series expansion of the principal branch of $$\sqrt{z}$$ about 1 and find its radius of convergence with complete justification. Also, obtain explicitly the coefficient of $$(z-1)^
{10}$$ in this series.

<center>Radius of convergence</center>

**Fall 2018, 4b.** Determine the radius of convergence **R** of $$\sum_{n=0}^{\infty}2^n z^{n^2}$$.

<center>contour integration</center>

**Fall 2018, 5.** Using a contour containing the arc $$S_R : Re^{i \theta}, \space 0 \leq \theta \leq \pi (R>0),$$ evaluate $$\int_{0}^{\infty} \frac{\cos ax - \cos bx}{x^2} dx$$ where $$0 < a < b$$ are fixed real numbers.

**Summer 2019, 5.** Using indentation lemma evaluate the integral $$\int_{0}^{\infty} \frac{x-\sin x}{x^3} dx$$.

**Summer 2019, 3.** Evaluate $$\int_{\gamma} \overline{z} dz$$, where $$\gamma (t) = e^{n\pi i t}$$ where $$n = 4$$ and $$n = 5$$ and $$ 0 \leq t \leq 1$$.