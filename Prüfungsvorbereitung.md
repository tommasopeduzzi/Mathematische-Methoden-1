# Prüfungsvorbereitung
**Woche 1**
- Beweise
	- Beweisstrategien:
		- Direkter Beweis: Beweis direkt aus grundlegenden Sätzen (Axiomen) hergeleitet.
		- Widerspruchsbeweis: Geht daraus hervor, dass eine mathematische Aussage nur entweder falsch oder wahr sein kann. Dann geht man vom Gegenteil der zu beweisenden Aussage aus und folgt daraus einen Widerspruch. Dieser Widerspruch kann gegen eine bereits bewiesene Aussage oder das zu beweisende selber sein.
- Graphen: Menge aus Punkten und Kanten, die die Punkte verbinden.
	- Baum: Ein Graph ist eine Menge aus $n>=2$ Punkten die mit genau $k = n-1$ Kanten verbunden sind und in denen es keine Teilfiguren gibt (Graph ist zusammendhängend). Darause folgt das der Graph keine Loops haben kann.
	- Prüfer-Codes für Bäume: Eindeutige Zahlenfolge mit $n-2$ Zahlen für Bäume mit durchnummerierten Knoten. Daraus folgt, dass es mit $n$ Knoten $n^{n-2}$ verschiedene Bäume gibt.
		- Prozess fürs konstruieren des Codes: Man sucht das freie Ende mit der höchsten Zahl und notiert den Nachbarn. Dann löscht man das Ende. Wiederholen, bis nur ein Punkt übrig ist.
		- Prozess für das rekonstruieren des Graphens: Den Anfang bildet der letzte Knoten des Codes und die kleinste Zahl, die nicht im Code vorkommt. Danach wird für jeden Eintrag des Codes von rechts nach links der Knoten, der am kleinsten ist und noch nicht gebraucht wurde mit dem Eintrag verbunden.
- Vollständige Induktion: Beweismethode für Aussagen in den natürlichen Zahlen. Man geht davon aus, dass wenn für das kleinste Element einer Menge eine Aussage gilt und wenn man beweisen kann, dass diese Aussage für jedes Nachfolgende Element gilt, gilt es für alle Element der Menge.
	- Induktionsverankerung: Fall mit dem kleinsten Element der Menge wird nachgerechnet.
	- Induktionsschritt: Man soll beweisen, dass die Aussage, bei welcher man annimmt, dass sie mit $n$  gilt, auch mit $n+1$ gilt. Dafür muss man die Aussage so umformen, dass alle $n$ zu $n+1$ werden.

**Woche 2**
- Binomialkoeffizienten: Es gibt  $\begin{pmatrix}n\\ k\end{pmatrix} = \frac{n!}{(n-k)!k!}$ Möglichkeiten aus n Elementen k auszuwählen. Der Teil $\frac{n!}{(n-k)!}$ gibt an, wie viele verschiedene Listen aus $k$ Elementen man aus $n$ Elementen nehmen kann. Dann wird noch durch $k!$ dividiert, da das die Anzahl verschieden geordneter Listen mit $k$ Elementen ist und die Reihenfolge egal ist. Ausserdem kann man Binomialkoeffizienten auch rekursiv defininieren: $\begin{pmatrix}n\\ k\end{pmatrix} = \begin{pmatrix}n-1\\ k\end{pmatrix} + \begin{pmatrix}n-1\\ k-1\end{pmatrix}$, mehr dazu im Skript.
	- Das Pascalsche Dreieck besteht aus Zahlen die folgendermassen bestimmt werden: Jede Zahl ist $\begin{pmatrix}n\\ k\end{pmatrix}$, wobei n die Zeile und k die Diagonale von rechts oben nach links unten ist. Ausserdem kann man ein Element definieren, in dem man das Element rechts oben und das link oben zusammenaddiert. Dies stimmt mit der Rekursionsformel überein.
	- Binomischer Lehrsatz: Folgendes gilt für $a,b \in \mathbb R$ und $n\in \mathbb N$: $(a+b)^n = \sum_{k=0}^n \begin{pmatrix}n\\ k\end{pmatrix}a^{n-k}b^k = \begin{pmatrix}n\\ 0\end{pmatrix}a^n + \begin{pmatrix}n\\ 1\end{pmatrix}a^{n-1}b + ... +\begin{pmatrix}n\\ n-1\end{pmatrix}ab^{n-1}+\begin{pmatrix}n\\ n\end{pmatrix}b^n$ Beweis im Skript.
- Eulersche Polyederformel: Für jeden planaren Graphen (Graph mit keinen sich kreuzenden Kanten -> Graph, der die Ebene in endliche viele Teile unterteilt, inklusive Aussenseite) gilt folgendes: $e - k + f = 2$, wobei e die Anzahl Ecken, k die Anzahl Kanten und f die Anzahl Flächen ist. Beweis mit Induktion über $n \in \mathbb N$ im Skript. Da man ein konvexes Polyeder auch als planaren Graphen auf eine 2-dimensionale Fläche projezieren kann, gilt die Formel auch für konvexe Polyeder mit e Ecken, k Kanten und f Flächen.
- (Über-)Abzählbarkeit: Grössen unendlicher Mengen können verschieden sein. So ist zum beispiel die Menge alle natürlichen Zahlen $\mathbb N$ kleiner als die aller ganzen Zahlen $\mathbb Z$. Es folgen wichtige Begriffe um Grössen uneendlicher Mengen zu kategorisieren:
	- Gleichmächtigkeit: Zwei Mengen A und B sind gleichmächtig, wenn jedem Element aus der Menge A ein Element aus der Menge B und vice versa zugeordnet werden kann. Die Abbildung f welche die Menge A auf die Menge B und vice versa abbildet nennt man eine bijektive Zuordnung oder eine 1:1-Abbildung.
	- Eine unendlich Menge ist abzählbar, wenn sie gleichmächtig ist wie $\mathbb N$ und überabzählbar wenn das nicht der Fall ist.
	- Die Menge der rationalen Zahlen $\mathbb Q_{>0}$ ist abzählbar, weil jedes Element (p/q) auf eine Koordinatensystem ausgelegt werden kann und eine Linie durchgezeichnet kann. Daher kann man diese Menge auf die natürlichen Zahlen abbilden und sie ist abzählbar.
	- Ist die Menge M Teil der Menge L und M ist nicht abzählbar, so ist L auch überabzählbar.
	- Man nehme an, man hätte eine Liste aller irrationalen Zahlen. Würde man die Diagonale dieser Liste nehmen hätte man eine neue irrationale Zahl, was der Behauptung widerspricht man hätte eine Liste aller irrationalen Zahlen. Daher ist die Menge aller irrationalen Zahlen überabzählbar.

**Woche 3**
- Zahlenfolge: Eine Zahlenfolge ist eine Liste an Zahlen die einer Bedingung entsprechen. Ein Beispiel ist $2,4,6,8,...$ welche die Bedingung $a_n = 2n$ hat.
- Grenzwert:
	- Wenn man für jeden Streifen mit der Breite $\epsilon > 0$ um die x-Achse ein Element der Folge findet, nach welchem die Zahlen nur noch im Streifen sind, so konvergiert die Folge gegen 0. Also muss es für jedes $\epsilon > 0$ mindestens einen Wert $n_0$ geben ab welchem alle Werte  im Bereich $-\epsilon$ und $\epsilon$ liegen.
	- Für jeden noch so dünnen Streifen um die x-Achse liegen bis auf endlich viele Ausnahmen alle Punkte im Streifen.
	- Um $n_0$ mit einem bestimmten $\epsilon$ zu finden, muss man $a_n < \epsilon$ nach $n$ auflösen und den kleinst möglichen Wert für $n$ der die Gleichung erfüllt. Dieses $n = n_0$.
- Konvergenz von Folgen
	- Man sagt eine Folge konvergiert gegen a, wenn die Differenz $a-a_n$ gegen null konvergiert. Dann verwendet man folgende Schreibweise: $\lim_{x\to\infty}a_n = a$
	- Man sagt eine Folge $a_n$ konvergiert gegen Unendlich ($\infty$) wenn die Folge $\frac1{a_n}$ gegen 0 konvergiert.
- Rechenregeln mit Grenzwerten:
	- $\lim_{n\to\infty} a_n\pm b_n = \lim_{x\to\infty}a_n \pm \lim_{x\to\infty}b_n$
	- $\lim_{n\to\infty} a_n\cdot b_n = \lim_{x\to\infty}a_n \cdot \lim_{x\to\infty}b_n$ 
	- Falls $\lim_{x\to\infty}b_n \neq 0$: $\lim_{n\to\infty} \frac{a_n}{ b_n} = \frac{\lim_{x\to\infty}a_n }{\lim_{x\to\infty}b_n}$

**Mehr zu Woche 3: Grenzwerte von Summen etc**

**Woche 4**
- Umkehrbarkeit von Funktionen:
	- Eine Funktion f, die die Definitionsmenge D auf die Wertemenge W abbildet, ist bijektiv, wenn man eine Umkehrfunktion g bilden kann welche die Wertemenge auf die Definitionsmenge von f abbildet.
	- Eine Funktion ist streng monoton steigend auf eine Teilmenge M von  D, wenn $f(x_1) < f(x_2) \forall x_1<x_2, x_i \in M$. Entsprechend ist eine Funktion streng monoton fallend auf eine Teilmenge M von D, wenn $f(x_1) > f(x_2) \forall x_1<x_2, x_i \in M$.
	- Ist eine Funktion streng monoton fallend/steigend auf eine Teilmenge M von D, so ist diese auf M umkehrbar.
- Grenzwerte von Funktionen:
	- Man sagt eine Funktion konvergiert an der Stelle $x_0$ gegen $y_0$ wenn für Folge in der Definitionsmenge die gegen $x_0$ konvergiert, die Folge der Funktionswerte der Folge gegen $y_0$ konvergiert.
	- Wenn eine Funktion f an der Stelle $x_0$ gegen $y_0$ konvergiert, so schreibt man:
		- $\lim_{x\to x_0} f(x) = y_0$ 
	- Wenn alle Folgen $x_n > x_0$, die gegen $x_0$ konvergieren, die Folge der Funktionswerte der Folge gegen $y_0$ konvergiert, so spricht man vom rechtsseitigen Grenzwert und schreibt:
		-  $\lim_{x\searrow x_0} f(x) = y_0$ 
	- Wenn alle Folgen $x_n < x_0$, die gegen $x_0$ konvergieren, die Folge der Funktionswerte der Folge gegen $y_0$ konvergiert, so spricht man vom rechtsseitigen Grenzwert und schreibt:
		-  $\lim_{x\nearrow x_0} f(x) = y_0$ 
	- Existiert an einer Stelle der rechtsseitige und der linksseitige Grenzwert und ist dieser gleich, so ist das der beidseitige Grenzwert.
	- Beispiele im Skript.
- Elementare Funktionen: Durch Kombinationen von Elemantaren Funktionen, die Trigonometrischen Funktionen, Exponentialfunktion und rationalen Funktionen, und deren Verknüpfungen durch Grundrechenarten, Umkehrung und die Zusammensetzung dieser Funktionen können viele verschieden Funktionen gebildet werden. 
	- Die trigonometrischen Funktionen ((arc)sin, (arc)cos, (arc)tan, etc) können am rechtwinkligen Dreieck und am Einheitskreise anhand von Beziehungen zwischen Winkel und verschiedenen Längen definiert werden. Zum Beispiel folgt aus dem Einheitskreis das für alle Winkel $\alpha$ folgendes gilt: $\cos(\alpha)^2 + \sin(\alpha)^2 =1$. Die Umkehrfunktionen der trigonometrischen Funktionen werden als die Arcusfunktionen bezeichnet.
	- Die Exponentialfunktion ist ihrer elementarsten Form eine Reihe $a^{n+1} = a\cdot a^n$$\forall n\in \mathbb N$. Diese Reihe kann auf Exponenten in den ganzen Reellen Zahlen vergrössert werden. Ein Spezialfall der Exponentialfunktion ($f(x) = a^x$) ist die Exponentialfunktion mit der Basis ($f(x) = exp(x) = e^x$), wobei $e$ als folgendes definiert werden kann $\lim_{n\to\infty}(1+\frac1n)^n$. Die Umkehrfunktion der Expontialfunktion mit der Basis a ($f(x)=a^x$) ist der Logarithmus der Basis a $g(x) = \log_a(x)$ und $\log_e(x) = \ln(x)$. Jede Exponentialfunktion kann mithilfe von e definiert werden: $f(x) = a^x = e^{ln(a)x}$ Die Exponentialfunktion kann für die Beschreibung Wachstums oder Verfalls sehr nützlich sein.
- Stetigkeit: Eine Funktion $f$ ist an der Stelle $x_0$ stetig, wenn der beidseitige Grenzwert an der Stelle $x_0$ exisistiert und $\lim_{x\to x_0} f(x) = f(x_0)$ gilt. 
	- Eine Funktion die aus stetigen Funktionen zusammengesetzt ist, ist selber stetig.
	- Zwischenwertsatz: Man nehme eine stetige Funktion f und ein Intervall $[x_1,x_2]$ in $\mathbb D$.  Man nehme an, $f(x_1) < y_0 < f(x_2)$ oder $f(x_1) > y_0 > f(x_2)$. Dann gibt es ein $x_0 \in  [x_1,x_2]$, so dass $f(x_0) = y_0$. 
	- Eine stetige Funktion nimmt in einem abgeschlossenen Intervall ihr Maximum und Minimum an.
	- Eine stetige Funktion bildet ein abgeschlossenes Intervall auf ein abgeschlossenes Intervall ab.

**Woche 5**
- Komplexe Zahlen: Beweggrund für die Erfindung komplexer Zahlen war die Suche nach Lösung belieber Polynome n-ten Grades. Das Problem ist, dass bei der Allgemeinen Lösung die Disriminante (der Teil in der Wurzel) oft $≤ 0$    ist. Da es in den reellen Zahlen $\mathbb R$ aber keine Lösung für die Quadratwurzel einer negativen Zahl gibt, musste etwas dazu erfunden werden
	- Die Imaginäre Zahl: Um dieses Problem zu lösen wurde die Zahl $i = \sqrt{-1}$ definiert. Also gilt: $i^2 = 1$
	- $a + ib$: Um komplexe Zahlen auszudrücken werden reelle Vielfachen von $i$ mit einer Konstanten im reelen Zahlenbereich addiert ($a, b \in \mathbb R$). Gerechnet wird mit komplexen Zahlen nach den den bereits bekannten algebraischen Gesetzen mit den oben erklärten Spezialregeln für $i$. Da für die Komplexen Zahlen ($\mathbb C = {a+ib|a,b\in\mathbb R}$) die gleichen Gesetze für die Addition und Multiplikation sie werden als Körper kategorisiert.
	- Gaussche Zahlenebene: Komplexe Zahlen kann man geometrisch auf der Gausschen Zahlenebene abbilden. Es gilt dabei folgende Abbildung: $\mathbb C \to \mathbb R^2$, da $z = a+ib \to (a,b)$ gilt. Es handelt sich hier um eine bijektive Abbildung, denn zu jeder komplexen Zahl gibt es genau einen Punkt auf der Zahlenebene und umgekehrt.
		- Um Zahlen auf der Gausschen Zahlenebene zu zeichnen, werden auf der x-Achse die reellen Zahlen und auf der y-Achse die rein imaginären Zahlen, also Vielfache von $i$, geplottet. Auf der Ebene gibt es einen sogenannten Ortsvektor, die Distanz zum Nullpunkt: $|z| = |a+ib| = \sqrt{a^2+b^2}$. Dieser Ortsvektor kann auch als der absolute Wert der komplexen Zahl $z$ interpretiert werden.
	- Eine zu einer komplexen Zahl $z = a + ib$ konjugierten komplexe Zahl $\overline z = a -ib$. Damit hat ein komplexes Polynom immer mindestens ein konjugiertes Paar von komplexen Lösungen. Eine Konjunktion in der Gausschen Zahlenebene bedeutet eine Spiegelung an der rellen Achse (x-Achse). Mit der Konjunktion lässt sich das Inverse einer komplexen Zahl einfach beschreiben durch: $z^{-1} = \frac {\overline z} {|z|^2}$.
	- Eine Multplikation einer komplexen Zahl mit $i$ kann als Drehung um 90° oder $\pi/2$ um den Nullpunkt gedacht werden. Um das besser zu verstehen werden komplexen Zahlen oft mit ihren Polarkoordinaten. Dafür ordnet man jeder komplexen Zahl $z$  einen Betrag $|z|$, sowie dem Winkel zwischen der Zahl auf der Gausschen Zahlenebene und der reellen Achse, gemessen gegen den Uhrzeigersinn $arg(z)$, zu. Durch diese zwei Argumente ist die Zahl bereits definiert. Man kann diese Werte auch wieder in kartesische Koordinaten und umgekehrt rechnen. Hier spielt also die Trigonometrie eine grosse Rolle. Mehr dazu, speziell zur Berechnung dieser Argumente, im Sript.
	- Für Argumente gilt ausserdem Folgendes. $arg(z\cdot w) = arg(z) + arg(w)$.
- Euler's Identität: Dank Euler ist bekannt: $e^{i x} = cos(x) + sin(x)$. Die Herleutung dazu findet man im Skript. Daher gilt Eulers bekannte Identität: $e^{i\pi} = -1$. Alle komplexen Zahlen der Form $e^{i\phi}$ liegen in der Gausschen Zahlenebene auf dem Einheitskreis. Daher gilt folgendes.
	- Für eine beliebige komplexe Zahl $z$ gilt: $z = a+ib=|z|e^{i\arg(z)}$. Zum Beispiel: $2 + i =\sqrt{2^2+1}\cdot e^{i\arctan(2)}=\sqrt5e^{i\arctan(2)}$. Diese Eigenschaft ist nützlich um Wurzeln im Komplexen zu ziehen: $(2 + i)^{10} =\sqrt5^{10}e^{i\cdot10\cdot\arctan(2)}$ oder $\sqrt{(2 + i)} =\sqrt5^\frac12({e^{i\arctan(2))}})^{\frac12}$ 

- Einheitswurzel komplexer Zahlen: für die gleichung $z^n = 1$ gibt es für $z$ n Lösungen in der Form $z_k = e^{ik\phi}$, wobei $\phi = \frac {2\pi} n$. Auf der Gausschen Zahlenebene bilden diese Lösungen ein regelmässiges n-Eck um den Nullpunkt. 
- Polynome im Komplexen: Daher kann aus Kombinationen von Vielfachen dieser Potenzen Polynome bilden. Für Polynome Polynome dritten und vierten Grades wurden von italienischen Mathematikern Formeln gefunden.
- Fundamentalsatz der Algebra: Über $\mathbb C$ hat jedes Polynom n-ten Grades eine Nullstelle. Diese Aussage kann über Induktion und Polynomendivision so umformen, dass auch gilt, dass jedes Polynom n-ten Grades über $\mathbb C$ n Lösungen, mit Vielfachheiten mitgezählt.

**Woche 6**
- Ableitung: Bei einer Funktion kann die Ableitung einer Funktion f an der Stelle $x_0$ als die Steigung der Tangente an der Stelle $x_0$ interpretiert werden. Die erste Ableitung  wird $f'$ genannt und kann so definiert werden: $f'(x_0) = \frac{d}{dx} f(x_0)$ .
- Differenzierbarkeit: Eine Funktion f ist an einer Stelle $x_0$ differenzierbar wenn der folgende Grenzwert existiert: $f'(x_0) = \lim_{x\to x_0} \frac{f(x_0) -f(x)}{x_0-x}$ 
- Einige Beispiele:
	- $f(x) = cx$ $\forall c\in\mathbb R$, so ist $f'(x) = c$
	- $f(x) = e^x$, so ist $f'(x) = e^x$
	- $f(x) = x^n$, so ist $f'(x) = nx^{n-1}$
	- $sin(x)' = cos(x)$, $cos(x)' = -sin(x)$, $(-sin(x))' = -cos(x)$, $(-cos(x))' = sin(x)$
- Dreigliedentwicklung: Ist eine Funktion f an der Stelle $x_0$ differenzierbar, kann eine sogenannte Dreigliedsumme aufgestellt werden: $f(x) = f(x_0) + f'(x_0)(x-x_0) + R(x)$, wobei R die Differenz die Differenz zwischen dem Wert x auf der Tangente und dem Wert auf der Funktion und $f(x_0) + f'(x_0)(x-x_0)$ die Tangente am Punkt $x_0$ beschreibt. **Bin mir hier etwas unsicher...**
- Rechenregeln für Ableitungen:
	- $(\alpha f \pm \beta g)'(x) = \alpha f'(x) \pm \beta f'(x)$    $\forall \alpha,\beta \in \mathbb R$ 
	- $(f\cdot g)'(x) = f'(x)g(x) + f(x)g'(x)$
	- $(\frac fg)'(x) = \frac{f'(x)g(x) - f(x)g'(x)}{g(x)^2}$ 
	- $(f(g(x)))' = f'(g(x)) \cdot g'(x)$ 
	- $g(x) = \frac1{f(x)}$, so gilt $g'(x) = \frac1{f'(g(x))}$ 
- L'Hopitâlsche Regel: $\lim_{x\to x_0} \frac{f(x)}{g(x)} = \lim_{x\to x_0} \frac{f'(x)}{g'(x)}$

**Woche 7**
- Lokale Extrema: Hat eine Funktion f an der Stelle $x_0$ einen Wert $\delta > 0$, so dass gilt $f(x_0) \geq f(x)$ $\forall x \in (x-\delta, x + \delta)$ hat f an der Stelle $x_0$ ein lokales Maximum. Gilt  sogar $f(x_0) > f(x)$ $\forall x \in (x-\delta, x + \delta)$, so ist an der Stelle $x_0$ ein isoliertes lokales Maximum zu finden. Umgekehrtes gilt für Minima: Hat eine Funktion f an der Stelle $x_0$ einen Wert $\delta > 0$, so dass gilt $f(x_0) \leq f(x)$ $\forall x \in (x-\delta, x + \delta)$ hat f an der Stelle $x_0$ ein lokales Minimum. Gilt  sogar $f(x_0) < f(x)$ $\forall x \in (x-\delta, x + \delta)$, so ist an der Stelle $x_0$ ein isoliertes lokales Minimum zu finden. 
	- Hat eine Funktion f an der Stelle $x_0$ ein lokales Extrema, so gilt: $f'(x_0) = 0$. Die Nullstellen der Ableitung nennt man auch kritische Stellen.
	- Satz von Rolle: Zwischen zwei gleichen Funktionswerteen befindet sich mindestens eine kritsche Stelle. Formell heisst das: Hat eine Funktion f die Stellen $x_1, x_2$ $x_1 < x_2$ und $f(x_1) = f(x_2)$ so existiert mindestens ein $x_0 \in [x_1, x_2]$, wo gilt $f'(x_0) = 0$.
	- Mittelwertsatz: Hat eine Funktion f zwei Stellen $x_1, x_2$ $x_1<x_2$, so existiert mindestens ein $x_0\in [x_1, x_2]$, wo gilt $f'(x_0) = \frac{f(x_2) -f(x_1)}{x_2-x_1}$. Das heisst an der Stelle $x_0$ ist die Tangente parallel zur Gerade durch $x_1$ und $x_2$.
- Höhere Ableitungen: Die zweite Ableitung einer differenzierbaren Funktion f ist definiert als: $f''(x) = \frac{d}{dx}f'(x)$. Allgemeiner gilt: $f^n(x) = \frac d {dx} f^{n-1}(x)$ für höhere Ableitungen.
	- Diese höhere Ableitung, speziel die zweite Ableitung kann zur Beurteilung kritischer Stellen benutzt werden: Ist $x_0$ eine kritische Stelle einer Funktion f, also gilt: $f'(x_0) = 0$. 
		- Ist $f''(x_0) < 0$, so ist die kritische Stelle ein lokales Maximum.
		- Ist $f''(x_0) > 0$, so ist die kritische Stelle ein lokales Minimum.
		- Ist $f''(x_0) = 0$, und wechselt $f'$ in der Nähe von $x_0$ das Vorzeichen nicht, so ist die kritische Stelle ein Sattelpunkt. 
- Newtonverfahren: Das Newtonverfahren ist ein Algorithmus mit welchem man Nullstellen approximieren kann. Dafür nimmt man für jeden Schritt die Ableitung der Funktion an der Stelle wo die Tangente der Ableitung des vorherigen Schrittes die x-Achse schneidet oder für den ersten Schritt einen Startwert $b$ in der Nähe einer Nullstelle. Formell ist das: $x_1 = b$ und $x_{n+1} = x_n - \frac{f(x_n)}{f'(x_n)}$. Dieses Verfahren konvergiert gegen eine Nullstelle.

**Woche 8**
- Das Integral: Unabhängig voneinander entwickelten Newton, Leibniz und Bernoulli das Integrieren von Funktionen, um die Fläche unter der Funktion zu berechnen, mithilfe von Stammfunktionen, also dem Gegensatz der Differenzialrechnung. 
- Riemann-Integral: Ein Integral kann man als Grenzwert einer Riemannssumme einer Funktion interpretieren, wobei eine Riemannssumme folgende Definiton hat: $R_{T_n}(f) = \sum_{k=0}^{n} f(\mathcal E_k)(x_k - x_{k-1})$, wobei $\mathcal E_k \in [x_{k-1}, x_k]$. Ein Riemann Integral einer Funktion f ist also definiert als $\lim_{n\to\infty} R_{T_n} (f)$. Wählt man als $\mathcal E$ das Minimum der Funktion im jeweiligen Intervall so spricht man von der Untersumme. Wählt man als $\mathcal E$ das Maximum der Funktion im jeweiligen Intervall so spricht man von der Obersumme. Die Schwankungssumme einer bestimmten Teilung T wird als die Differenz der Obersumme und Untersumme definiert. Gibt es für jeden Wert $\epsilon > 0$ eine Teilung T einer Funktion f auf einem Intervall $[a,b]$, bei der die Schwakungssumme $D_T(f) \leq \epsilon$, so ist die FUnktion Riemann-integrierbar und es gilt folgendes: $\int_a^bf(x)dx = \lim_{n\to\infty} R_{T_n} (f)$ 
	- Jede auf $[a,b]$ stetige Funktion ist auf dem Intervall Riemann-integrierbar.
- Regeln für Riemann-Integrale:
	- Linearität: $\int_a^b (f(x)+g(x)) dx = \int_a^b f(x) dx + \int_a^b g(x)dx$ und $\int_a^b \lambda \cdot f(x)dx = \lambda \int_a^b f(x)dx$ 
	- Monotonie: Falls gilt $f(x) \leq g(x)$ $\forall x\in[a,b]$, so gilt auch $\int_a^bf(x)dx \leq \int_a^bg(x)dx$ 
	- Betragsregel: $\left|\int_a^bf(x)dx\right| \leq \int_a^b|f(x)|dx$  
	- Additivität der Intervalle: $\int_a^t f(x)dx + \int_t^bf(x)dx = \int_a^bf(x)dx$
	- Folgerung 1: Verändert man endlich viele Werte einer Funktion in eine Intervall $[a,b]$, so bleibt das Riemann-Integral auf $[a,b]$ gleich.
	- Folgerung 2: Ist eine Funktion f auf dem Intervall $[a,b]\backslash T$ stetig und gibt es endlich viele rechts- bzw. linkseitige Grenzwerte $\lim_{x\searrow\text{oder}\nearrow x_k}f(x)$  so ist f auf dem Intervall $[a,b]$ Riemann-Integrierbar.
- Mittelwertsatz der Integralrechnung: Ist eine Funktion f auf dem Intervall $[a,b]$ stetig, so gibt es einen Wert $\tau\in [a,b]$, so dass $f(\tau) = \frac{\int_a^bf(x)dx}{b-a}$.
- Stammfunktionen: Eine Integral einer stetigen Funktion f auf $[a,b]$ $\int_a^b f(x)dx = F(b)-F(a) = F(x) \Biggr|_{a}^{b}$, wobei $F' = f$. Für ein unbestimmtes Integral einer Funktion f $\int f(x)dx = F(x) + C$. Im Skript ist eine Liste der wichtigsten Stammfunktionen zu finden. 
- Regel der Partiellen Integration: $\int_a^b f(x)g'(x) dx = -\int_a^b f'(x)g(x) dx + f(x)g(x)\Biggr|_a^b$ oder $\int_a^b f(x)g'(x) dx + \int_a^b f'(x)g(x) dx = f(x)g(x)\Biggr|_a^b$ 

**Woche 9**
- Substitutionsregel: Ein Integral kann so umgeschrieben werden, dass es einfacher ist es zu berechnen. Um das zu tun muss eine Substitution u mit Hilfe von x definiert werden, die Ableitung von u über x und damit du berechnet werden und die Grenzen in u einsetzen und neu berechnen. Ein Beispiel soll folgen:
	- Man nehme das Integral $\int_0^a (2-3x)^4dx$ und $u = 2-3x$. Daher ist $\frac {du}{dx} = -3$ => $du =-3dx$. Das Integral kann nun folgendermassen über u geschrieben werden: $-\frac13\int_{2-3\cdot0}^{2-3a} u^4 du$, was einfacher zu berechnen ist. Der Koeffizient $-\frac13$ ist da um den Koeffizienten in dem $du = -3dx$ zu neutralisieren.
- Integration von rationalen Funktionen: Um rationale Funktionen, also der Quotient zweier Polynome $p,q$ $\frac p q$ kann durch Polynomendivision auf folgende Form gebracht werden, falls der Grad von p grösser ist als der von q, ansonsten kann dieser Schritt übersprungen werden: $p_1 + \frac{p_2}{q}$, bei dem der Grad von $p_2$ kleiner ist als der von q. 
	- Das Ziel ist es nun diesen Bruch separat zu integrieren, denn das integrieren von $p_1$ ist trivial. Die Strategie um die Stammfunktion dieser rationalen Funktion zu finden ist es, sie in Brüche mit einfachen Nennern zu bringen und diese dann in eine der drei folgenden Formen zu bringen:
		- $\int \frac{du}{u} = \ln|u|$
		- $\int\frac{du}{u^n} = \frac{-1}{(n-1)u^{n-1}}$$\forall n \in \mathbb N_{>1}$ 
		- $\int \frac{du}{u^2+c^2} = \frac1carctan(\frac uc)$ 
	- Um diese rationalen Funktionen in die richtige Form zu bringen, gibt es einige Strategien:
		- Manchmal reicht es einfach das Polynom im Nenner zu einer Potenz zusammenzufassen und es passt für die zweite Form.
		- Manchmal kann das Polynom im Nenner in eine quadratische Potenz plus einen konstanten Ausdruck zu bringen. Das reicht dann für die dritte Form.
		- Bei komplexeren Polynomen kann die Funktion durch Partialbruchzerlegung aufgeteilt werden. Dafür wird eine Summe von Brüchen mit den Nullstellen im Nenner und einer Konstante im Zähler definiert. Danach können diese Konstanten berechnet werden und vor das Integral geholt werden.
- Uneigentliche Integrale: Manche Integrale können trotz ihrer Grenzen im Unendlichen einen endlichen Wert haben. Diese Werte nennt man uneigentliche Integrale. Ein Beispiel für ein unegeintliches Integral ist $\int_0^\infty e^{-x} dx = \lim_{t\to\infty} \int_0^t e^{-x}dx =  \lim_{t\to\infty} (1-e^-x)\biggr|_0^t = 1$ 

**Woche 10**
- Lineare Algebra: Das Feld der Mathematik der linearen Algebra beschäftigt sich mit dem Lösen linearer Gleichungssystemen, die überall vorkommen. Ein Lineares Gleichungssystem ist eine Menge linearer Gleichungen mit einen oder mehr Unbekannten, die alle gleichzeitig erfüllt sein sollen.
	- Matrixen: Um lineare Gleichungssysteme einfach darzustellen, schreibt man sie in eine Matrix. Eine Matrix der Form $n\times m$ hat n Zeilen und m Spalten. Um ein lineares Gleichungssystem in eine Matrix zu schreiben, werden die Unbekannten jedes Gleichungssystems auf eine Seite und die Konstanten auf die andere Seite des gleichs verschoben. Dann wird für eine Matrix, die Koeffizientenmatrix A , der Form $n\times m$, wobei n die Anzahl der Gleichungen und m die Anzahl der Unbekannten ist. Jeder Spalte wird also einer Unbekannten zugeteilt und der Koeffizient jeder Unbekannten auf jeder Zeile wird entsprechend eingetragen. Die Konstanten werden in einer Matrix der Form $n\times1$, dem Ergebnisvektor B, eingetragen. Zum Beispiel: $\begin{aligned}x+2y = 3\\ 	3x + 4z = 0 \\	6y + 8z + 3x = 6 \end{aligned}$ wird zur Koeffizientenmatrix A $\begin{pmatrix}1&2&0\\3&0&4\\3&6&8\end{pmatrix}$ und zum Ergebnisvektor B $\begin{pmatrix}3\\0\\6\end{pmatrix}$. 
	- Multiplizieren von Matrixen mit Vektoren: Eine Matrix der Form $n\times m$ kann mit einem Vektor der From $m\times1$ multpliziert werden. Dafür wird alle Elemente der ersten Spalte mit dem ersten Element, alle der zweiten Spalte mit dem zweiten Element, etc. Zum Beispiel: $\begin{pmatrix}a_{11}& a_{12} & ... & a_{1m} \\a_{21}& a_{22} & ... & a_{2m} \\ ...&...&...&...\\a_{n1}& a_{n2} & ... & a_{nm} \end{pmatrix}\times \begin{pmatrix}x_1\\x_2\\...\\x_m\end{pmatrix} = \begin{pmatrix}a_{11}\cdot x_1+ a_{12}\cdot x_2 + ... + a_{1m} \cdot x_m\\a_{21}\cdot x_1+ a_{22}\cdot x_2 + ... + a_{2m}\cdot x_m \\ ...+...+...+...\\a_{n1}\cdot x_1+ a_{n2} \cdot x_2+ ... + a_{nm} \cdot x_m\end{pmatrix}$ 
	Das heisst ein lineares Gleichungssystem kann kurz so geschrieben werden: $A\times\begin{pmatrix}x_1\\x_2\\...\\x_m\end{pmatrix} = B$
	- Eine Lösungsmenge eines solchen linearen Gleichungssystems kann also als die Menge aller Spaltenvektoren sein, die diese Bedingung erfüllen: $\mathbb L = \left\{ v = \begin{pmatrix}x_1\\x_2\\...\\x_m\end{pmatrix} \in \mathbb K^n \Biggr| A\cdot v = B \right\}$ 
	- Um eine solche Lösung zu finden wendet man oft das Gaussche Eliminationsverfahren an. Dafür muss man zuerst die erweiterte Matrix der Koeffizientenmatrix und dem Ergebnisvektor bilden. Die erweiterte Matrix einer Koeffizientenmatrix $\begin{pmatrix}a_{11}& a_{12} & ... & a_{1m} \\a_{21}& a_{22} & ... & a_{2m} \\ ...&...&...&...\\a_{n1}& a_{n2} & ... & a_{nm} \end{pmatrix}$ und einem Ergebnisvektor $\begin{pmatrix}b_1\\b_2\\...\\b_n\end{pmatrix}$ ist $\left(\begin{array}{cccc|c}a_{11}& a_{12} & ... & a_{1m} &b_1\\a_{21}& a_{22} & ... & a_{2m} &b_2 \\ ...&...&...&...&...\\a_{n1}& a_{n2} & ... & a_{nm} &b_n\end{array}\right)$. Diese Matrix soll nun durch elementare Umformungen auf der linken Seite auf Zeilenstufenform gebracht werden. Eine Matrix der Form $n\times m$ ist in ihrer Zeilenstufen wenn die ersten $m$ Zeilen an ihrerem $i$-ten Eintrag eine 1 haben und der Rest alles Nullen sind. Mit elementaren Umformungen sind das Vertauschen von Zeilen, das addieren von Zeilen mit einem Vielfachen anderer Zeilen, sowie das multiplizieren von Zeilen mit einem Koeffizient $>0$ gemeint. Es lässt sich beweisen, dass sich jede beliebige Matrix durch diese Umformungen auf Zeilenstufenform bringen lässt.
	- Hat ein Gleichungssystem also mit n Gleichungen n Unbekannte, so hat es eine eindeutige Lösung, denn der Rang der Koeffizientmatrix ist n. Der Rang einer Matrix gibt an, wie viele Zeilen ausgenommen Nullzeilen eine Matrix hat. Eine Koeffzientenatrix mit Rang r hat also $n-r$ beliebig wählbare Parameter.

**Woche 11**
- Rechnen mit Matrixen: Mit Matrixen kann durch die Definiton einer Matrixaddition, einer Skalarmultiplikation und einer Matrixmultiplikation gerechnet werden.
	- Matrixadition: $\begin{pmatrix}a_{11}& a_{12} & ... & a_{1m} \\a_{21}& a_{22} & ... & a_{2m} \\ ...&...&...&...\\a_{n1}& a_{n2} & ... & a_{nm} \end{pmatrix} +\begin{pmatrix}b_{11}& b_{12} & ... & b_{1m} \\b_{21}& b_{22} & ... & b_{2m} \\ ...&...&...&...\\b_{n1}& b_{n2} & ... & b_{nm} \end{pmatrix} = \begin{pmatrix}a_{11}+b_{11}& a_{12}+b_{12} & ... & a_{1m}+b_{1m} \\a_{21}+b_{21}& a_{22}+b_{22} & ... & a_{2m}+b_{2m} \\ ...&...&...&...\\a_{n1}+b_{n1}& a_{n2}+b_{n2} & ... & a_{nm}+b_{nm}\end{pmatrix}$
	- Skalarmultiplikation: $\lambda\cdot \begin{pmatrix}a_{11}& a_{12} & ... & a_{1m} \\a_{21}& a_{22} & ... & a_{2m} \\ ...&...&...&...\\a_{n1}& a_{n2} & ... & a_{nm} \end{pmatrix}=\begin{pmatrix}\lambda a_{11}&\lambda a_{12} & ... &\lambda a_{1m} \\\lambda a_{21}&\lambda a_{22} & ... &\lambda a_{2m} \\ ...&...&...&...\\\lambda a_{n1}&\lambda a_{n2} & ... &\lambda a_{nm} \end{pmatrix}$ 
	- Die Multiplikation zweier Matrixen ist etwas komplizierter: Die Formen der beiden Matrixen muss stimmen. Eine Matrix A der Form $n\times s$ kann nur mit einer Matrix B der Form $s\times m$ multipliziert werden und produziert eine Matrix C der Form $n\times m$. Denn um den Eintrag $c_{ij}$ von C auszurechnen,  muss man die gewichtete Summe der i-ten Zeile von A mit den Gewichten der j-ten Spalte von B berechnen.
- Die Einheitsmatrix: Die n-te Einheitsmatrix E ist eine Matrix der Form $n\times n$ mit nur Einsen auf der Diagonale. Daraus folgt die Eigenschaft, dass $EA = AE = A$
- Inverse: Das Inverse B einer Matrix A hat die Eigenschaft, dass $BA = AB = E$. Eine Matrix kann nur ein Inverses besitzen, falls sie vollen Rang hat (also Rang n bei einer Form $n\times n$). Das Inverse einer Matrix A der Form $n\times n$ ist $\frac1{ad-bc}\begin{pmatrix}d &-b\\-c&a\end{pmatrix}$. Um das Inverse einer Matrix A der Form $n\times n$ zu berechnen muss man die erweiterte Matrix der Matrix A und der n-ten Einheitsmatrixen $(A|E)$ bilden und die linke Seite auf Zeilenstufenform bringen. Auf der rechten Seite ist dann das Inverse B von A.
- Determinante: Die Determinante einer Matrix A ist eine Zahl die verschiedene Eigenschaften über die Matrix liefert, zum Beispiel ob diese invertierbar ist oder nicht.
	- Für $2\times 2$-Matrixen $\begin{pmatrix} a &b \\c&d\end{pmatrix}$ ist die Determinante $ad - bc$.
	- Für $n\times n$-Matrixen kann die Determinante mithilfe von mehreren $2\times 2$-Matrixen berechnet werden. Dafür wählt man sich eine Zeile/Spalte aus und nimmt die gewichtete Summe der Determinanten der Matrixen die entstehen, wenn man die Spalte und Zeile jedes Eintrags der ausgewählten Spalte verdeckt, mit dem Gewicht des jeweiligen Eintrags, mit dem Vorzeichen nach dem folgenden Schema $\left[\begin{array}{cccc}+&-&+&-&...\\-&+&-&+&...\\+&-&+&-&...\\-&+&-&+&...\\...&...&...&...&...\end{array}\right]$. 
	- Die Determinante der Einheitsmatrix E $det(E) = 1$
	- Eine Matrix A der Form $n\times n$ mit der Determinante $det(A) \neq 0$ hat den Rang $r = n$ und ein Inverses $A^{-1} = B$ 

**Woche 12**
- Geometrische Bedeutung der Determinante: Die Determinante kann man als den Flächeninhalt/das Volumen des durch die Spaltenvektoren aufgespannten Parallelogram, bzw. Spatens interpretiert werden. Dabei ist das Vorzeichen von der Orientierung des Körpers abhängig. Ist die Determinante mehrerer solcher Vektoren 0, so sind die Vektoren linear abhängig voneinander.
	- Vorzeichen der Determinante: Ist der Winkel $\alpha$ zwischen den zwei Vektoren auf der Ebene $0<\alpha<\pi$, so ist das Vorzeichen positiv. Gilt $0>\alpha>-\pi$, so ist das Vorzeichen negativ. Im Dreidimensionalen Raum muss der Spaten der 3-Finger-Regel, dann ist er positiv, sonst ist es negativ.
	- Skalarprodukt: Das Skalarprodukt zweier Vektoren $v = \begin{pmatrix}x_1\\ y_1\\z_1\end{pmatrix}, w= \begin{pmatrix}x_2\\ y_2\\z_2\end{pmatrix}$ $\langle v,w\rangle = x_1x_2 + y_1y_2 + z_1z_2$.
	- Vektorprodukt: Das Vektorprodukt zweier Vektoren $v = \begin{pmatrix}x_1\\ y_1\\z_1\end{pmatrix}, w= \begin{pmatrix}x_2\\ y_2\\z_2\end{pmatrix}$ $v\times w = \left|\begin{array}{}x_1& x_2& e_1\\y_1& y_2& e_2\\z_1& z_2& e_3\\\end{array}\right| = \begin{pmatrix}y_1z_2-y_2z_1\\ x_1z_2-z_1x_2\\x_1y_2-y_1x_2\end{pmatrix}$.
	- Die Determinante dreier Vektoren entspricht dem Skalarprodukt der zwei ersten miteinander multiplizierten Vektoren und dem dritten Vektor. $det(v,w,z) = \langle u\times v, z\rangle$ 
- Vektorräume: Ein Vektorraum ist eine Menge aus Vektoren für die Multiplikation und Addition definiert wird. Vektoren können durch Pfeile repräsentiert werden. Ein linearer Unterraum ist eine Untermenge eines Vektorraums, was selber auch ein Vektorraums ist.
$a_n = \frac{n^2+1}{n+3}$