# Aufgabenblatt 12
**Aufgabe 1**
$A= \left(\begin{array}{cc}
7&-4 \\
-5&3\\
0 &0
\end{array} \right)$

$B= \left(\begin{array}{ccc}
3&4&-1\\
5&7&0\\
\end{array} \right)$

a) 
$AB=\left(\begin{array}{ccc}
21 -20 &28-28&-7\\
-15+15&-20+21 &5\\
0&0&0
\end{array} \right)$Typ $3\times3$

$BA =\left(\begin{array}{cc}
21 -20 &-12+12\\
35-35&-20+21\\
\end{array} \right) = E$ Typ $2\times2$

$\left(\begin{array}{ccc}
1 &0&-7\\
0&1 &5\\
0&0&0
\end{array} \right)\neq\left(\begin{array}{cc}
1 &0\\
0&1\\
\end{array} \right)$
Schon vom Typ her nicht gleich.

b) 
$AC =\left(\begin{array}{cc}
7&-4 \\
-5&3\\
0 &0
\end{array} \right)\times \left(\begin{array}{ccc}
a&b&c \\
d&e&f\\
\end{array} \right)=\left(\begin{array}{ccc}
1&0 &0\\
0&1&0\\
0&0&1
\end{array} \right)$
Dafür (für das Feld $E_{2_2}$) muss folgendes gelten:
$0c + 0f =1$ Widerspruch

---
**Aufgabe 2**
$A=\left(\begin{array}{cc}2&5\\4&8\end{array}\right)$ 
$\frac1{ad-bc} = \frac{1}{16-20} = \frac1{-4}$
$A^{-1} =\left(\begin{array}{cc}-2&1.25\\1&-0.5\end{array}\right)$
$A^{-1}A \stackrel{?}{=} \left(\begin{array}{cc}-4+5&-10+10\\4-4&5-4\end{array}\right) =\left(\begin{array}{cc}
1 &0\\
0&1\\
\end{array} \right)$ ✅
$A\left(\begin{array}{cc}
x\\
y\\
\end{array} \right) = \left(\begin{array}{cc}
4\\
8\\
\end{array} \right)$   | mal $A^{-1}$ von links
$\left(\begin{array}{cc}
x\\
y\\
\end{array} \right) =\left(\begin{array}{cc}-2&1.25\\1&-0.5\end{array}\right) \left(\begin{array}{cc}
4\\
8\\
\end{array} \right) = \left(\begin{array}{cc}-8+10\\4-4\end{array}\right)= \left(\begin{array}{cc}2\\0\end{array}\right)$

$B= \left(\begin{array}{ccc}1&0&-2\\7&4&3\\6&3&1\end{array}\right)$
$\left(\begin{array}{c|c}B&E\end{array}\right)= \left(\begin{array}{ccc|ccc}1&0&-2&1&0&0\\7&4&3&0&1&0\\6&3&1&0&0&1\end{array}\right)\stackrel{\longrightarrow}{\text{II-7I}}\left(\begin{array}{ccc|ccc}1&0&-2&1&0&0\\0&4&17&-7&1&0\\6&3&1&0&0&1\end{array}\right)\stackrel{\longrightarrow}{\text{II/4 und III-6I}}\left(\begin{array}{ccc|ccc}1&0&-2&1&0&0\\0&1&4.25&-1.75&0.25&0\\0&3&13&-6&0&1\end{array}\right)$$\stackrel{\longrightarrow}{\text{II-3II und III*4}}\left(\begin{array}{ccc|ccc}1&0&-2&1&0&0\\0&1&4.25&-1.75&0.25&0\\0&0&1&-3&-3&4\end{array}\right)\stackrel{\longrightarrow}{\text{II-4.25III}}\left(\begin{array}{ccc|ccc}1&0&-2&1&0&0\\0&1&0&11&13&-17\\0&0&1&-3&-3&4\end{array}\right)$$\stackrel{\longrightarrow}{\text{I+2III}}\left(\begin{array}{ccc|ccc}1&0&0&-5&-6&8\\0&1&0&11&13&-17\\0&0&1&-3&-3&4\end{array}\right)$

$B^{-1} = \left(\begin{array}{ccc|ccc}-5&-6&8\\11&13&-17\\-3&-3&4\end{array}\right)$
$B^{-1}B =\left(\begin{array}{ccc}1&0&-2\\7&4&3\\6&3&1\end{array}\right)\left(\begin{array}{ccc|ccc}-5&-6&8\\11&13&-17\\-3&-3&4\end{array}\right) = \left(\begin{array}{ccc}1&0&0\\0&1&0\\0&0&1\end{array}\right)$
$B\left(\begin{array}{c}x\\y\\z\end{array}\right) =\left(\begin{array}{c}2\\3\\-1\end{array}\right)$ | mal $B^{-1}$ von links
$\left(\begin{array}{c}x\\y\\z\end{array}\right) =\left(\begin{array}{ccc|ccc}-5&-6&8\\11&13&-17\\-3&-3&4\end{array}\right)\left(\begin{array}{c}2\\3\\-1\end{array}\right)=\left(\begin{array}{c}-10-18-8\\22+39+17\\-6-9-4\end{array}\right) = \left(\begin{array}{c}-36\\78\\-19\end{array}\right)$
---
**Aufgabe 3**
a) $\left|\begin{array}{}0&-\sqrt6&0\\\sqrt2&10&0\\-1&5\pi&\sqrt3\end{array}\right| =-\sqrt2\left|\begin{array}{}-\sqrt6&0\\5\pi&\sqrt3\end{array}\right|-\left|\begin{array}{}-\sqrt6&0\\10&0\end{array}\right| = -\sqrt2(-3\sqrt2 )=6$
b) 
$\left|\begin{array}{}1&4&0&3\\2&0&7&-1\\3&0&-2&-1\\0&6&1&-4\end{array}\right|\stackrel{=}{\text{2. Spalte entwicheln}}-4\left|\begin{array}{}2&7&-1\\3&-2&1\\0&1&-4\end{array}\right|+6\left|\begin{array}{}1&0&3\\2&7&-1\\3&-2&1\\\end{array}\right| = -4(-1(2+3)-4(21+4))+6(1(7-2)+3(-4-21))=-4(-105)+6(-70) = 0$

c) $\left|\begin{array}{}2&7&0&3\\0&2&0&0\\6&-3&4&0\\1&5&-1&1\end{array}\right|\stackrel{=}{\text{der 4. Spalte entwickeln}}-3\left|\begin{array}{}0&2&0\\6&-3&4\\1&5&-1\end{array}\right|+\left|\begin{array}{}2&7&0\\0&2&0\\6&-3&4\\\end{array}\right| =-3(-2(4+6))+(2(8)) = 60+16 = 76$
