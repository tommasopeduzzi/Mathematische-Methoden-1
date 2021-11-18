# Aufgabenblatt 9
**Aufgabe 1**
a)$f(x) = 1 -|x|+\frac{1}{2}x$
$F(x) = x-\frac{1}{4}x^2$
Nullstellen von $f$:
$1 - |x| + \frac{1}{2}x$ => $|x| = -1 - \frac{1}{2}x$
=> $x =  -1 -\frac{1}{2}x$ => $x_0 = -\frac{2}{3}$
=> $x = 1 + \frac{1}{2}x$ => $x_1 = 2$
Fläche: $A= |\int_{-2}^{-\frac23} f(x)dx| + \int_{-\frac23}^{2} f(x)dx= 2.\overline2 + (3+\frac{7}{9}) = 6$

b) $f(x) = x^3 -x^2 -2x = x(x+1)(x-2)$
$F(x) = \frac{1}{4}x^4 - \frac{1}{3}x^3 -x^2$
Nullstellen: $x_0 = -1$, $x_1 = 0$, $x_2 = 2$
Fläche: $|\int_{-1}^{0}f(x)dx| + \int_0^2f(x)dx =\frac5{12}+\frac{28}{9} = \frac{127}{36}$
![[Skizze Aufgabe 1.png]]
---
**Aufgabe 2**
a) $F(x) = \frac{1}{2}\ln|\frac{1+x}{1-x}|$
$f(x) = \frac{1}{1-x^2}$
$F'(x)\stackrel{?}{=}f(x)$
$F'(x)=\frac{1}{2}\frac{1}{\frac{1+x}{1-x}}$, da $\ln'(|x|) = \frac{1}{x}$ laut Tabelle Stammfunktionen im Skript
$F'(x) = \frac{1-x}{2+2x}$

b) $F(x) \frac{1}{\sqrt c}\arctan(\frac x {\sqrt c})$	
$f(x) = \frac{1}{c+x^2}$
$F' = f$ direkt ablesbar aus Tabelle der Stammfunktionen im Skript. Herleitung:
$(\frac{1}{\sqrt c}\arctan(\frac x {\sqrt c}))' = \frac{\frac{\sqrt c(\frac{\sqrt c-\frac{x}{2\sqrt{c}}}{c})}{1+\frac{x^2}c}*\frac1{x\sqrt c}arctan(\frac{x}{\sqrt c})}{c}$$=\frac{\frac{{c-\frac{x}{2}}}{c+x^2}*\frac1{x\sqrt c}arctan(\frac{x}{\sqrt c})}{c} =\frac{c-\frac{x}{2}*arctan(\frac{x}{\sqrt c})}{c(x\sqrt c(c+x^2))}$, weiter komme ich nicht.

c) $F(x) = \arcsin(x)$
$f(x) = \frac{1}{\sqrt{1-x^2}}$
$F' = f$ direkt ablesbar aus der Tabelle der Stammfunktionen im Skript. Hier hergeleitet:
$(sin^{-1}(x))' = \frac{1}{sin'(arcsin(x))}$ nach Umkehrregel
$(sin^{-1}(x))' = \frac{1}{cos(arcsin(x))} =\frac{1}{\sqrt{1-sin^2(arcsin(x))}}$  Da $cos^2(x) + sin^2(x) = 1$ Daraus folgt:
$arcsin'(x) = \frac{1}{\sqrt{1-x^2}}$

---
**Aufgabe 3**
a) $\int_{0}^\pi sin(x)x^2+sin(x) dx$
$\int_{0}^\pi \cos(x)\frac13x^3 +(sin(x)+\frac13x^3)|_{0}^\pi +(-cos(x))|_{0}^\pi$
b) $\int_1^a x^n\ln(x)dx = -\int_1^a\frac{x^{n}}{n+1}dx + \frac{1}{n+1}x^{n+1}\ln(x)|_1^a$
c) 