# Aufgabenblatt 13
**Aufgabe 1**
a) Drei Vektoren sind abhängig wenn $det(u,v,w) = -3 (-2.5-2x)+2(x+0.25) = 0$ => $x = -1$
b) Volumen eines Würfels mit Seitenlänge 2 ist 8
Da Determinante als Volumen des Spatens interpretiert werden kann, muss folgendes gelten:$det(u,v,w) = -3 (-2.5-2x)+2(x+0.25) = 8$ => $x = 0$

---
**Aufgabe 2**
$u = \left(\begin{array}{c}x_1\\y_1\\z_1\end{array}\right)$

$v = \left(\begin{array}{c}x_2\\y_2\\z_2\end{array}\right)$

$u\times v = \left(\begin{array}{c}y_1z_2 - z_1y_2\\z_1x_2-x_1z_2\\x_1y_2-y_1x_2\end{array}\right)$

 $w = \left(\begin{array}{c}x_3\\y_3\\z_3\end{array}\right)$

a) $\langle u\times v ,e_1\rangle =y_1z_2-z_1y_2 = 1*\left|\begin{array}{c}y_1&y_2\\z_1&z_2\end{array}\right|= \det(u,v,e_1)$
$\langle u\times v ,e_2\rangle =z_1x_2-x_1z_2= 1*\left|\begin{array}{c}x_1&x_2\\z_1&z_2\end{array}\right|= \det(u,v,e_2)$
$\langle u\times v ,e_3\rangle =x_1y_2-y_1x_2= 1*\left|\begin{array}{c}x_1&x_2\\y_1&y_2\end{array}\right| = \det(u,v,e_3)$

b)
$\langle u\times v ,w\rangle =x_3(y_1z_2-z_1y_2) + y_3(z_1x_2-x_1z_2)+z_3(x_1y_2-y_1x_2)$
$= x_3*\left|\begin{array}{c}y_1&y_2\\z_1&z_2\end{array}\right|+y_3*\left|\begin{array}{c}x_1&x_2\\z_1&z_2\end{array}\right|+z_3*\left|\begin{array}{c}x_1&x_2\\y_1&y_2\end{array}\right|= \det(u,v,w)$

c)
$v\times u =\left(\begin{array}{c}z_1y_2 -y_1z_2 \\x_1z_2-z_1x_2\\y_1x_2-x_1y_2\end{array}\right)$ => $-1*\left(\begin{array}{c}z_1y_2 -y_1z_2 \\x_1z_2-z_1x_2\\y_1x_2-x_1y_2\end{array}\right) = \left(\begin{array}{c}y_1z_2 - z_1y_2\\z_1x_2-x_1z_2\\x_1y_2-y_1x_2\end{array}\right) = -(v\times u) = u\times v$

$v\times w = \left(\begin{array}{c}y_2z_3 - z_2y_3\\z_2x_3-x_2z_3\\x_2y_3-y_2x_3\end{array}\right)$

$w\times u =\left(\begin{array}{c}y_3z_1 - z_3y_1\\z_3x_1-x_3z_1\\x_3y_1-y_3x_1\end{array}\right)$

$x_1y_2z_3 - x_1z_2y_3 + y_1z_2x_3-y_1x_2z_3 + z_1x_2y_3-z_1y_2x_3 = \langle u,v\times w \rangle =\langle w, u\times v\rangle = \langle v, w\times u\rangle$

---
**Aufgabe 3**
a) Hier bin ich mir nicht sicher: Bei der Streckung sehe ich kein Problem, da man einfach $\lambda$ oder $\micro$ verändern kann. Bei der Addition kann es zum Beispiel vorkommen, dass eine Zeile der Summe eine Nullzeile ist, während die anderen befüllt sind. Damit ist die Summe nicht in $U$ und $U$ ist kein linearer Unterraum von $\mathbb R^3$
b) Unterraum von $\mathbb R^3$: Gerade im Raum, weil es ein Schnittpunkt zwischen zweier Ebenen ist.
c) Unterraum von $\mathbb R^3$, da jegliche Streckung und/oder Addition nicht den Winkel verändern kann und daher jede Summe zweier Elemente und jede Streckung eines Elements auch einen Winkel von 45° mit der z-Achse bilden.
d) Kein Unterraum von $\text{Mat}_{2\times2}$, denn damit eine Matrix eine Determinante von 0 hat, muss der Rang nicht voll sein, dass heisst eine Spalte oder eine Zeile muss nur aus Nullen bestehen. Man kann also zum Beispiel also eine Matrix der Menge bei der die zweite Zeile aus Nullen besteht und eine bei der die Zweite Spalte nur aus Nullen besteht aus der Menge addieren und erhält eine Matrix bei der keine Nullzeilen oder -spalten vorhanden sind.
e) Unterraum von  $\text{Mat}_{2\times2}$, denn jede Addition und Skalarmultiplikation behält die gleiche Form und das Resultat ist daher in der Menge vorhanden.