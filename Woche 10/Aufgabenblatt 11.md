# Aufgabenblatt 11
**Aufgabe 1**
a)
Koeffizientenmatrix, Rang 3:
$\left(
\begin{array}{ccc|c}
2 &-1&3&5 \\
1 &2&-1  & 0\\
-4 & 1 & 0 & 1
\end{array}
\right) \stackrel{\longrightarrow}{\text{I*0.5}}\left(
\begin{array}{ccc|c}
1 &-0.5&1.5&2.5 \\
1 &2&-1  & 0\\
-4 & 1 & 0 & 1
\end{array}
\right)\stackrel{\longrightarrow}{\text{4*II+III}}$ 
$\left(
\begin{array}{ccc|c}
1 &-0.5&1.5&2.5 \\
0 &9&-4  & 1\\
-4 & 1 & 0 & 1
\end{array}
\right)\stackrel{\longrightarrow}{\text{II/9 und III+4*I}}\left(
\begin{array}{ccc|c}
1 &-0.5&1.5&2.5 \\
0 &1&-4/9 & 1/9\\
0 & -1 & 6 & 11
\end{array}
\right)$
$\stackrel{\longrightarrow}{\text{III+-2*I und III/3}}\left(
\begin{array}{ccc|c}
1 &-0.5&1.5&2.5 \\
0 &1&-4/9 & 0\\
0 & 0 & 1 & 2
\end{array}
\right)$
$x_3 =2$
$x_2  -\frac{4}{9}x_3 = \frac{1}{9}$ => $x_2 = 1$
$x_1 -0.5x_2 +1.5x_3 =2.5$ => $x_1 =2.5-3+0.5 = 0$

b)
$\left(
\begin{array}{cccc|c}
2 &-1&1&2&6 \\
-1 &0&3  & 1&2\\
-5& 1 & 8 & 1&0
\end{array}
\right) \stackrel{\longrightarrow}{\text{III und II vertauschen und I/2}}$
$\left(
\begin{array}{cccc|c}
1 &-0.5&0.5&1&3 \\
-5& 1 & 8 & 1&0\\
-1 &0&3  & 1&2\\
\end{array}
\right) \stackrel{\longrightarrow}{\text{II+5*I und III+I}}$
$\left(
\begin{array}{cccc|c}
1 &-0.5&0.5&1&3 \\
0& -1.5& 10.5 & 6&15\\
0&-0.5 &3.5&2  & 5\\
\end{array}
\right) \stackrel{\longrightarrow}{\text{II/-1.5 und III+II/-3}}$
$\left(
\begin{array}{cccc|c}
1 &-0.5&0.5&1&3 \\
0& 1 & -7 & -4&10\\
0&-0.5 &3.5&2  & 5\\
\end{array}
\right)\stackrel{\longrightarrow}{\text{III + II/2}}$
$\left(
\begin{array}{cccc|c}
1 &-0.5&0.5&1&3 \\
0& 1 & -7 & -4&10\\
0&0&0&0&0\\
\end{array}
\right)$, also nur Rang 2 und zwei Variablen frei wählbar.
$x_4, x_3 \in \mathbb R$
$x_2 = 10 + 7x_3 + 4x_4$
$x_1 = 8 + 3x_3 + 3x_4$
$\mathbb L = \left(
\begin{array}{c}
8\\
10 \\
0\\
0
\end{array}
\right)+
\left\{\begin{array}{ccc|c}\left(
\begin{array}{c}
x_3 \\
x_4\\
\end{array}
\right) 
\times
{| \forall x_3, x_4 \in \mathbb R}\end{array}\right\}$

---
**Aufgabe 2**
$\left(
\begin{array}{ccc|c}
1 & -2&5&4\\
2 & -3 & 4 & 0 \\
4& -5&2&-8\\
-1&3&\alpha&\beta
\end{array}
\right)\stackrel{\longrightarrow}{\text{II-2I}}$ $\left(
\begin{array}{ccc|c}
1 & -2&5&4\\
0 &1 & -6 & -8 \\
4& -5&2&-8\\
-1&3&\alpha&\beta
\end{array}
\right)\stackrel{\longrightarrow}{\text{IV +I-II und III streichen}}$ 
$\left(
\begin{array}{ccc|c}
1 & -2&5&4\\
0 &1 & -6 & -8 \\
0&0&\alpha+11&\beta+12
\end{array}
\right)$
a) 
leer, falls $\alpha = -11$ und $\beta \neq -12$, da dann die unterste Zeile $\left(\begin{array}{ccc|c}0&0&0&\beta+12\neq 0\end{array}\right)$ wäre und da $\beta +12 \neq 0$ gilt, und es daher keine Lösung gäbe.

b) 
einelementig, falls $\alpha \neq -11$ und $\beta \in \mathbb R$, da dann $\alpha + 11\neq0$ und die letzte Zeile dann so aussehen würde: $\left(\begin{array}{ccc|c}0&0&\alpha +11\neq 0&\beta+12\end{array}\right)$. Dies liefert eine reelle Lösung.

c) 
unendlich, falls  $\alpha = -11$ und $\beta = -12$, da dann die erweiterte Matrix mit der letzten Zeile $\left(\begin{array}{ccc|c}0&0&0&0\end{array}\right)$ auf Rang 2 wechselt, das Gleichungssystem aber 3 Unbekannten hat. Das heisst $x_3\in\mathbb R$ ist frei wählbar.

---
**Aufgabe 3**
$p(x) = ax^3 + bx^2+cx + d$ 
$p'(x) = 3ax^2 + 2bx + c$
$p(x) * 5x =5ax^4 + 5bx^3+5cx^2 + 5dx = f(x)$
$F(x) =ax^5 + \frac{5}{4}bx^4 + \frac{5}{3}cx^3 + \frac{5}{2}dx^2$
Gelten muss:
$-a + b-c+d = -1$
$8a +4b + 2c + d = 5$
$12a + 4b + c = 2$
$F(1) - F(-1) = a + \frac{5}{4}b + \frac{5}{3}c + \frac{5}{2}d - (-a + \frac{5}{4}b - \frac{5}{3}c + \frac{5}{2}d) = 2a + \frac{10}{3}c = 8$
Erweiterte Matrix des Gleichungssystems:
$\left(
\begin{array}{cccc|c}
-1 &1&-1&1&-1 \\
8& 4 & 2 & 1&5\\
12&4 &1&0  & 2\\
2&0&\frac{10}3&0  & 8\\
\end{array}
\right)\stackrel{\longrightarrow}{\text{I und IV vertauschen}}$
$\left(
\begin{array}{cccc|c}
2&0&\frac{10}3&0  & 8\\
8& 4 & 2 & 1&5\\
12&4 &1&0  & 2\\
-1 &1&-1&1&-1 \\
\end{array}
\right)\stackrel{\longrightarrow}{\text{I/2 und II +8IV}}$
$\left(
\begin{array}{cccc|c}
1&0&\frac{5}3&0  & 4\\
0& 12 & -6 & 9&-3\\
12&4 &1&0  & 2\\
-1 &1&-1&1&-1 \\
\end{array}
\right)\stackrel{\longrightarrow}{\text{II/12 und III +12IV}}$
$\left(
\begin{array}{cccc|c}
1&0&\frac{5}3&0  & 4\\
0& 1 & -0.5 & 0.75&-0.25\\
0&16 &-11&12  & -10\\
-1 &1&-1&1&-1 \\
\end{array}
\right)\stackrel{\longrightarrow}{\text{III-16II und IV + I}}$
$\left(
\begin{array}{cccc|c}
1&0&\frac{5}3&0  & 4\\
0& 1 & -0.5 & 0.75&-0.25\\
0&0 &-3&0  & -7\\
0 &1&\frac23&1&3\\
\end{array}
\right)\stackrel{\longrightarrow}{\text{III/-3 und IV-II}}$
$\left(
\begin{array}{cccc|c}
1&0&\frac{5}3&0  & 4\\
0& 1 & -0.5 & 0.75&-0.25\\
0&0 &1&0  & \frac73\\
0 &0&\frac76&0.25&3.25\\
\end{array}
\right)\stackrel{\longrightarrow}{\text{IV -(7/6)II}}$
$\left(
\begin{array}{cccc|c}
1&0&\frac{5}3&0  & 4\\
0& 1 & -0.5 & 0.75&-0.25\\
0&0 &1&0  & \frac73\\
0 &0&0&0.25&3.25+\frac{7^2}{18}\\
\end{array}
\right)\stackrel{\longrightarrow}{\text{IV*4}}$
$\left(
\begin{array}{cccc|c}
1&0&\frac{5}3&0  & 4\\
0& 1 & -0.5 & 0.75&-0.25\\
0&0 &1&0  & \frac73\\
0 &0&0&1&13+\frac{196}{18}\\
\end{array}
\right)$
$d= 13+\frac{196}{18} = 23.\overline8$
$c =\frac{7}{3}$
$b=-0.25+\frac{7}{6}-0.75*23.\overline8 = -17$
$a =4 - \frac{35}{9} = 0.\overline1$
$p(x) = 0.\overline1x^3-17x^2+\frac{7}{3}x + 23.\overline8$