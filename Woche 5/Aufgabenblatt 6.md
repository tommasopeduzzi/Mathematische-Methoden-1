# Aufgabenblatt 6
**Aufgabe 1**
a) 
1) $(\sqrt 3 + i)^3 = (\sqrt 3 + i)^2*(\sqrt 3 + i) = (2 + 6i)*(\sqrt 3 + i)$
$= (2\sqrt3 - 6) + i(2 + 6\sqrt 3)$
2) $(2+3i)* \frac{1+2i}{(1-2i)(1+2i)} =\frac{1+2i}{3} (2+3i) = \frac 1 3 (1+2i)(2+3i)$$= \frac 1 3 ((2 - 6) + i(4 + 3)) = \frac 1 3 (-4 + 7i)$
 3) $\frac 1 {-5+2i\sqrt6} = \frac{-5-2i\sqrt6}{25+24}$
 4) $\frac{1}{(1+i)^2} =\frac{1}{2i} =\frac{-2i}{4} = -0.5i$

b)
1) $i^3 = -i = 0-1i$ Daraus folgt $|z| = 1$ & $arg(z)=-\frac \pi 2$
2) $|z| = \sqrt{6^2} = 6$
$arg(z) = arctan(\frac 0 6) = 0$
3) $|z| = \sqrt{(2\sqrt 3)^2 + 2^2} = \sqrt {14}$
$arg(z) = arctan(\frac{2}{2\sqrt 3}) =\frac \pi 6$ 
4) $|z| = \sqrt{(-\frac35)^2 +\frac45^2} = \sqrt\frac{25}{25} = 1$
$arg(z) = arctan(\frac{\frac45}{\frac35})+\pi = arctan(\frac43)+\pi$

c) $|z| = \sqrt{1^2+\sqrt{3}^2}$
 $\arg(z) = \arctan(\sqrt3) = \frac{\pi}{3}$
 $z^{50} = |z|^{50}(arg(z))^{50} = 2^{50}*e^{i\frac{\pi}{3}50}$
 **sieht nicht besonders einfacher aus**

---
**Aufgabe 2**

a) $1 < |x+(y-2)i| < 2$
$1 < \sqrt{x^2+(y-2)^2} < 2$  |$()^2$
$1<x^2+(y-2)^2 < 4$
![[Pasted image 20211027093842.png]]
Fläche zwischen dem roten Kreis und dem schwarzen Kreis.

b)$\sqrt{x^2+(y-1)^2} > \sqrt{x^2+(y+1)^2}$    |$()^2 -x^2$
$y^2-2y+1 > y^2 + 2y + 1$
$-y>y$, dass heisst wenn y < 0 ist
$\mathbb{L} =\{a,b \in \mathbb R \mid b<0 \}$
![[Pasted image 20211027153811.png]]
c) $2z^2-8z +26 = 0$
$2z^2 -8z + 26 = 0$
$z_{1,2} = \frac{8 \pm \sqrt{64 - 4*2*26}}{2*2}$
$z_{1,2} = \frac{8 \pm \sqrt{144}*\sqrt{-1}}{2*2}$
$z_{1,2} = \frac{8 \pm 12i}{2*2} = 2\pm3i$
![[Pasted image 20211027154038.png]]

d) $z_0 = e^{i0*\frac {2\pi}{4}} = 1$
$z_1 = e^{i1*\frac {2\pi}{4}} =\cos(\frac \pi 2) + i\sin(\frac \pi 2) = i$
$z_2 = e^{i2*\frac {2\pi}{4}} = \cos(\pi) + \sin(\pi)i = -1$
$z_3 = e^{32*\frac {2\pi}{4}} = \cos(\frac {3\pi} 2) + \sin(\frac {3\pi} 2)i = -i$
![[Pasted image 20211027154310.png]]
e)
$z^4 = -4$
$r = \frac{a}{e^{i\pi}} = 4$
$z_0 = \sqrt[4]{4} *e^{i\frac{0+0*2\pi}{4}} = \sqrt{2}$
$z_1 = \sqrt[4]{4} *e^{i\frac{0+1*2\pi}{4}} =\sqrt2e^{i\frac{0+2\pi}{4}}=\sqrt2e^{i\frac{\pi}{2}} = \sqrt2i$
$z_2 = \sqrt2 e^{i\pi} = -\sqrt{2}$
$z_3 = \sqrt[4]{4} *e^{i\frac{6\pi}{4}} =-\sqrt2i$
![[Pasted image 20211027161318.png]]

---
**Aufgabe 3**
a) 
Über  $\mathbb R$:  $p(x) = x^4-2x^2-15 = (x^2-5)(x^2-3)$$=(x-\sqrt5)(x+\sqrt5)(x^2+3)$

b)
Über  $\mathbb R$: $p(x) = x^3 -x^2 -8x + 12 =(x-2)(x^2+x-6) = (x-2)^2(x+3)$
Ich bin mir bei a) und b) nicht sicher wie es über $\mathbb C$ auflösbar sein soll, wenn es so bereits in lineare Faktoren, die nicht weiter zerlegbar sind, faktoriert werden kann...
c)
Über $\mathbb C$: $p(x) = x^4 + 4 = (x-\sqrt{2})(x- \sqrt2e^{i\frac{\pi}{2}})(x +\sqrt{2})(x + \sqrt2e^{i\frac{\pi}{2}})$
Über  $\mathbb R$: $(x-\sqrt{2})(x +\sqrt{2})(x- \sqrt2i)(x + \sqrt2i) = (x-\sqrt{2})(x +\sqrt{2})(x^2 +x\sqrt2i -x\sqrt2i -2)$$=(x-\sqrt{2})(x +\sqrt{2})(x^2-2)$