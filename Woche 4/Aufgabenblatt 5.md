# Aufgabenblatt 5
[[blattMMI5.pdf]]
### Aufgabe 1

a) $\mathbb{W} = \{y | \lim_{x\searrow-\frac \pi 2} \frac{sin(x)}{cos(x)} \leq y\leq \lim_{x\nearrow\frac \pi 2} \frac{sin(x)}{cos(x)} \} = \{y | -\infty \leq y\leq\infty \}$
$y = tan(\frac{x-\pi}{2})$
$2arctan(y) +\pi = x$
$g(x) = 2arctan(x) + \pi$
![[1a.jpg]]

b)$\mathbb W = \{y| (5-2^0)\leq y<\lim_{x\to\infty}5-2^x\} = \{y| 4\leq y< 5 \}$
$y = 5-2^{-x}$
$y + 5 = 2^{-x}$
$-log_2(y+5) = x$
$g(x) = -log_2(x+5)$
![[1b.jpg]]


---
### Aufgabe 2
1)  $lim_{x\to\infty} \frac{x-\sqrt{5}x^2-3}{4+x^2} =_{/x^2} lim_{x\to\infty} \frac{\frac{1}{x} - \sqrt{5} - \frac{3}{x^2}}{\frac{4}{x^2}+1} =\frac{0-\sqrt{5} - 0}{0+1} = -\sqrt{5}$
2) $lim_{x\to\infty \frac{3-2^x-10^x}{1+10^x}} =_{/10^x} \frac {\frac 3 {10^x} - \frac {2^x}{10^x} -1}{\frac 1 {10^x} + 1} = \frac{0-0-1}{0+1} = -1$ 
3) $lim_{x\to0}\frac{tan(x)} x =\frac{lim_{x\to0} tan(x)}{lim_{x\to0} x} = \frac 0 0 = 1$ 
5) $lim_{x\to\infty} arctan(\frac{x^2-x^3+1}{x^2+x}) =lim_{x\to\infty} arctan(\frac{\frac 1 x-1+\frac 1 {x^3}}{\frac 1 x+ \frac 1 {x^2}})$
$lim_{x\to\infty} \frac{\frac 1 x -1 +\frac 1 {x^3}}{\frac 1 x+ \frac 1 {x^2}} = -1$
$arctan(-1) = -\frac{\pi}{4}$ 



---
### Aufgabe 3
a) $f(x) = -(x-3)(\frac{1}{-x^2*x-1}+\frac{1}{(x-1)^2}+\frac{1}{x+1})$
b) $\left(1+\left(\sum_{n=1}^{100}\frac{9}{10^{n}}\right)\ \right)\cdot e^{-\left(x-1\right)^{2}}$ **Bin mir nicht sicher ob das korrekt ist, da $1.\overline9 = 2$ ist... 
c)$f(x) = 3sin(13x)$  
d)  $f(x) = 4e^{-x^{0.5}}+1$