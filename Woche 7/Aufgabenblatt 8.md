# Aufgabenblatt 8¨
**Aufgabe 1**
a) $f(x) = \frac{(x-1)(x+3)}{e^x}$
    $f'(x) = \frac{(2x + 2) e^x - e^x(x^2+2x-3)}{e^{2x}} =\frac{e^x((\sqrt5 + x)(\sqrt5-x))}{e^{2x}}= e^{-x}((\sqrt5 + x)(\sqrt5-x))$	$f''(x))= -e^x((\sqrt5 + x)(\sqrt5-x)) *e^{-x}(2x*2\sqrt5)$
	Kritische Stellen/Nullstellen der Ableitung: $\pm \sqrt5$
	Bei $x =\sqrt5$ $f''(\sqrt5) = 0$ 
	$f'$ wechselt von + auf - =>isoliertes lokales Maximum
	Bei $x =-\sqrt5$ $f''(-\sqrt5) = 0$
	$f'$ wechselt von - auf + =>isoliertes lokales Minimum
	![[1c.png]]
	Nullstellen:
	$1$ und $3$
	Grenzwerte:
	$\lim_{x\to\infty} \frac{(x-1)(x+3)}{e^x} = 0$
	$\lim_{x\to-\infty} \frac{(x-1)(x+3)}{e^x} = \lim_{x\to-\infty} \frac{2x + 2}{e^x} = \infty$
b) $f(x) = \ln(x^3+1)$
	$f'(x) = \frac {3x^2} {x^3+1}$
		$f''(x) = \frac{6x(x^3+1) - (3x^2)^2}{x^6+2x^3+1}$
	Kritische Stellen: 
	Bei $x = 0$: $f''(0) = 0$ Wechselt nicht das Vorzeichen, also Sattelpunkt.
	![[1b.png]]
	Nullstellen: $0$
	Grenzwerte:
	$\lim_{x\to\infty} \ln(x^3 + 1) = \infty$
	$\lim_{x\to-\infty} \ln(x^3 + 1) = \lim_{x\to-\infty}  \ln(x) = undefined$ 
	$\lim_{x\searrow-1} \ln(x^3+1) =\lim_{x\searrow0} \ln(x) = -\infty$
	c) $f(x) = \arctan(x^3-9x^2)$
	$f'(x) = \frac{3x(x-6)}{1+(x^3-9x^2)^2}$
	Kritische Stellen: $0, 6$ 
	Bei $x=0$: $f'$ wechselt von positiv auf negativ, also isoliertes lokales Maximum
	Bei $x=6$: wechselt von negativ auf positiv, also isoliertes lokales Minimum
	![[1a.png]]
	Nullstellen: $0, 9$
	$\lim_{x\to\infty} \arctan(x^3-9x^2) = \infty$
	$\lim_{x\to-\infty} \arctan(x^3-9x^2) = -\infty$
---
**Aufgabe 2**
a)  $f(x) = cosh(x):= \frac{1}{2}(e^x+e^{-x}) = \frac{1}{2} e^x + \frac{1}{2}e^{-x}$
$f'(x) =\frac{1}{2}e^x - \frac{1}{2}e^{-x}$
$f''(x) = \frac{1}{2}e^x+\frac{1}{2}e^{-x}$
$\frac{1}{2}e^x+\frac{1}{2}e^{-x} = 0$ <=> $x=0$
Bei $x = 0$:  $f''$ wechselt Vorzeichen, dass heisst dort befindet sich ein Wendepunkt. Da $f''$ immer positiv ist, ist f strikt konvex.

b) $f(x) = \ln(x+\sqrt{1 + x^2})$
$f'(x)\frac{1}{\sqrt{1+x^2}}$
$f''(x) = \frac{\frac{1}{2\sqrt{1+x^2}}}{1 + x^2} = \frac{1+x^2}{2\sqrt{1+x^2}}$
$f''$ hat keine (reelle) Nullstellen, also keine Wendepunkte. Da $f''$ immer positiv ist, ist $f$ strikt konvex.

c) $f(x) = \frac{1}{\sigma}\exp(-\frac{(x-x_0)^2}{2\sigma^2})$
$f'(x) = −\frac{(x − x_0)}{σ^3} \exp(-\frac{(x − x_0)^2}{2σ^2 })$
$f''(x) =\dfrac{\left(x-x_0\right)^2\mathrm{e}^{-\frac{\left(x-x_0\right)^2}{2{\sigma}^2}}}{{\sigma}^5}-\dfrac{\mathrm{e}^{-\frac{\left(x-x_0\right)^2}{2{\sigma}^2}}}{{\sigma}^3}$
Wendepunkt bei $x = x_0$, da dort $f'' = 0$ (und es das Vorzeichen wechselt).
Da $f'' > 0$  gilt, ist $f$ strikt konvex.
---
**Aufgabe 3**:
$f(x) = x^7 -\frac{7}{2}x^2 + 2$
$f'(x) = 7x^6 - 7x$ <=>$f'(x) = 0$ bei $x= 0$ und da $x^5 = 1$ auch bei $x=1$, dass heisst maximal 3 Nullstellen, nach Rolle. 
$f''(x) = 42x^5 -7$
$f(-1) = -1 - \frac{7}{2} + 2 = -2.5 < 0$
$f(-0.5) > 0$
Da $f''<0$ im Intervall $[-1, -0.5]$ ist die Funktion konkav, alo nur eine Nullstelle $x_*$ in diesem Intervall.
Newtonverfahren:
1. Erste Tangente: $y = f(-0.5) + f'(-0.5)(x-(-0.5))$ => $x = -0.81$
2. Zweite Tangente: $y = f(-0.81) + f'(-0.81)(x-(-0.81))$ => $x = -0.7413$
3. Dritte Tangente: $y = f(-0.7413) + f'(-0.7413)(x-(-0.7413))$ => $x = -0.734$


$f(0.2) > 0$ und $f(0.8)$ und eine Nullstelle von $f'$, also maximal 2 Nullstellen von $f$:
1) Erste Tangente: $y = f(0.2) + f'(0.2)(x-0.2)$ => $x= 1.529$
2) Zweite Tangente: $y = f(1.529) + f'(1.529)(x-1.529)$ =>= $x= 1.359$
3) Dritte Tangente: $y = f(1.359) + f'(1.359)(x-1.359)$ => $x= 1.2405$
4) Vierte Tangente: $y = f(1.2405) + f'(1.2405)(x-1.2405)$ => $x= 1.173$
5) 5. Tangente: $y = f(1.173) + f'(1.173)(x-1.173)$ => $x = -0.734$ => $x= 1.1491$
6) 6. Tangente: $y = f(1.1491) + f'(1.1491)(x-1.1491)$ => $x = -0.734$ => $x= 1.1461$
$f(0.8)< 0$
$f(0.5) > 0$ 


1. Erste Tangente: $y = f(0.8) + f'(0.8)(x-0.8)$ => $x = 0.792$ **Geraten...**
