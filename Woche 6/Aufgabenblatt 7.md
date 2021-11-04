# Aufgabenblatt 7
**Aufgabe 1**
a) $f(x) = \frac x {1 + x^2}$
$f(x)' = \frac {1 - x^2}{(1 +x^2)^2}$
b)
$f(x) = \frac {sin(x)} x$
$f'(x) = \frac{cos(x)x - sin(x)}{x^2}$
c)
$f(x) = e^{-2x}\cos(3x)$
$f'(x) = -2e^{-2x}cos(3x) + e^{-2x}sin(3x)3$
d)

$f(x) = \ln(x+\sqrt{1 + x^2})$
$u = ln(x)$ 
$u' = \frac 1 x$
$v = x + \sqrt{1+x^2}$
$v' = 1 + \frac 1 {2\sqrt{1+x^2}}+2x$
$f'(x) =\frac {\frac {x}{\sqrt{1+x^2}}} {x + \sqrt{1+x^2}} = \frac {x} {1+x^2 + x*\sqrt{1+x^2}} = \frac{1}{\sqrt{1+x^2}}$

e) $f(x) = \arctan(\frac 1 {x^2})$
$f'(x) = \arctan'(\frac{1}{x^2}) * -\frac{2}{x^3}$$=\frac{1}{1+\frac{1}{x^4}}\times-\frac{2}{x^3} = - \frac{2x}{(1+\frac1{x^4})x^4} =-\frac{2x}{x^4+1}$

---
**Aufgabe 2**
a) $f(x) = \frac{1}{8}x^3 - \frac{3}{2}x + 2$
$f'(x) =\frac{3}{8}x^2-1.5$
Tangente bei $x_0 = 0$:
$y = 2- 1.5x$ 
Tangente bei $x_1 = 2$:
$y = f(2) + f'(2)(x-2) = 0$ 
$\frac{1}{8}x^3 - \frac{3}{2}x + 2 = 0$
$x_1 = -4$

Tangente bei $x_2 = -2$:
$\frac{1}{8}x^3 - \frac{3}{2}x - 2 = 0$ 
$x_1 = 4$ 
![[Skizze 2A.jpg]]
b) $f(x) = cosh(x):= \frac{1}{2}(e^x+e^{-x}) = \frac{1}{2} e^x + \frac{1}{2}e^{-x}$
$f'(x) =\frac{1}{2}e^x - \frac{1}{2}e^{-x}$
Tangente bei $x_0 = 0$:
$y = f(0) + f'(0)x = 1$
Tangente bei $x_1 = ln(2)$:
$y = f(ln(x)) +f'(ln(2))(x-ln(2))$
$= 1.25 + 0.75(x-ln(2))$
---
**Aufgabe 3**
a) Nicht differenzierbar
b) Differenzierbar, da:
$\lim_{x\to0} \frac{\sin(x)}{x} = \lim_{x\to 0} cos(x) = 1$
$f'(x) =         \begin{cases}\frac{cos(x)x + sin(x)}{x^2} \mbox{ für}x \neq0\\ 0 \mbox{ für } x = 0\end{cases}$
$f'(0) = 0$
c) Differenzierbar, da:
$\lim_{x\searrow0}x\ln(x) = \lim_{x\searrow0} \frac{ln(x)}{\frac 1 x} = \lim_{x\searrow0} \frac{x^{-1}}{-{x^{-2}}} = \lim_{x\searrow0} -x = 0$$f'(x) =\begin{cases}\ln(x)+1 \mbox{ für}x \neq0\\ 0 \mbox{ für } x = 0\end{cases}$
$f'(x) = 0$
d)Differenzierbar, da:
$lim_{x\to0} \frac{1}{x^2} =\infty$
$lim_{x\to\infty} exp(-x) = 0$
$f'(0) = 0$