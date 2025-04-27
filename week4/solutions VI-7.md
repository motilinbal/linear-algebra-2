# Page 0

# אלגברה לינארית 

## סמסטר ב' תשפ"ה

## שאלה VI.7.1

א. אם ,$W=\operatorname{span}\left\{w_{1}, \ldots, w_{m}\right\}$ ו $U=\operatorname{span}\left\{u_{1}, \ldots, u_{k}\right\}$
$U+W=\operatorname{span}\left\{u_{1}, \ldots, u_{k}, w_{1}, \ldots, w_{m}\right\}$.
כדי למצא מימד של $U+W$ נבנה בסיס לתת מרחב הזה. לשם כך נסדר את
הוקטורים הפורשים כשורות במטריצה ונדרג:

$$
\begin{aligned}
& \cdot \operatorname{dim}(U+W)=3
\end{aligned}
$$

ב. נמצא את המימדים של $U \cap W$ ונחשב את המימד של $U \cap W$ בעזרת הנוסחה

$$
\operatorname{dim}(U+W)=\operatorname{dim}(U)+\operatorname{dim}(W)-\operatorname{dim}(U \cap W)
$$

לשם כך נמצא בסיס ב- $U$ : נסדר את הוקטורים הפורשים את $U$ כשורות במטריצה ונמצא את דרגתה. נקבל

$$
\left(\begin{array}{cccc}
1 & -1 & 1 & -1 \\
1 & 1 & 1 & 1 \\
1 & 3 & 1 & 3
\end{array}\right) \sim \ldots \sim\left(\begin{array}{llll}
1 & 0 & 1 & 0 \\
0 & 1 & 0 & 1 \\
0 & 0 & 0 & 0
\end{array}\right)
$$

# Page 1

השורות השונות מאפס מהוות בסיס ב־ $U$ ולפיכך $\operatorname{dim}(U)=2$. באופן דומה, נמצא בסיס ב־ $W$ ע״י דירוג של המטריצה המתאימה:

$$
\begin{aligned}
& \left(\begin{array}{llll}
3 & 1 & 3 & 1 \\
1 & 2 & 1 & 2 \\
1 & 2 & 0 & 2
\end{array}\right) \sim \ldots \sim\left(\begin{array}{llll}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 1 \\
0 & 0 & 1 & 0
\end{array}\right) \\
& \operatorname{dim}(W)=3
\end{aligned}
$$

ולכן $\operatorname{dim}(U \cap W)=2+3-3=2$.
ג. לפי הדירוג בסעיף (א) הקבוצה

$$
\left\{\left.\left(\begin{array}{l}
1 \\
0 \\
0 \\
0
\end{array}\right),\left(\begin{array}{l}
0 \\
1 \\
0 \\
1
\end{array}\right),\left(\begin{array}{l}
0 \\
0 \\
1 \\
0
\end{array}\right)\right\}
$$

מהווה בסיס בתת מרחב $U+W$.
ד. נסביר את שיטה למציאת בסיס בחיתוך של שני תתי מרחבים. $v \in U \cap W$ אם $v \in U \cap W$ אם ורק אם קיימים קבועים

$$
v=\sum_{i=1}^{k} c_{i} u_{i}=\sum_{j=1}^{m} d_{j} w_{j}
$$

כאשר $\left\{w_{1}, \ldots, w_{m}\right\} \quad U \cap U \cap W$ נמצא בסיס לקבוצת הפתרונות של ממ״ל הומוגנית

$$
\sum_{i=1}^{k} c_{i} u_{i}-\sum_{j=1}^{m} d_{j} w_{j}=0
$$

נסמן את וקטורי הבסיס שהתקבלו ב $\mathbb{R}^{k+m} \supset\left\{x_{1}, \ldots, x_{\ell}\right\}$ וב־ $x_{i j}$ את הרכיב $\mathbb{R}^{k+m} \supset\left\{x_{1}, \ldots, x_{\ell}\right\}$ וב־ $y_{j}$ את הרכיב
$\mathrm{c}^{-} j$ של הוקטור $x_{i}$. לפי הבניה הזו הוקטורים

$$
v_{i}=\sum_{j=1}^{k} x_{i j} u_{j}=\sum_{j=1}^{m} x_{i, k+j} w_{j}, \quad i=1, \ldots, \ell
$$

# Page 2

פורשים את . לכן בסיס של $\operatorname{span}\left\{v_{1}, \ldots, v_{\ell}\right\}$ הוא גם בסיס ב $U \cap W$ ואותו אפשר למצוא בכלים הרגילים (למשל לסדר $v_{i}$ כשורות במטריצה ולמצא את דרגתה).
הצעד האחרון מיותר אם . מצעד $U$ ל. משתף פעולה. נוכיח כי במקרה הזה $\left\{v_{1}, \ldots, v_{\ell}\right\}$ אכן בת"ל. לשם כך נניח $\alpha_{1}, \ldots, \alpha_{\ell}$ קבועים עבורם

$$
\sum_{i=1}^{\ell} \alpha_{i} v_{i}=0
$$

ונראה 0 . נציב ונקבל . $\alpha_{1}=\ldots=\alpha_{\ell}=0$

אם $\left\{u_{1}, \ldots, u_{k}\right\}$ בת"ל אז

באופן דומה

ולכן

לפי (2) ו (3)

ולכן $\alpha_{1}=\ldots=\alpha_{\ell}=0$
נפעיל את האלגוריתם על הנתונים של השאלה. נדרג מטריצת המקדמים המתאימה לממ"ל (1)

$$
\left(\begin{array}{cccccc}
1 & 1 & 1 & -3 & -1 & -1 \\
-1 & 1 & 3 & -1 & -2 & -2 \\
1 & 1 & 1 & -3 & -1 & 0 \\
-1 & 1 & 3 & -1 & -2 & -2
\end{array}\right) \sim \ldots \sim\left(\begin{array}{cccccc}
1 & 0 & -1 & -1 & \frac{1}{2} & 0 \\
0 & 1 & 2 & -2 & -\frac{3}{2} & 0 \\
0 & 0 & 0 & 0 & 0 & 1 \\
0 & 0 & 0 & 0 & 0 & 0
\end{array}\right)
$$

# Page 3

לפיכך בסיס בקבוצת הפתרונות הוא

$$
x_{1}=\left(\begin{array}{r}
1 \\
-2 \\
1 \\
0 \\
0 \\
0
\end{array}\right), \quad x_{2}=\left(\begin{array}{l}
1 \\
2 \\
0 \\
1 \\
0 \\
0
\end{array}\right), \quad x_{3}=\left(\begin{array}{r}
-1 \\
3 \\
0 \\
0 \\
2 \\
0
\end{array}\right)
$$

ולכן הוקטורים

$$
v_{1}=\sum_{i=1}^{3} x_{1 i} u_{i}=\left(\begin{array}{l}
0 \\
0 \\
0 \\
0
\end{array}\right), v_{2}=\sum_{i=1}^{3} x_{2 i} u_{i}=\left(\begin{array}{l}
3 \\
1 \\
1 \\
3 \\
1
\end{array}\right), v_{3}=\sum_{i=1}^{3} x_{3 i} u_{i}=\left(\begin{array}{l}
2 \\
4 \\
2 \\
4
\end{array}\right)
$$

פורשים את $U \cap W$. שני הוקטורים השונים מ־0 אינם מקביליים ולכן בת"ל. קיבלנו כי הקבוצה

$$
\left\{\left(\begin{array}{l}
3 \\
1 \\
3 \\
1
\end{array}\right),\left(\begin{array}{l}
1 \\
2 \\
1 \\
2
\end{array}\right)\right\}
$$

הינה בסיס ב $U \cap W$.
הערה: בנתוני השאלה אפשר להגיע לתשובה באופן מידי. ראינו כי $\operatorname{dim}(U)=2$ וגם $U \cap W=2$. אך $U \cap W$ תת מרחב של $U$ ולכן $U=U \cap W$, כלומר בסיס ב $U$ הוא גם בסיס ב $U \cap W$. האלגוריתם הנ"ל מאפשר לפתור שאלות מהסוג הזה באופן כללי.

# שאלה VI.7.2 

א. מתקיים $S=S+\{0\} \subseteq S+S$. נותר להוכיח הכלה בכיוון השני. אם $v \in S+S$ אזי $u+w \in S$ כאשר $v=u+w$ וגם $u \in S$. משום ש $S$ תת מרחב, ולכן $S+S \subseteq S$. קיבלנו

$$
S=S+S \text {. } \quad \text {. } \quad \text { אינה תת מרחב, אך } S+S=S
$$

# Page 4

נגדיר תתי מרחבים

$$
W=\left\{x \in \mathbb{R}^{n}: x_{1}+\ldots+x_{n}=0\right\}, \quad U=\left\{x \in \mathbb{R}^{n}: x_{1}=\ldots=x_{n}\right\}
$$

הוקטור

$$
u_{1}=\left(\begin{array}{l}
1 \\
\vdots \\
1
\end{array}\right)
$$

$n-1$ בסיס במרחב $U$ (כי כל וקטור ב־ $U$ הינו כפולה של , $u_{1}$. הקבוצה של 1 וקטורים

בסיס ב־ $W$ (לממ״ל $n-1$ יש משתנים חופשיים, כלומר $W=1-0$ והקבוצה הנ״ל בת״ל ). הקבוצה $U+W=\mathbb{R}^{n}$ בת שלושה מִתאימה) ולכן בסיס ב־״ $\mathbb{R}^{n}$ (כי המימד של $n \mathbb{R}^{n}$ שווה ל־ $n$ ). מכאן נובע כי $W=$ אם

$$
\lim (U \cap W)=\operatorname{dim}(U+W)-\operatorname{dim}(W)-\operatorname{dim}(U)=n-(n-1)-1=0
$$

לכן

שאלה VI.7.4
א. הקבוצה

$$
\left\{u_{1}, u_{2}\right\}=\left\{\left(\begin{array}{r}
-1 \\
1 \\
0
\end{array}\right),\left(\begin{array}{r}
-1 \\
0 \\
1
\end{array}\right)\right\}
$$

בסיס ב־ $U$ (מרחב הפתרונות של הממ״ל $a+b+c=0$. הקבוצה

$$
\left\{v_{1}, v_{2}\right\}=\left\{\left(\begin{array}{l}
1 \\
0 \\
1
\end{array}\right),\left(\begin{array}{l}
0 \\
1 \\
0
\end{array}\right)\right\}
$$

# Page 5

בסיס ב־V (מרחב הפתרונות של הממ״ל ( $a-c=0$. מתקיים

$$
U+V=\operatorname{span}\left(\left\{u_{1}, u_{2}, v_{1}, v_{2}\right\}\right)
$$

משום ש $U+V \subseteq \mathbb{R}^{3}$, כדי להוכיח $U+V=\mathbb{R}^{3}$, מספיק להראות כי $\operatorname{dim}(U+V)=3$. לשם כך נסדר את הוקטורים כשורות במטריצה ונמצא את דרגתה:

$$
\left(\begin{array}{ccc}
-1 & 1 & 0 \\
-1 & 0 & 1 \\
1 & 0 & 1 \\
0 & 1 & 0
\end{array}\right) \sim \ldots \sim\left(\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0
\end{array}\right)
$$

דרגת המטריצה שווה ל־3 ולכן ומכאן

$$
U+W=\mathbb{R}^{3}
$$

הסכום הזה אינו ישר כי

$$
\operatorname{dim}(U \cap W)=\operatorname{dim}(U)+\operatorname{dim}(V)-\operatorname{dim}(U+V)=1
$$

ב. הקבוצה

$$
\left\{w_{1}\right\}=\left\{\left.\left(\begin{array}{l}
0 \\
0 \\
1
\end{array}\right)\right\}
$$

בסיס ב־V ו $\operatorname{dim}(U+W)=\operatorname{span}\left(\left\{u_{1}, u_{2}, w_{1}\right\}\right) \backslash W=\operatorname{span}\left(\left\{u_{1}, u_{2}, w_{1}\right\}\right)$
$\operatorname{div} \operatorname{div} W=\operatorname{span}\left(\left\{u_{1}, u_{2}, w_{1}\right\}\right) \backslash W=\operatorname{dim}(U+W)=3$

$$
\left(\begin{array}{ccc}
-1 & 1 & 0 \\
-1 & 0 & 1 \\
0 & 0 & 1
\end{array}\right) \sim \ldots \sim\left(\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right)
$$

דרגת המטריצה שווה ל־3 ולכן הוקטורים בת״ל ו $U+V=\mathbb{R}^{3}$. הסכום הינו ישר כי

$$
\operatorname{dim}(U \cap W)=\operatorname{dim}(U)+\operatorname{dim}(V)-\operatorname{dim}(U+V)=0
$$

# Page 6

$$
\begin{aligned}
& V+W=\operatorname{span}\left(\left\{v_{1}, v_{2}, w_{1}\right\}\right) \\
& \left\{v_{1}, v_{2}, w_{1}\right\}=\left\{\left.\left(\begin{array}{l}
1 \\
0 \\
1
\end{array}\right),\left(\begin{array}{l}
0 \\
1 \\
0
\end{array}\right),\left(\begin{array}{l}
0 \\
0 \\
1
\end{array}\right)\right\}
\end{aligned}
$$

בת"ל ולכן $U+V=\mathbb{R}^{3} \backslash \operatorname{dim}(U+V)=3$
$\operatorname{dim}(U \cap W)=\operatorname{dim}(U)+\operatorname{dim}(V)-\operatorname{dim}(U+V)=0$.

# שאלה VI.7.5 

נסדר את הוקטורים כשורות במטריצה ונדרג:

$$
\left(\begin{array}{lll}
1 & 0 & 1 \\
3 & 2 & 1 \\
1 & 2 & 3 \\
2 & 2 & 3
\end{array}\right) \sim \cdots \sim\left(\begin{array}{lll}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1 \\
0 & 0 & 0
\end{array}\right)
$$

לכן $\operatorname{dim}(U+V)=\operatorname{dim}\left(\operatorname{span}\left(u_{1}, u_{2}, u_{3}, u_{4}\right\}\right)=3$ משפט המימדים

$$
\operatorname{dim}(U \cap V)=2+2-3=1>0
$$

ולכן הסכום לא ישר.

## שאלה VI.7.6

הטענה אינה נכונה. כדוגמה נגדית אפשר לקחת, למשל, $U=W=V$. במקרה הזה, $U \cap W \neq\{0\}$ וגם $V=U+W$ אם $V=U \cup W$ . $U \cap W \neq\{0\}$ באופן כללי יותר, מתקיימת טענה הבאה: אם $V$ מרחב וקטורי ו $V=U \cup W$ עבור תת מרחבים $U, W \subseteq V$ או $U, W \subseteq V$. נוכיח בשלילה: נניח קיימים וקטורים $w \in W, w \notin U \quad u \in U, u \notin W$ ונגיע לסתירה. מתקיים $V, w \in W \subseteq U \cup W=V$ וגם $V, w \in W \subseteq U \cup W=V$ מרחב וקטורי, $U$ ו- $w \in U$ או $w \in U$ ו- $w \in U$ מרחב, $w \in U$ וזאת סתירה. באופן דומה, אם $w \in W$ או $w \in W$ וגם זאת סתירה.

# Page 7

שאלה VI.7.7

נגדיר תת מרחבים (מעל שדה של ממשיים)

$$
H:=\left\{A \in \mathbb{C}^{n \times n}: A=A^{\dagger}\right\}, \quad G:=\left\{A \in \mathbb{C}^{n \times n}: A=-A^{\dagger}\right\}
$$

כל מטריצה $B \in \mathbb{C}^{n \times n}$ ניתנת לפירוק:

$$
B=\underbrace{\frac{1}{2}\left(B+B^{\dagger}\right)}_{\in H}+\underbrace{\frac{1}{2}\left(B-B^{\dagger}\right)}_{\in G}
$$

ולכן $A=-A ו A^{\dagger}=A$ או $A \in H \cap G$ ו $B \in H \cap G$ . $H+G=\mathbb{C}^{n \times n}$. מכאן $B=0$ ולכן $H \cap G=\{0\}$. קיבלנו $\{0\}$. $A=0$

שאלה VI.7.8

יהיה $C$ מרחב וקטורי של פונקציות $f: \mathbb{R} \mapsto \mathbb{R}$ רציפות ונגדיר קבוצת כל הפונקציות הזוגיות ב־ $C$ :

$$
A=\{f \in C: f(x)=f(-x), \forall x \in \mathbb{R}\}
$$

והפונקציות האי־זוגיות ב־ $C$ :

$$
B=\{f \in C: f(x)=-f(-x), \forall x \in \mathbb{R}\}
$$

א. נראה כי $A$ סגורה תחת חיבור וכפל בסקלר ולכן תת מרחב. עבור $f, g \in A$
$(f+g)(x)=f(x)+g(x)=f(-x)+g(-x)=(f+g)(-x), \quad \forall x \in \mathbb{R}$
כלומר $f+g \in A$. עבור $c \in \mathbb{R}$. עבור $g \in A$
$(c f)(x)=c f(x)=c f(-x)=(c f)(-x) \quad \forall x \in \mathbb{R}$
כלומר $f \in A$. באופן דומה $B$ סגורה תחת חיבור וכפל בסקלר ולכן תת מרחב: עבור $f, g \in B$

$$
\begin{aligned}
(f+g)(x)= & f(x)+g(x)=-f(-x)-g(-x)= \\
& -(f(-x)+g(-x))=-(f+g)(-x), \quad \forall x \in \mathbb{R} \\
& c \in \mathbb{R} . \text { עבור } f+g \in B \\
(c f)(x)= & c f(x)=-c f(-x)=-(c f)(-x), \quad \forall x \in \mathbb{R}
\end{aligned}
$$

ולכן $c f \in B$.

# Page 8

$$
f(x)=-f(-x) \text { עם } f(x)=f(-x) \text { אז } f \in A \cap B
$$

לכן

$$
f(-x)=-f(-x), \quad \forall x \in \mathbb{R} \quad \Longrightarrow \quad 2 f(-x)=0, \quad \forall x \in \mathbb{R}
$$

כלומר $A+B=A \oplus B$ ומכאן $A \cap B=\{0\}$. לכן $\operatorname{cl}_{x \in \mathbb{R}} A \in \mathbb{R}$. לכן $\operatorname{cl}_{x \in \mathbb{R}} A \cap B=\{0\}$.

שאלה VI.7.9

נגדיר $\}$ : $U=\operatorname{span}(T)$ ו $T=\left\{x^{6}, x^{7}, \ldots\right\}$ (כל הפולינומים מדרגה סופית גדולה מ־5). ראינו כי הוקטורים ב־T בת״ל ולכן $T$ בסיס ב־U. הקבוצה $\left\{1, x, \ldots, x^{5}\right\}$ בסיס ב־F. ראינו כי הקבוצה

$$
S=S_{5} \cup T=\left\{1, x, x^{2}, \ldots\right\}
$$

בסיס ב־F. בנוסף $4(\mathrm{~g})$

$$
F[x]=F_{5}[x] \oplus U
$$

כלומר $U$ הוא המשלים של F. $F[x]$ ב $F_{5}[x]$.

שאלה VI.7.9

תהי $C([0,1])$ קבוצת הפונקציות הרציפות מעל $[0,1]$ ל־R. נגדיר תת קבוצה של פונקציות קבועות:

$$
W=\{f \in C([0,1]): f(x)=f(0), \forall x \in[0,1]\}
$$

ותת קבוצה של פונקציות המתאפסות בנקודה נתונה

$$
U=\{f \in C([0,1]): f(c)=0\}
$$

נראה כי

$$
C([0,1])=U+W
$$

עבור כל $(g \in C([0,1])$ נרשום

$$
g(x)=\underbrace{(g(x)-g(c))}_{=u(x)}+\underbrace{g(c)}_{=w(x)} .
$$

# Page 9

הפונקציה $w$ קבועה ולכן $w \in W$. הפונקציה $u$ מתאפסת ב- $c$

$$
u(c)=g(c)-g(c)=0
$$

ולכן $u \in U$. הוכחנו את (4). נותר להראות כי

$$
U \cap W=\{0\}
$$

נניח $h(c)=0$ אז $h \in U \cap W$ וגם

$$
h(x)=h(0), \quad \forall x \in[0,1]
$$

בפרט 0) $h(x)=0, \forall x \in[0,1]$.

$$
C([0,1])=U \oplus W
$$

