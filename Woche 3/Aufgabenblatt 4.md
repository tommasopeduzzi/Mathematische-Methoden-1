# Aufgabenblatt 4
![[blattMMI4.pdf]]

### Aufgabe 1
a) $a_n = \frac{1}{\sqrt{n^3+1}}$ 
$\frac{1}{\sqrt{n_0^3+1}} <\epsilon$
$\frac{1}{\epsilon^2} < n_0^3+1$
$\sqrt[3]{\frac{1}{\epsilon^2}-1} < n_0$
Epsilon  $\epsilon = 10^{-3}$ einsetzen:
$\sqrt[3]{\frac{1}{{10^{-3}}^2}-1} = 100 < n_0$
$n_0 = 101$

Epsilon  $\epsilon = 10^{-6}$ einsetzen:
$\sqrt[3]{\frac{1}{{10^{-6}}^2}-1} = 10000 < n_0$
$n_0 = 10001$
Für jedes $\epsilon$ gibt es ein $n_0$, so dass $\sqrt[3]{\frac{1}{\epsilon^2}-1} < n_0$ und $|a_n| < \epsilon$ $\forall n≥n_0$.

b) 
$1.\overline{359} = 1 + \sum_{k=1}^{\infty} \frac{359}{10^{3k}} = 1 + 359 *\frac{\frac{1}{10^3}}{1-\frac{1}{10^3}} = 1+ \frac{359}{999}$ 
$1.35 + 10^{-2}* \sum_{k=1}^{\infty} \frac{9}{10^{k}} = 1.35 + 10^{-2}*9*\frac{\frac{1}{10^2}}{1-\frac{1}{10^2}} = \frac{34}{25}$ 

---
**Aufgabe 2**
a)
$a_n = \frac{3n * n^2 +3}{4n^2 - 6n + 1}$
$a_n = \frac{2 + n - \frac{3}{n}}{4n -6 + \frac{1}{n}}$ 
$\lim_{n\to\infty} a_n = \lim_{n\to\infty} \frac{\frac{2}{n} + 1 - \frac{3}{n^2}}{4 - \frac{6}{n}+\frac{1}{n^2}} = \frac{0+1+0}{4-0+0} = \frac{1}{4}$
b) $\lim_{n\to\infty}\frac{(n^3+1)^{\frac{1}{2}}-n}{2n(n)^{\frac{1}{2}}} =\lim_{n\to\infty}\frac{(n^3+1)^{\frac{1}{2}}-n}{2n(n)^{\frac{1}{2}}} = \lim_{n\to\infty}\frac{\frac{\sqrt{n^3+1}}{n^{1.5}}-n^{-0.5}}{2} = \frac{\frac{\infty}{\infty}-0}{2} = \frac{1}{2}$
c)
$c_n = \frac{4^{n+1}(1.5+(-1)^n*\frac{1}{2^n-2})}{4^{n+1}(\frac{8*3^n}{4^{n+1}+1})}$
$lim_{n\to\infty} c_n = lim_{n\to\infty} \frac{1.5+(-1)^n*\frac{1}{2^n-2}}{\frac{8*3^n}{4^{n+1}}+1} = \frac{1.5 + 0}{0 + 1} = 1.5$
d)
$s_n =\sum_{k=1}^{n} \frac{2^{k+1}}{(-5)^k} = 2 * \sum_{k=1}^{n} \frac{2^{k}}{(-5)^k}$
$lim_{n\to\infty} s_n = 2 * \lim_{n\to\infty} \sum_{k=1}^{n} \frac{2^{k}}{(-5)^k} = 2* \frac{\frac{2}{-5}}{1-\frac{2}{-5}} =2*\frac{\frac{-2}{5}}{\frac{7}{5}}=-\frac{4}{7}$
---
**Aufgabe 3**
Induktionsverankerung:
 $\frac{2}{1(2)(3)} = \frac{1}{2} - \frac{1}{(2)(3)} = \frac{1}{3}$ ✔️
 
 Induktionsschritt:
 Ang.: $\sum_{k=1}^{n} \frac{2}{k(k+1)(k+2)} = \frac{1}{2} - \frac{1}{(n+1)(n+2)}$
Es gilt zu beweisen $\sum_{k=1}^{n+1} \frac{2}{k(k+1)(k+2)} = \frac{1}{2} - \frac{1}{(n+2)(n+3)} = \frac{1}{2} - \frac{1}{n^2 + 5n + 6}$
$\sum_{k=1}^{n} \frac{2}{k(k+1)(k+2)} = \frac{1}{2} - \frac{1}{(n+1)(n+2)}$      |$+ \frac{2}{(n+1)(n+2)(n+3)} = \frac{2}{(n^3 + 6n^2 + 11n + 6)}$
$\sum_{k=1}^{n+1} \frac{2}{k(k+1)(k+2)} = \frac{1}{2} - \frac{1}{(n+1)(n+2)}*\frac{(n+3)}{(n+3)} + \frac{2}{(n+1)(n+2)(n+3)} = \frac{1}{2} - \frac{(n+1)}{(n+1)(n+2)(n+3)} = \frac{1}{2} -\frac{1}{(n+2)(n+3)}$ qed
Grenzwertsberechnung:
$\frac 1 2\sum_{k=1}^\infty \frac{1}{k(k+1)(k+2)} = \frac 1 2\lim_{n\to\infty} (\frac{1}{2}-\frac{1}{(n+2)(n+3)}) = \frac 1 2(\frac{1}{2} + \lim_{n\to\infty}-2* \lim_{n\to\infty}\frac{1}{(n+2)}\lim_{n\to\infty}\frac{1}{(n+3)})$
$\frac 1 2 \sum_{k=1}^\infty \frac{1}{k(k+1)(k+2)} = \frac 1 2\lim_{n\to\infty} (\frac{1}{2}-\frac{1}{(n+2)(n+3)}) = \frac 1 2 (\frac{1}{2} + -2 *0*0)= \frac{1}{4}$
---
### Kontrollfragen:
**Frage 1:**
a) X
b) X
c) ✔️

**Frage 2:**
a) ✔️, weil $|q|<1$
b) X, weil $\sum_{k=0}^\infty lim_{m\to\infty} (\frac 1 m -1)^k=\sum_{k=0}^\infty 0 -1$, was keinen Grenzwert hat. (siehe unten).
c) X, weil $|-1| < 1$ ist falsch


