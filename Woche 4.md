# Woche 4
----
![[skriptMMI4.pdf]]

## Grenzwerte von Funktionen
### 2.3 Elementare Funktionen:
**Beispiel 3.4.2:**:
1) $f(x) = arctan(1/x^2)$
	$1/x^2$ ist an der y-Achse symmetrisch, dass heisst $arctan(1/x^2)$ ist auch symmetrisch.
	Da $1/x^2$ streng monoton fallend ist, ist $arctan(1/x^2)$ auch monot fallend für $x ≥ 0$
	
	$\lim_{x\to\infty} arctan(1/x^2) = arctan(\lim{x\to \infty} 1/x^2) = 0$
	$\lim_{x\to 0} arctan(1/x^2) = \pi/2$, weil $1/x^2$ gegen unendlich geht und $lim_{x\to\infty} arctan(x) = \pi/2$

Mehr Beispiele schaue Skript, bin faul :) 

Elementare Funktionen (und deren Kombinationen) sind nützlich um natürliche Prozesse zu modellieren. Sei dies der Bevölkerungswachstum, Schwingungen oder radioaktiver Zerfall.

---
## Stetigkeit von Funktionen
### Definition 2.4.1 :
Eine Funktion f heisst stetig an der Stelle $x_0$, wenn $lim_{x\to x_0} f(x) = f(x_0)$.
Andare Charakterisierung:
$f$ ist stetig bei $x_0$, wenn zu jedem $\epsilon >0$ ein $\delta <0$ existiert, so dass $|x-x_0| < \delta$ und $|f(x) - f(x_0)| < \epsilon$.

Für Beispiele siehe [[skriptMMI4.pdf]].
![[Aufgabenblatt 5]]