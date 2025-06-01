## 1. Предел посл-ти точек в $R^n$. Точки множества. Открытые и замкнутые мн-ва. Внутренность, замыкание, граница.

**Предел последовательности (посл-ти) точек $\{ \mathbf{x}_k \}_{k=1}^\infty \subset R^n$**
Точка $\mathbf{a} \in R^n$ наз. пределом посл-ти $\{\mathbf{x}_k\}$, если $\forall \varepsilon > 0 \ \exists N \in \mathbb{N} \ : \ \forall k > N \implies \|\mathbf{x}_k - \mathbf{a}\| < \varepsilon$. Обозн.: $\lim_{k \to \infty} \mathbf{x}_k = \mathbf{a}$ [1, стр. 185].
Сходимость в $R^n$ эквивалентна покоординатной сходимости [1, стр. 185].

**Точки множества $E \subset R^n$**

* **Точка прикосновения (адгерентная точка)**: $\mathbf{x} \in R^n$ наз. точкой прикосновения мн-ва $E$, если любая ее окрестность $U(\mathbf{x})$ содержит хотя бы одну точку из $E$ ($U(\mathbf{x}) \cap E \neq \emptyset$) [1, стр. 186].
* **Внутренняя точка**: $\mathbf{x} \in E$ наз. внутренней точкой мн-ва $E$, если $\exists U(\mathbf{x}) : U(\mathbf{x}) \subset E$ [1, стр. 185].
* **Предельная точка**: $\mathbf{x} \in R^n$ наз. предельной точкой мн-ва $E$, если любая ее окрестность $U(\mathbf{x})$ содержит хотя бы одну точку из $E$, отличную от $\mathbf{x}$ ($U(\mathbf{x}) \cap (E \setminus \{\mathbf{x}\}) \neq \emptyset$) [1, стр. 186].
* **Изолированная точка**: $\mathbf{x} \in E$ наз. изолированной, если $\exists U(\mathbf{x}) : U(\mathbf{x}) \cap E = \{\mathbf{x}\}$ (т.е. точка мн-ва, не являющаяся предельной для него).

**Открытые и замкнутые множества (мн-ва)**

* **Открытое мн-во**: Мн-во $G \subset R^n$ наз. открытым, если все его точки — внутренние ($G = \text{int } G$) [1, стр. 187].
    * Свойства:

1. $\emptyset$ и $R^n$ — открыты.
2. Объединение любого числа открытых мн-в открыто [1, стр. 189].
3. Пересечение конечного числа открытых мн-в открыто [1, стр. 190].
* **Замкнутое мн-во**: Мн-во $F \subset R^n$ наз. замкнутым, если оно содержит все свои предельные точки ($F' \subset F$, где $F'$ — мн-во предельных точек $F$) [1, стр. 188].
    * Свойства:

1. $\emptyset$ и $R^n$ — замкнуты.
2. Пересечение любого числа замкнутых мн-в замкнуто [1, стр. 190].
3. Объединение конечного числа замкнутых мн-в замкнуто [1, стр. 190].
4. Мн-во $F$ замкнуто $\iff$ его дополнение $R^n \setminus F$ открыто [1, стр. 188].

**Внутренность, замыкание и граница множества $E \subset R^n$**

* **Внутренность (int $E$)**: Мн-во всех внутренних точек $E$. int $E$ — наибольшее открытое мн-во, содержащееся в $E$ [1, стр. 185, 187].
* **Замыкание ($\bar{E}$ или cl $E$)**: Мн-во всех точек прикосновения $E$. $\bar{E} = E \cup E'$. $\bar{E}$ — наименьшее замкнутое мн-во, содержащее $E$ [1, стр. 190-191].
* **Граница (Fr $E$ или $\partial E$)**: Мн-во точек $\mathbf{x} \in R^n$ таких, что любая их окрестность содержит точки как из $E$, так и из $R^n \setminus E$. $\partial E = \bar{E} \setminus \text{int } E = \bar{E} \cap \overline{R^n \setminus E}$ [1, стр. 190].


## 2. Кривые. Т-ма Лагранжа для вектор-ф-ии. Гладкая кривая, касательная, замена параметра. Длина кривой. Натур. параметр. Кривизна.

**Кривая на плоскости и в пространстве**
Кривая (путь) — непрерывное отображение $\mathbf{r}: [a,b] \to R^n$, где $[a,b]$ — отрезок, $\mathbf{r}(t) = (x_1(t), ..., x_n(t))$ [1, стр. 175].

**Теорема Лагранжа о среднем для вектор-функции**
Если $\mathbf{f}: [a,b] \to R^m$ непрерывна на $[a,b]$ и диф-ма на $(a,b)$, то $\|\mathbf{f}(b) - \mathbf{f}(a)\| \le (b-a) \sup_{t \in (a,b)} \|\mathbf{f}'(t)\|$ [1, стр. 176].

* Док-во (идея): Рассмотреть скалярную функцию $\varphi(t) = (\mathbf{f}(b) - \mathbf{f}(a)) \cdot \mathbf{f}(t)$. Применить к ней т. Лагранжа, затем неравенство Коши-Буняковского.

**Гладкая кривая, касательная, допустимая замена параметра**

* **Гладкая кривая**: Кривая $\mathbf{r}(t)$ наз. гладкой, если $\mathbf{r}(t) \in C^1([a,b])$ (т.е. компоненты $x_i(t)$ непрерывно диф-мы) и $\mathbf{r}'(t) \neq \mathbf{0}$ для $\forall t \in (a,b)$ [1, стр. 178].
* **Касательная к гладкой кривой**: В точке $\mathbf{r}(t_0)$ это прямая, проходящая через $\mathbf{r}(t_0)$ с направляющим вектором $\mathbf{r}'(t_0)$ [1, стр. 178]. Уравнение: $\mathbf{R} = \mathbf{r}(t_0) + \tau \mathbf{r}'(t_0)$.
* **Допустимая замена параметра**: $t = \varphi(\tau)$, где $\varphi: [\alpha, \beta] \to [a,b]$ — функция класса $C^1$, $\varphi'(\tau) \neq 0$ для $\forall \tau \in (\alpha, \beta)$. Если $\varphi' > 0$, ориентация сохраняется; если $\varphi' < 0$ — меняется на противоположную [1, стр. 176].

**Длина кривой**
Длина гладкой кривой $\mathbf{r}(t)$, $t \in [a,b]$: $L = \int_a^b \|\mathbf{r}'(t)\| dt = \int_a^b \sqrt{(x_1'(t))^2 + ... + (x_n'(t))^2} dt$ [1, стр. 177].
Длина не зависит от допустимой замены параметра.

**Производная переменной длины дуги. Натуральный параметр.**

* **Переменная длина дуги (функция длины дуги)**: $s(t) = \int_a^t \|\mathbf{r}'(\tau)\| d\tau$ [1, стр. 178].
* **Производная длины дуги по параметру $t$**: $\frac{ds}{dt} = s'(t) = \|\mathbf{r}'(t)\|$ [1, стр. 178].
* **Натуральный параметр $s$**: Параметр кривой, равный длине дуги, отсчитываемой от некоторой фиксированной точки. Для него $\|\mathbf{r}'(s)\| = 1$ [1, стр. 179-180]. Переход: $t \mapsto s(t)$.

**Кривизна кривой**

* **Для натурального параметра $s$**: $k(s) = \|\mathbf{r}''(s)\| = \left\| \frac{d^2\mathbf{r}}{ds^2} \right\|$. Вектор $\mathbf{r}''(s)$ ортогонален $\mathbf{r}'(s)$ [1, стр. 180].
* **Для произвольного параметра $t$ (в $R^3$)**: $k(t) = \frac{\|\mathbf{r}'(t) \times \mathbf{r}''(t)\|}{\|\mathbf{r}'(t)\|^3}$ [1, стр. 181].
* **Для плоской кривой $y=f(x)$**: $k(x) = \frac{|f''(x)|}{(1 + (f'(x))^2)^{3/2}}$.
* **Радиус кривизны**: $R = 1/k$ (если $k \neq 0$) [1, стр. 180].


## 3. Пределы ф-ий мн. переменных. Непрерывность. Связность.

**Пределы функций многих переменных (фмп) (и отображений)**

* **Предел по совокупности переменных**: $\lim_{\mathbf{x} \to \mathbf{x}_0} f(\mathbf{x}) = L$, если $\forall \varepsilon > 0 \ \exists \delta > 0 : \forall \mathbf{x} \in D(f), 0 < \|\mathbf{x} - \mathbf{x}_0\| < \delta \implies \|f(\mathbf{x}) - L\| < \varepsilon$ [1, стр. 197]. (Для отображений $f:R^n \to R^m$).
* **Предел по направлению $\mathbf{v}$ ($\|\mathbf{v}\|=1$)**: $\lim_{t \to 0^+} f(\mathbf{x}_0 + t\mathbf{v})$ [1, стр. 197].
    * Если существует предел по совокупности, то существуют и равны ему пределы по всем направлениям. Обратное неверно [1, стр. 198].
    * Повторные пределы: $\lim_{x_1 \to x_{0,1}} (\lim_{x_2 \to x_{0,2}} ... f(\mathbf{x}) ... )$. Их существование и равенство не гарантируют существование предела по совокупности [1, стр. 199].

**Непрерывность отображения $f: D \subset R^n \to R^m$**

* $f$ непрерывна в $\mathbf{x}_0 \in D$, если $\lim_{\mathbf{x} \to \mathbf{x}_0} f(\mathbf{x}) = f(\mathbf{x}_0)$ [1, стр. 199].
* **Т-ма (непрерывность и открытость прообразов)**: Отображение $f: X \to Y$ непрерывно $\iff$ для любого открытого мн-ва $V \subset Y$ его прообраз $f^{-1}(V) = \{\mathbf{x} \in X : f(\mathbf{x}) \in V\}$ открыт в $X$ [1, стр. 200].
    * Док-во ($\Rightarrow$): Пусть $f$ непр., $V \subset Y$ открыто. Возьмем $\mathbf{x}_0 \in f^{-1}(V)$, т.е. $f(\mathbf{x}_0) \in V$. Т.к. $V$ откр., $\exists \varepsilon > 0: U_\varepsilon(f(\mathbf{x}_0)) \subset V$. Из непр. $f$, $\exists \delta > 0: f(U_\delta(\mathbf{x}_0)) \subset U_\varepsilon(f(\mathbf{x}_0)) \subset V$. Значит $U_\delta(\mathbf{x}_0) \subset f^{-1}(V)$. Т.е. $\mathbf{x}_0$ — внутр. точка $f^{-1}(V)$.
    * Док-во ($\Leftarrow$): Пусть прообраз любого откр. мн-ва открыт. Возьмем $\mathbf{x}_0 \in X$, $f(\mathbf{x}_0) \in Y$. Для $\forall \varepsilon > 0$ окрестность $U_\varepsilon(f(\mathbf{x}_0))$ открыта. Ее прообраз $f^{-1}(U_\varepsilon(f(\mathbf{x}_0)))$ открыт и содержит $\mathbf{x}_0$. Значит $\exists \delta > 0: U_\delta(\mathbf{x}_0) \subset f^{-1}(U_\varepsilon(f(\mathbf{x}_0)))$, что означает $f(U_\delta(\mathbf{x}_0)) \subset U_\varepsilon(f(\mathbf{x}_0))$. Это определение непрерывности.

**Непрерывность композиции непрерывных отображений**
Если $\mathbf{g}: X \subset R^n \to Y \subset R^k$ непрерывно в $\mathbf{x}_0$, и $\mathbf{f}: Y \to Z \subset R^m$ непрерывно в $\mathbf{y}_0 = \mathbf{g}(\mathbf{x}_0)$, то композиция $\mathbf{h} = \mathbf{f} \circ \mathbf{g}: X \to Z$ непрерывна в $\mathbf{x}_0$ [1, стр. 200-201].

* Док-во: Для $\forall \varepsilon > 0$, из непр. $\mathbf{f}$ в $\mathbf{y}_0$ $\exists \sigma > 0 : \|\mathbf{y} - \mathbf{y}_0\| < \sigma \implies \|\mathbf{f}(\mathbf{y}) - \mathbf{f}(\mathbf{y}_0)\| < \varepsilon$. Из непр. $\mathbf{g}$ в $\mathbf{x}_0$ для этого $\sigma$ $\exists \delta > 0 : \|\mathbf{x} - \mathbf{x}_0\| < \delta \implies \|\mathbf{g}(\mathbf{x}) - \mathbf{g}(\mathbf{x}_0)\| < \sigma$. Тогда для $\|\mathbf{x} - \mathbf{x}_0\| < \delta \implies \|\mathbf{g}(\mathbf{x}) - \mathbf{y}_0\| < \sigma \implies \|\mathbf{f}(\mathbf{g}(\mathbf{x})) - \mathbf{f}(\mathbf{y}_0)\| < \varepsilon$.

**Связность и линейная связность множеств**

* **Связное мн-во**: Мн-во $E \subset R^n$ связно, если его нельзя представить в виде $E = A \cup B$, где $A, B$ непусты, $A \cap B = \emptyset$, и $A, B$ открыты в $E$ (т.е. $A = E \cap G_A, B = E \cap G_B$ для открытых в $R^n$ мн-в $G_A, G_B$) [1, стр. 201]. (Без док-ва свойств).
* **Линейно связное мн-во**: Мн-во $E \subset R^n$ линейно связно, если $\forall \mathbf{a}, \mathbf{b} \in E$ существует непрерывная кривая $\gamma: [^1] \to E$ такая, что $\gamma(0)=\mathbf{a}, \gamma(1)=\mathbf{b}$ [1, стр. 201].
* **Эквивалентность для открытых мн-в**: Открытое мн-во в $R^n$ связно $\iff$ оно линейно связно [1, стр. 202].
* **Сохранение связности**: Непрерывный образ связного мн-ва связен [1, стр. 201]. (Без док-ва).
* **Сохранение линейной связности**: Непрерывный образ линейно связного мн-ва линейно связен [1, стр. 201].
    * Док-во: Пусть $f: E \to R^m$ непр., $E$ лин. связно. $\forall \mathbf{y}_1, \mathbf{y}_2 \in f(E)$, $\exists \mathbf{x}_1, \mathbf{x}_2 \in E : f(\mathbf{x}_1)=\mathbf{y}_1, f(\mathbf{x}_2)=\mathbf{y}_2$. Т.к. $E$ лин. связно, $\exists \gamma(t): [^1] \to E$ непр. кривая, $\gamma(0)=\mathbf{x}_1, \gamma(1)=\mathbf{x}_2$. Тогда $\tilde{\gamma}(t) = f(\gamma(t))$ — непр. кривая в $f(E)$, $\tilde{\gamma}(0)=\mathbf{y}_1, \tilde{\gamma}(1)=\mathbf{y}_2$.


## 4. Компакты в $R^n$. Свойства непрерывных на компакте функций.

**Компакты в $R^n$**

* **Опр. (Гейне-Бореля-Лебега)**: Мн-во $K \subset R^n$ наз. компактом (компактным), если оно замкнуто и ограничено [1, стр. 191-192].
* **Опр. (через покрытия)**: Мн-во $K$ компактно, если из любого его открытого покрытия $\{G_\alpha\}$ ($K \subset \bigcup_\alpha G_\alpha$) можно выделить конечное подпокрытие ($K \subset \bigcup_{i=1}^N G_{\alpha_i}$). (Это определение более общее).

**Свойства функций, непрерывных на компакте**
Пусть $f: K \to R^m$ непрерывна на компакте $K \subset R^n$.

* **Т-ма Вейерштрасса 1 (об ограниченности)**: Если $f: K \to R$ (скалярная функция) непрерывна на компакте $K$, то $f$ ограничена на $K$ [1, стр. 194].
    * Док-во (от противного): Предположим, $f$ не ограничена. Тогда $\forall n \in \mathbb{N} \ \exists \mathbf{x}_n \in K : |f(\mathbf{x}_n)| > n$. Т.к. $K$ компакт, из посл-ти $\{\mathbf{x}_n\}$ можно выделить сх. подпосл-ть $\{\mathbf{x}_{n_k}\} \to \mathbf{x}_0 \in K$. Из непр. $f$, $f(\mathbf{x}_{n_k}) \to f(\mathbf{x}_0)$. Но $|f(\mathbf{x}_{n_k})| > n_k \to \infty$, противоречие.
* **Т-ма Вейерштрасса 2 (о достижении точных граней)**: Если $f: K \to R$ непрерывна на компакте $K$, то она достигает на $K$ своих точных верхней и нижней граней (т.е. $\exists \mathbf{x}_*, \mathbf{x}^* \in K : f(\mathbf{x}_*) = \inf_K f, f(\mathbf{x}^*) = \sup_K f$) [1, стр. 194].
    * Док-во (для $\sup$): По т.1, $M = \sup_K f < \infty$. По опр. $\sup$, $\forall n \in \mathbb{N} \ \exists \mathbf{x}_n \in K : M - 1/n < f(\mathbf{x}_n) \le M$. Из $\{\mathbf{x}_n\} \subset K$ (компакт) $\exists$ сх. подпосл-ть $\mathbf{x}_{n_k} \to \mathbf{x}^* \in K$. Из непр. $f$, $f(\mathbf{x}_{n_k}) \to f(\mathbf{x}^*)$. Из $M - 1/n_k < f(\mathbf{x}_{n_k}) \le M$ по предельному переходу $f(\mathbf{x}^*) = M$.
* **Т-ма Кантора (о равномерной непрерывности)**: Если $f: K \to R^m$ непрерывна на компакте $K$, то $f$ равномерно непрерывна на $K$. Т.е. $\forall \varepsilon > 0 \ \exists \delta > 0 : \forall \mathbf{x}', \mathbf{x}'' \in K, \|\mathbf{x}' - \mathbf{x}''\| < \delta \implies \|f(\mathbf{x}') - f(\mathbf{x}'')\| < \varepsilon$ [1, стр. 195].
    * Док-во (от противного): Предп. $f$ не р.н. Тогда $\exists \varepsilon_0 > 0 : \forall \delta_n = 1/n \ \exists \mathbf{x}_n', \mathbf{x}_n'' \in K : \|\mathbf{x}_n' - \mathbf{x}_n''\| < 1/n$ но $\|f(\mathbf{x}_n') - f(\mathbf{x}_n'')\| \ge \varepsilon_0$. Из $\{\mathbf{x}_n'\} \subset K$ $\exists$ сх. подпосл-ть $\mathbf{x}_{n_k}' \to \mathbf{x}_0 \in K$. Тогда и $\mathbf{x}_{n_k}'' \to \mathbf{x}_0$ (т.к. $\|\mathbf{x}_{n_k}' - \mathbf{x}_{n_k}''\| < 1/n_k \to 0$). Из непр. $f$, $f(\mathbf{x}_{n_k}') \to f(\mathbf{x}_0)$ и $f(\mathbf{x}_{n_k}'') \to f(\mathbf{x}_0)$. Тогда $\|f(\mathbf{x}_{n_k}') - f(\mathbf{x}_{n_k}'')\| \to 0$. Противоречие с $\|f(\mathbf{x}_n') - f(\mathbf{x}_n'')\| \ge \varepsilon_0$.


## 5. Диф-ть фмп. Производные, градиент. Условия диф-ти. Матрица Якоби. Диф-ть композиции.

**Дифференцируемость функции $f: D \subset R^n \to R$ в точке $\mathbf{x}_0 \in \text{int } D$**
Ф-ия $f$ диф-ма в $\mathbf{x}_0$, если ее приращение $\Delta f = f(\mathbf{x}_0 + \Delta\mathbf{x}) - f(\mathbf{x}_0)$ можно представить в виде: $\Delta f = \mathbf{A} \cdot \Delta\mathbf{x} + o(\|\Delta\mathbf{x}\|)$ при $\Delta\mathbf{x} \to \mathbf{0}$ [1, стр. 272].
Здесь $\mathbf{A} = (A_1, ..., A_n)$ — вектор-строка (линейный функционал), $\mathbf{A} \cdot \Delta\mathbf{x}$ — скалярное произведение. $\mathbf{A}$ наз. производной (или дифференциалом) $f$ в $\mathbf{x}_0$. Обозн. $df(\mathbf{x}_0)$ или $f'(\mathbf{x}_0)$.

**Производные по направлению, частные производные (ч.п.), градиент**

* **Ч.п.**: $\frac{\partial f}{\partial x_i}(\mathbf{x}_0) = \lim_{h \to 0} \frac{f(x_{0,1}, ..., x_{0,i}+h, ..., x_{0,n}) - f(\mathbf{x}_0)}{h}$ [1, стр. 273]. Если $f$ диф-ма в $\mathbf{x}_0$, то $A_i = \frac{\partial f}{\partial x_i}(\mathbf{x}_0)$.
* **Градиент**: $\nabla f(\mathbf{x}_0) = \text{grad } f(\mathbf{x}_0) = \left(\frac{\partial f}{\partial x_1}(\mathbf{x}_0), ..., \frac{\partial f}{\partial x_n}(\mathbf{x}_0)\right)$. Тогда $df(\mathbf{x}_0)(\Delta\mathbf{x}) = \nabla f(\mathbf{x}_0) \cdot \Delta\mathbf{x}$ [1, стр. 273].
* **Производная по направлению $\mathbf{v}$ ($\|\mathbf{v}\|=1$)**: $\frac{\partial f}{\partial \mathbf{v}}(\mathbf{x}_0) = \lim_{t \to 0^+} \frac{f(\mathbf{x}_0 + t\mathbf{v}) - f(\mathbf{x}_0)}{t}$. Если $f$ диф-ма, то $\frac{\partial f}{\partial \mathbf{v}}(\mathbf{x}_0) = \nabla f(\mathbf{x}_0) \cdot \mathbf{v}$ [1, стр. 273].

**Условия дифференцируемости**

* **Необходимые**: Если $f$ диф-ма в $\mathbf{x}_0$:

1. Существуют все ч.п. $\frac{\partial f}{\partial x_i}(\mathbf{x}_0)$ [1, стр. 273].
2. $f$ непрерывна в $\mathbf{x}_0$ [1, стр. 273].
    * Док-во (2): $\Delta f = \nabla f(\mathbf{x}_0) \cdot \Delta\mathbf{x} + o(\|\Delta\mathbf{x}\|)$. При $\Delta\mathbf{x} \to \mathbf{0}$, $\Delta f \to 0$.
* **Достаточные**: Если все ч.п. $\frac{\partial f}{\partial x_i}$ существуют в некоторой окрестности точки $\mathbf{x}_0$ и непрерывны в самой точке $\mathbf{x}_0$, то $f$ диф-ма в $\mathbf{x}_0$ [1, стр. 274].
    * Док-во (идея для $n=2$): $\Delta f = f(x_0+\Delta x, y_0+\Delta y) - f(x_0, y_0) = [f(x_0+\Delta x, y_0+\Delta y) - f(x_0, y_0+\Delta y)] + [f(x_0, y_0+\Delta y) - f(x_0, y_0)]$. Применить т. Лагранжа к каждому слагаемому. Использовать непр. ч.п.

**Матрица Якоби отображения $\mathbf{F}: D \subset R^n \to R^m$, $\mathbf{F}=(f_1, ..., f_m)$**
Отображение $\mathbf{F}$ диф-мо в $\mathbf{x}_0$, если $\Delta \mathbf{F} = \mathbf{F}(\mathbf{x}_0 + \Delta\mathbf{x}) - \mathbf{F}(\mathbf{x}_0) = J_{\mathbf{F}}(\mathbf{x}_0) \Delta\mathbf{x} + \mathbf{o}(\|\Delta\mathbf{x}\|)$, где $J_{\mathbf{F}}(\mathbf{x}_0)$ — матрица Якоби (линейный оператор):
$J_{\mathbf{F}}(\mathbf{x}_0) = \begin{pmatrix} \frac{\partial f_1}{\partial x_1} & \cdots & \frac{\partial f_1}{\partial x_n} \\ \vdots & \ddots & \vdots \\ \frac{\partial f_m}{\partial x_1} & \cdots & \frac{\partial f_m}{\partial x_n} \end{pmatrix}_{\mathbf{x}=\mathbf{x}_0}$
[1, стр. 273]. Якобиан — $\det(J_{\mathbf{F}})$, если $n=m$.

**Дифференцируемость композиции отображений (цепное правило)**
Пусть $\mathbf{g}: D_g \subset R^n \to D_f \subset R^k$ диф-мо в $\mathbf{x}_0$, и $\mathbf{f}: D_f \to R^m$ диф-мо в $\mathbf{y}_0 = \mathbf{g}(\mathbf{x}_0)$. Тогда композиция $\mathbf{h}(\mathbf{x}) = \mathbf{f}(\mathbf{g}(\mathbf{x}))$ диф-ма в $\mathbf{x}_0$, и ее матрица Якоби: $J_{\mathbf{h}}(\mathbf{x}_0) = J_{\mathbf{f}}(\mathbf{y}_0) \cdot J_{\mathbf{g}}(\mathbf{x}_0)$ (произведение матриц) [1, стр. 275].

* Док-во (идея): $\Delta \mathbf{h} = \Delta \mathbf{f}(\mathbf{g}(\mathbf{x}_0+\Delta\mathbf{x})) - \mathbf{f}(\mathbf{g}(\mathbf{x}_0))$. $\Delta \mathbf{y} = \mathbf{g}(\mathbf{x}_0+\Delta\mathbf{x}) - \mathbf{g}(\mathbf{x}_0) = J_{\mathbf{g}}(\mathbf{x}_0)\Delta\mathbf{x} + \mathbf{o}(\|\Delta\mathbf{x}\|)$. $\Delta \mathbf{f} = J_{\mathbf{f}}(\mathbf{y}_0)\Delta\mathbf{y} + \mathbf{o}(\|\Delta\mathbf{y}\|)$. Подставить $\Delta\mathbf{y}$, учесть $\|\Delta\mathbf{y}\| = O(\|\Delta\mathbf{x}\|)$.


## 6. Ч.п. и диф-лы высш. порядков. Формула Тейлора.

**Частные производные (ч.п.) и дифференциалы (диф-лы) высших порядков**

* **Ч.п. высших порядков**: $\frac{\partial^2 f}{\partial x_j \partial x_i} = \frac{\partial}{\partial x_j}\left(\frac{\partial f}{\partial x_i}\right)$, $\frac{\partial^2 f}{\partial x_i^2} = \frac{\partial}{\partial x_i}\left(\frac{\partial f}{\partial x_i}\right)$ и т.д. [1, стр. 276].
* **Диф-лы высших порядков**: $d^k f(\mathbf{x}_0; \Delta\mathbf{x}) = \left(\sum_{i=1}^n \Delta x_i \frac{\partial}{\partial x_i}\right)^k f(\mathbf{x}_0)$.
Напр., $d^2 f = \sum_{i,j=1}^n \frac{\partial^2 f}{\partial x_i \partial x_j}(\mathbf{x}_0) \Delta x_i \Delta x_j$ [1, стр. 276]. ($\Delta x_i$ здесь рассматриваются как фиксированные приращения).

**Независимость смешанной ч.п. от порядка дифференцирования (Т-ма Шварца/Юнга/Клеро)**
Если ч.п. $\frac{\partial^2 f}{\partial x_i \partial x_j}$ и $\frac{\partial^2 f}{\partial x_j \partial x_i}$ существуют в окрестности точки $\mathbf{x}_0$ и непрерывны в $\mathbf{x}_0$, то $\frac{\partial^2 f}{\partial x_i \partial x_j}(\mathbf{x}_0) = \frac{\partial^2 f}{\partial x_j \partial x_i}(\mathbf{x}_0)$ [1, стр. 277].

* Док-во (для $n=2$, $f(x,y)$): Рассмотреть выражение $W = f(x+h, y+k) - f(x+h, y) - f(x, y+k) + f(x,y)$. Ввести $\varphi(x) = f(x, y+k) - f(x,y)$, тогда $W = \varphi(x+h) - \varphi(x)$. По т. Лагранжа $W = h \varphi'(x+\theta_1 h) = h [f'_x(x+\theta_1 h, y+k) - f'_x(x+\theta_1 h, y)]$. Еще раз т. Лагранжа: $W = hk f''_{xy}(x+\theta_1 h, y+\theta_2 k)$. Аналогично, группируя по-другому, $W = kh f''_{yx}(x+\theta_3 h, y+\theta_4 k)$. Разделить на $hk$, устремить $h,k \to 0$, используя непрерывность вторых производных.

**Инвариантность формы дифференциала**

* **Первого порядка $df$**: Форма $df = \sum_{i=1}^n \frac{\partial f}{\partial u_i} du_i$ инвариантна, т.е. не зависит от того, являются ли $u_i$ независимыми переменными или функциями других независимых переменных $x_j$ ($u_i = u_i(x_1, ..., x_k)$) [1, стр. 278].
* **Второго порядка $d^2f$**: Форма $d^2 f = \sum_{i,j=1}^n \frac{\partial^2 f}{\partial u_i \partial u_j} du_i du_j$ инвариантна (сохраняется) **только если** $u_i$ являются **линейными** функциями независимых переменных ($u_i = \sum a_{ij} x_j + b_i$), т.е. $d^2u_i = 0$ [1, стр. 278]. В общем случае $d^2f = \sum_{i,j} \frac{\partial^2 f}{\partial u_i \partial u_j} du_i du_j + \sum_k \frac{\partial f}{\partial u_k} d^2 u_k$.

**Формула Тейлора для фмп**
Пусть $f$ имеет непр. ч.п. до порядка $k+1$ в окрестности $\mathbf{x}_0$. Тогда для $\mathbf{x}$ из этой окрестности:
$f(\mathbf{x}) = f(\mathbf{x}_0) + \sum_{m=1}^k \frac{1}{m!} d^m f(\mathbf{x}_0; \mathbf{x}-\mathbf{x}_0) + R_k(\mathbf{x})$,
где $d^m f(\mathbf{x}_0; \mathbf{x}-\mathbf{x}_0) = \left( (x_1-x_{0,1})\frac{\partial}{\partial x_1} + ... + (x_n-x_{0,n})\frac{\partial}{\partial x_n} \right)^m f(\mathbf{x}_0)$.

* **Остаточный член в форме Пеано**: Если $f$ имеет непр. ч.п. до порядка $k$ в $\mathbf{x}_0$, то $R_k(\mathbf{x}) = o(\|\mathbf{x}-\mathbf{x}_0\|^k)$ при $\mathbf{x} \to \mathbf{x}_0$ [1, стр. 279].
* **Остаточный член в форме Лагранжа**: Если $f$ имеет непр. ч.п. до порядка $k+1$ в окрестности $\mathbf{x}_0$, то $R_k(\mathbf{x}) = \frac{1}{(k+1)!} d^{k+1} f(\mathbf{x}_0 + \theta(\mathbf{x}-\mathbf{x}_0); \mathbf{x}-\mathbf{x}_0)$ для некоторого $\theta \in (0,1)$ [1, стр. 280].
* **Интегральная форма остаточного члена**: Если $f$ имеет непр. ч.п. до порядка $k+1$ на отрезке $[\mathbf{x}_0, \mathbf{x}]$, то $R_k(\mathbf{x}) = \frac{1}{k!} \int_0^1 (1-t)^k d^{k+1} f(\mathbf{x}_0 + t(\mathbf{x}-\mathbf{x}_0); \mathbf{x}-\mathbf{x}_0) dt$ (здесь $d^{k+1}f$ рассматривается как функция от $t$ по первой компоненте) [1, стр. 281].
    * Док-во (идея): Рассмотреть $\varphi(t) = f(\mathbf{x}_0+t(\mathbf{x}-\mathbf{x}_0))$. Разложить $\varphi(t)$ по ф-ле Тейлора для одной переменной в точке $t=0$ до $t=1$.


## 7. Теоремы о неявной функции и об обратном отображении.

**Теорема о неявной функции, заданной одним уравнением**
Пусть $F(x_1, ..., x_n, y) \equiv F(\mathbf{x}, y)$ определена в окрестности точки $M_0(\mathbf{x}_0, y_0)$. Если:

1. $F \in C^1(U(M_0))$ (т.е. $F$ и ее ч.п. $\frac{\partial F}{\partial x_i}, \frac{\partial F}{\partial y}$ непрерывны в $U(M_0)$).
2. $F(\mathbf{x}_0, y_0) = 0$.
3. $\frac{\partial F}{\partial y}(\mathbf{x}_0, y_0) \neq 0$.
Тогда $\exists$ окрестность $U(\mathbf{x}_0)$ точки $\mathbf{x}_0$ и окрестность $V(y_0)$ точки $y_0$ и **единственная** функция $y = f(\mathbf{x})$, определенная и непрерывно диф-ма в $U(\mathbf{x}_0)$, такая что:
а) $\forall \mathbf{x} \in U(\mathbf{x}_0) \implies f(\mathbf{x}) \in V(y_0)$ (график локально не выходит из "коробки").
б) $y_0 = f(\mathbf{x}_0)$.
в) $F(\mathbf{x}, f(\mathbf{x})) \equiv 0$ для $\forall \mathbf{x} \in U(\mathbf{x}_0)$.
Причем ч.п. функции $f$ находятся по формуле: $\frac{\partial f}{\partial x_i}(\mathbf{x}) = - \frac{\frac{\partial F}{\partial x_i}(\mathbf{x}, f(\mathbf{x}))}{\frac{\partial F}{\partial y}(\mathbf{x}, f(\mathbf{x}))}$ [1, стр. 284].

* Док-во (идея существования для $n=1$): Из (3) (пусть $F'_y > 0$) $\implies F$ строго возрастает по $y$ около $y_0$. Из (2) и непр. $F$, для $\mathbf{x}$ близких к $\mathbf{x}_0$, $F(\mathbf{x}, y_0-\varepsilon) < 0$ и $F(\mathbf{x}, y_0+\varepsilon) > 0$. По т. о промежуточном значении $\forall \mathbf{x}$ близкого к $\mathbf{x}_0$ $\exists ! y \in (y_0-\varepsilon, y_0+\varepsilon)$ такое, что $F(\mathbf{x},y)=0$. Это определяет $y=f(\mathbf{x})$. Диф-ть доказывается отдельно.

**Теорема о системе неявных функций**
Пусть дана система $\begin{cases} F_1(x_1, ..., x_n, y_1, ..., y_m) = 0 \\ ... \\ F_m(x_1, ..., x_n, y_1, ..., y_m) = 0 \end{cases}$ или $\mathbf{F}(\mathbf{x}, \mathbf{y}) = \mathbf{0}$.
Пусть $\mathbf{F}: R^{n+m} \to R^m$ определена в окрестности точки $P_0(\mathbf{x}_0, \mathbf{y}_0)$. Если:

1. $\mathbf{F} \in C^1(U(P_0))$ (все компоненты $F_j$ и их ч.п. непрерывны).
2. $\mathbf{F}(\mathbf{x}_0, \mathbf{y}_0) = \mathbf{0}$.
3. Якобиан $\frac{D(F_1, ..., F_m)}{D(y_1, ..., y_m)}(\mathbf{x}_0, \mathbf{y}_0) = \det \left( \frac{\partial F_i}{\partial y_j}(\mathbf{x}_0, \mathbf{y}_0) \right)_{i,j=1}^m \neq 0$.
Тогда $\exists$ окрестность $U(\mathbf{x}_0)$ и окрестность $V(\mathbf{y}_0)$ и **единственное** отображение $\mathbf{y} = \mathbf{f}(\mathbf{x})$, $\mathbf{f}: U(\mathbf{x}_0) \to V(\mathbf{y}_0)$, такое что $\mathbf{f}$ непрерывно диф-мо в $U(\mathbf{x}_0)$ и:
а) $\mathbf{y}_0 = \mathbf{f}(\mathbf{x}_0)$.
б) $\mathbf{F}(\mathbf{x}, \mathbf{f}(\mathbf{x})) \equiv \mathbf{0}$ для $\forall \mathbf{x} \in U(\mathbf{x}_0)$.
Матрица Якоби $J_{\mathbf{f}}(\mathbf{x})$ находится из \$ [J_{\mathbf{y}}\mathbf{F}] \cdot J_{\mathbf{f}} + [J_{\mathbf{x}}\mathbf{F}] = 0 \implies J_{\mathbf{f}} = - [J_{\mathbf{y}}\mathbf{F}]^{-1} \cdot [J_{\mathbf{x}}\mathbf{F}] \$ [1, стр. 286].

**Теорема о локальной обратимости (об обратном отображении)**
Пусть отображение $\mathbf{f}: D \subset R^n \to R^n$ ($D$ — открытое мн-во). Если:

1. $\mathbf{f} \in C^1(D)$ (непрерывно диф-мо в $D$).
2. В точке $\mathbf{x}_0 \in D$ якобиан $\det(J_{\mathbf{f}}(\mathbf{x}_0)) \neq 0$.
Тогда $\exists$ окрестность $U(\mathbf{x}_0)$ точки $\mathbf{x}_0$ и окрестность $V(\mathbf{y}_0)$ точки $\mathbf{y}_0 = \mathbf{f}(\mathbf{x}_0)$ такие, что:
а) Отображение $\mathbf{f}: U \to V$ является биекцией (взаимно однозначно).
б) Обратное отображение $\mathbf{g} = \mathbf{f}^{-1}: V \to U$ также непрерывно диф-мо ($\mathbf{g} \in C^1(V)$).
в) Матрица Якоби обратного отображения: $J_{\mathbf{g}}(\mathbf{y}) = [J_{\mathbf{f}}(\mathbf{g}(\mathbf{y}))]^{-1}$ для $\mathbf{y} \in V$ [1, стр. 287].

* Док-во (идея): Рассмотреть систему $\mathbf{F}(\mathbf{y}, \mathbf{x}) = \mathbf{f}(\mathbf{x}) - \mathbf{y} = \mathbf{0}$. Применить т. о системе неявных функций, чтобы выразить $\mathbf{x}$ через $\mathbf{y}$. Якобиан $\frac{D(F_1,...,F_n)}{D(x_1,...,x_n)} = \det(J_{\mathbf{f}}(\mathbf{x}_0)) \neq 0$.


## 8. Экстремумы фмп: необх. и дост. условия.

**Локальный экстремум**
Точка $\mathbf{x}_0 \in D(f)$ наз. точкой локального минимума (максимума) функции $f$, если $\exists U(\mathbf{x}_0)$ такая, что $\forall \mathbf{x} \in U(\mathbf{x}_0) \cap D(f) \setminus \{\mathbf{x}_0\}$ выполняется $f(\mathbf{x}) \ge f(\mathbf{x}_0)$ (соотв. $f(\mathbf{x}) \le f(\mathbf{x}_0)$). Если неравенства строгие, то экстремум строгий [1, стр. 289].

**Необходимые условия экстремума (Теорема Ферма)**
Если $f$ диф-ма в точке $\mathbf{x}_0$ и $\mathbf{x}_0$ — точка локального экстремума, то $\nabla f(\mathbf{x}_0) = \mathbf{0}$ (т.е. все ч.п. 1-го порядка $\frac{\partial f}{\partial x_i}(\mathbf{x}_0) = 0$) [1, стр. 289].
Точки, где $\nabla f = \mathbf{0}$, наз. стационарными или критическими.

* Док-во: Зафиксировать все переменные, кроме $x_i$. Рассмотреть $g(t) = f(x_{0,1}, ..., x_{0,i-1}, t, x_{0,i+1}, ..., x_{0,n})$. Точка $x_{0,i}$ будет точкой экстремума для $g(t)$. По т. Ферма для одной переменной $g'(x_{0,i}) = \frac{\partial f}{\partial x_i}(\mathbf{x}_0) = 0$. Повторить для всех $i$.

**Достаточные условия экстремума (для $f \in C^2$)**
Пусть $\mathbf{x}_0$ — стационарная точка $f$ ($\nabla f(\mathbf{x}_0) = \mathbf{0}$), и $f$ дважды непрерывно диф-ма в окрестности $\mathbf{x}_0$.
Рассмотрим второй дифференциал (квадратичную форму от приращений $\mathbf{h} = (h_1, ..., h_n)$):
$d^2f(\mathbf{x}_0; \mathbf{h}) = \sum_{i,j=1}^n \frac{\partial^2 f}{\partial x_i \partial x_j}(\mathbf{x}_0) h_i h_j = \mathbf{h}^T H(\mathbf{x}_0) \mathbf{h}$, где $H(\mathbf{x}_0)$ — матрица Гессе (гессиан).

1. Если $d^2f(\mathbf{x}_0; \mathbf{h})$ положительно определена ($d^2f > 0$ для $\mathbf{h} \neq \mathbf{0}$), то $\mathbf{x}_0$ — точка строгого локального минимума.
2. Если $d^2f(\mathbf{x}_0; \mathbf{h})$ отрицательно определена ($d^2f < 0$ для $\mathbf{h} \neq \mathbf{0}$), то $\mathbf{x}_0$ — точка строгого локального максимума.
3. Если $d^2f(\mathbf{x}_0; \mathbf{h})$ знакопеременна (принимает и полож., и отриц. значения), то в $\mathbf{x}_0$ экстремума нет (седловая точка).
4. Если $d^2f(\mathbf{x}_0; \mathbf{h})$ полуопределена (нестрого $\ge 0$ или нестрого $\le 0$, и $\exists \mathbf{h} \neq \mathbf{0}$ : $d^2f=0$), то требуется дополнительное исследование (напр., знака $f(\mathbf{x}) - f(\mathbf{x}_0)$ или старших диф-лов) [1, стр. 290].

* Док-во (идея для 1): Из ф-лы Тейлора: $f(\mathbf{x}_0+\mathbf{h}) - f(\mathbf{x}_0) = \nabla f(\mathbf{x}_0)\cdot \mathbf{h} + \frac{1}{2} d^2f(\mathbf{x}_0; \mathbf{h}) + o(\|\mathbf{h}\|^2)$. Т.к. $\nabla f(\mathbf{x}_0)=\mathbf{0}$, то $f(\mathbf{x}_0+\mathbf{h}) - f(\mathbf{x}_0) = \frac{1}{2} d^2f(\mathbf{x}_0; \mathbf{h}) + o(\|\mathbf{h}\|^2)$. Если $d^2f$ полож. определена, то $d^2f(\mathbf{x}_0; \mathbf{h}) \ge \lambda_{\min} \|\mathbf{h}\|^2$ ($\lambda_{\min}$ > 0 — мин. собств. число гессиана). Тогда для малых $\|\mathbf{h}\|$ знак $f(\mathbf{x}_0+\mathbf{h}) - f(\mathbf{x}_0)$ определяется знаком $d^2f$.
* **Критерий Сильвестра** (для знакоопределенности $d^2f$): Пусть $\Delta_k$ — главные угловые миноры матрицы Гессе $H(\mathbf{x}_0)$.
    * $d^2f > 0 \iff \Delta_1 > 0, \Delta_2 > 0, ..., \Delta_n > 0$.
    * $d^2f < 0 \iff \Delta_1 < 0, \Delta_2 > 0, \Delta_3 < 0, ..., (-1)^n \Delta_n > 0$.


## 9. Условные экстремумы. Метод Лагранжа.

**Условный экстремум**
Экстремум функции $f(x_1, ..., x_n)$ при наличии $m$ условий (ограничений) вида $\varphi_k(x_1, ..., x_n) = 0$, $k=1, ..., m$, где $m < n$ [1, стр. 291]. Точка $\mathbf{x}_0$, удовлетворяющая условиям, наз. точкой условного экстремума, если она является точкой обычного экстремума для $f$ на мн-ве $M = \{\mathbf{x} \in R^n : \varphi_k(\mathbf{x})=0 \ \forall k\}$.

**Метод множителей Лагранжа: необходимые условия**
Для нахождения точек возможного условного экстремума составляется **функция Лагранжа**:
$L(\mathbf{x}, \boldsymbol{\lambda}) = f(\mathbf{x}) + \sum_{k=1}^m \lambda_k \varphi_k(\mathbf{x})$, где $\boldsymbol{\lambda} = (\lambda_1, ..., \lambda_m)$ — множители Лагранжа.
**Теорема**: Если $\mathbf{x}_0$ — точка условного экстремума функции $f$ при условиях $\varphi_k(\mathbf{x})=0$, $f, \varphi_k \in C^1$ в окрестности $\mathbf{x}_0$, и ранг матрицы Якоби системы ограничений $\left( \frac{\partial \varphi_k}{\partial x_j}(\mathbf{x}_0) \right)_{k=1..m, j=1..n}$ равен $m$ (т.е. градиенты $\nabla \varphi_k(\mathbf{x}_0)$ линейно независимы), то $\exists \boldsymbol{\lambda}_0 = (\lambda_{0,1}, ..., \lambda_{0,m})$ такие, что точка $(\mathbf{x}_0, \boldsymbol{\lambda}_0)$ является стационарной для функции Лагранжа $L$:
$\begin{cases} \frac{\partial L}{\partial x_i}(\mathbf{x}_0, \boldsymbol{\lambda}_0) = \frac{\partial f}{\partial x_i}(\mathbf{x}_0) + \sum_{k=1}^m \lambda_{0,k} \frac{\partial \varphi_k}{\partial x_i}(\mathbf{x}_0) = 0, \quad i=1, ..., n \\ \frac{\partial L}{\partial \lambda_k}(\mathbf{x}_0, \boldsymbol{\lambda}_0) = \varphi_k(\mathbf{x}_0) = 0, \quad k=1, ..., m \end{cases}$
[1, стр. 292].

* Док-во (идея): Условия $\varphi_k(\mathbf{x})=0$ определяют ($n-m$)-мерное мн-во. В точке экстремума $\mathbf{x}_0$ вектор $\nabla f(\mathbf{x}_0)$ должен быть ортогонален касательному пространству к этому мн-ву. Векторы $\nabla \varphi_k(\mathbf{x}_0)$ также ортогональны этому пространству. Из линейной независимости $\nabla \varphi_k(\mathbf{x}_0)$ следует, что $\nabla f(\mathbf{x}_0)$ является их линейной комбинацией: $\nabla f(\mathbf{x}_0) = -\sum \lambda_{0,k} \nabla \varphi_k(\mathbf{x}_0)$.

**Метод множителей Лагранжа: достаточные условия**
Пусть $(\mathbf{x}_0, \boldsymbol{\lambda}_0)$ — стационарная точка функции Лагранжа. Пусть $f, \varphi_k \in C^2$ в окрестности $\mathbf{x}_0$.
Рассмотрим второй дифференциал функции Лагранжа по переменным $\mathbf{x}$ в точке $(\mathbf{x}_0, \boldsymbol{\lambda}_0)$ для приращений $\mathbf{h}=(dx_1, ..., dx_n)$, удовлетворяющих условиям связи в дифференциальной форме:
$d^2L_{\mathbf{x}}(\mathbf{x}_0, \boldsymbol{\lambda}_0; \mathbf{h}) = \sum_{i,j=1}^n \frac{\partial^2 L}{\partial x_i \partial x_j}(\mathbf{x}_0, \boldsymbol{\lambda}_0) dx_i dx_j$
при условиях $\sum_{j=1}^n \frac{\partial \varphi_k}{\partial x_j}(\mathbf{x}_0) dx_j = 0$ для $k=1, ..., m$ (т.е. $d\boldsymbol{\varphi}(\mathbf{x}_0; \mathbf{h}) = \mathbf{0}$).

1. Если $d^2L_{\mathbf{x}}(\mathbf{x}_0, \boldsymbol{\lambda}_0; \mathbf{h}) > 0$ для всех $\mathbf{h} \neq \mathbf{0}$, удовлетворяющих $d\boldsymbol{\varphi}=\mathbf{0}$, то $\mathbf{x}_0$ — точка строгого условного локального минимума.
2. Если $d^2L_{\mathbf{x}}(\mathbf{x}_0, \boldsymbol{\lambda}_0; \mathbf{h}) < 0$ для всех $\mathbf{h} \neq \mathbf{0}$, удовлетворяющих $d\boldsymbol{\varphi}=\mathbf{0}$, то $\mathbf{x}_0$ — точка строгого условного локального максимума.
3. Если $d^2L_{\mathbf{x}}$ знакопеременна на этом мн-ве приращений, то условного экстремума в $\mathbf{x}_0$ нет.
4. Если $d^2L_{\mathbf{x}}$ полуопределена, требуется доп. исследование [1, стр. 293].

## 10. Несобственный интеграл (н.и.) Римана. Критерии сх-ти.

**Несобственный интеграл (н.и.) Римана**

* **I рода (бесконечные пределы)**: $\int_a^{\infty} f(x)dx = \lim_{B \to \infty} \int_a^B f(x)dx$. Если предел сущ. и конечен, н.и. сх., иначе расх. [1, стр. 206]. Аналогично для $\int_{-\infty}^b f(x)dx$ и $\int_{-\infty}^{\infty} f(x)dx = \int_{-\infty}^c f(x)dx + \int_c^{\infty} f(x)dx$.
* **II рода (от неограниченной функции)**: Если $f(x)$ не ограничена в окрестности $b$ (особая точка), то $\int_a^b f(x)dx = \lim_{\varepsilon \to 0^+} \int_a^{b-\varepsilon} f(x)dx$. Если особая точка $a$, то $\lim_{\varepsilon \to 0^+} \int_{a+\varepsilon}^b f(x)dx$ [1, стр. 209].

**Критерий Коши сходимости н.и.**
Для $\int_a^{\infty} f(x)dx$: н.и. сх. $\iff \forall \varepsilon > 0 \ \exists A_0 > a : \forall A', A'' > A_0 \implies \left|\int_{A'}^{A''} f(x)dx\right| < \varepsilon$ [1, стр. 211].
Для $\int_a^b f(x)dx$ с особой точкой $b$: н.и. сх. $\iff \forall \varepsilon > 0 \ \exists \delta > 0 : \forall \eta_1, \eta_2 \in (0, \delta) \implies \left|\int_{b-\eta_1}^{b-\eta_2} f(x)dx\right| < \varepsilon$.

* Док-во: Следует из критерия Коши для предела функции $F(B) = \int_a^B f(x)dx$.

**Интегралы от неотрицательных функций ($f(x) \ge 0$)**
Н.и. $\int_a^{\infty} f(x)dx$ (где $f(x) \ge 0$) сх. $\iff$ функция $\Phi(B) = \int_a^B f(x)dx$ ограничена сверху [1, стр. 210].

* Док-во: $\Phi(B)$ не убывает. Если ограничена сверху, то имеет конечный предел. Если не ограничена, то предел $\infty$.

**Признак сравнения (для $f(x) \ge 0, g(x) \ge 0$)**
Пусть $0 \le f(x) \le g(x)$ для $x \ge a$.

1. Если $\int_a^{\infty} g(x)dx$ сх., то $\int_a^{\infty} f(x)dx$ сх.
2. Если $\int_a^{\infty} f(x)dx$ расх., то $\int_a^{\infty} g(x)dx$ расх. [1, стр. 211].

* Док-во (1): $\int_a^B f(x)dx \le \int_a^B g(x)dx$. Если $\int g dx$ сх., то $\int_a^B g(x)dx \le M$. Значит $\int_a^B f(x)dx$ ограничена сверху и сх.
* **Следствия (предельная форма)**: Пусть $f(x) > 0, g(x) > 0$ и $\lim_{x \to \infty} \frac{f(x)}{g(x)} = C$.
    * Если $0 < C < \infty$, то $\int fdx$ и $\int gdx$ сх./расх. одновременно [1, стр. 212].
    * Если $C=0$ и $\int gdx$ сх., то $\int fdx$ сх.
    * Если $C=\infty$ и $\int gdx$ расх., то $\int fdx$ расх.
* **Эталонные интегралы**: $\int_a^{\infty} \frac{dx}{x^p}$ сх. при $p>1$, расх. при $p \le 1$ ($a>0$). $\int_a^b \frac{dx}{(b-x)^p}$ сх. при $p<1$, расх. при $p \ge 1$.

**Абсолютная и условная сходимости интегралов**

* **Абсолютная сх-ть**: Н.и. $\int_a^{\infty} f(x)dx$ сх. абсолютно, если сх. $\int_a^{\infty} |f(x)|dx$ [1, стр. 212].
* Из абсолютной сх-ти следует обычная (просто) сх-ть. Док-во: $| \int_{A'}^{A''} f(x)dx | \le \int_{A'}^{A''} |f(x)|dx$. Применить критерий Коши.
* **Условная сх-ть**: Н.и. сх., но не сх. абсолютно [1, стр. 212]. Пример: $\int_1^{\infty} \frac{\sin x}{x} dx$.

**Признаки Дирихле и Абеля (для знакопеременных функций)**

* **Признак Дирихле**: $\int_a^{\infty} f(x)g(x)dx$ сх., если:

1. Первообразная $F(B) = \int_a^B f(x)dx$ ограничена ($|F(B)| \le M$).
2. Функция $g(x)$ монотонно стремится к 0 при $x \to \infty$ ($g(x) \ monotonically \to 0$) [1, стр. 213].
    * Док-во: Интегрирование по частям $\int_{A'}^{A''} fg dx = [Fg]_{A'}^{A''} - \int_{A'}^{A''} F g' dx$. Использовать вторую теорему о среднем для интеграла $\int F g' dx$.
* **Признак Абеля**: $\int_a^{\infty} f(x)g(x)dx$ сх., если:

1. Н.и. $\int_a^{\infty} f(x)dx$ сх.
2. Функция $g(x)$ монотонна и ограничена [1, стр. 214].
    * Док-во: Если $g(x) \to L \neq 0$, то $g(x) = L + (g(x)-L)$. $g(x)-L$ монотонно $\to 0$. Применить признак Дирихле к $\int f(x)(g(x)-L)dx$.


## 11. Числовые ряды. Критерии сх-ти. Абс. и усл. сх-ть.

**Числовые ряды и их свойства**
Ряд $\sum_{k=1}^{\infty} a_k = a_1 + a_2 + ...$. $S_n = \sum_{k=1}^n a_k$ — $n$-я частичная сумма.
Ряд сх., если $\exists \lim_{n \to \infty} S_n = S$ (конечный предел, сумма ряда). Иначе расх. [1, стр. 217].

* **Необходимый признак сх-ти**: Если $\sum a_k$ сх., то $\lim_{k \to \infty} a_k = 0$ [1, стр. 218]. Обратное неверно (напр., гармонический ряд $\sum 1/k$).
    * Док-во: $a_n = S_n - S_{n-1}$. Если $\lim S_n = S$, то $\lim a_n = S-S=0$.
* **Свойства**: Линейность. Отбрасывание/добавление конечного числа членов не влияет на сх-ть (но влияет на сумму).

**Критерий Коши сходимости ряда**
Ряд $\sum a_k$ сх. $\iff \forall \varepsilon > 0 \ \exists N \in \mathbb{N} : \forall n > N \ \forall p \ge 1 \implies \left|\sum_{k=n+1}^{n+p} a_k\right| < \varepsilon$ ($|S_{n+p} - S_n| < \varepsilon$) [1, стр. 223].

* Док-во: Следует из критерия Коши для посл-ти частичных сумм.

**Ряды с неотрицательными членами ($a_k \ge 0$)**
Ряд $\sum a_k$ (где $a_k \ge 0$) сх. $\iff$ посл-ть частичных сумм $S_n$ ограничена сверху [1, стр. 218].

* **Признак сравнения**: Пусть $0 \le a_k \le b_k$ для $\forall k \ge K_0$.

1. Если $\sum b_k$ сх., то $\sum a_k$ сх.
2. Если $\sum a_k$ расх., то $\sum b_k$ расх. [1, стр. 219].
* **Следствие (предельная форма)**: Если $a_k > 0, b_k > 0$ и $\lim_{k \to \infty} \frac{a_k}{b_k} = C$.
    * Если $0 < C < \infty$, то $\sum a_k$ и $\sum b_k$ сх./расх. одновременно [1, стр. 219].
    * Если $C=0$ и $\sum b_k$ сх., то $\sum a_k$ сх.
    * Если $C=\infty$ и $\sum b_k$ расх., то $\sum a_k$ расх.
* **Признак Даламбера**: Пусть $a_k > 0$. $\lim_{k \to \infty} \frac{a_{k+1}}{a_k} = q$.

1. $q < 1 \implies$ ряд сх. 2. $q > 1 \implies$ ряд расх. 3. $q = 1 \implies$ нет вывода [1, стр. 221].
* **Признак Коши (радикальный)**: Пусть $a_k \ge 0$. $\limsup_{k \to \infty} \sqrt[k]{a_k} = q$ (или $\lim$ если сущ.).

1. $q < 1 \implies$ ряд сх. 2. $q > 1 \implies$ ряд расх. 3. $q = 1 \implies$ нет вывода [1, стр. 221-222].
    * Сравнение: Если сущ. предел Даламбера, то сущ. и предел Коши, и они равны. Обратное не всегда. Признак Коши "сильнее".
* **Интегральный признак Коши-Маклорена**: Если $f(x)$ неотрицательна, не возрастает на $[N, \infty)$ и $a_k = f(k)$, то ряд $\sum_{k=N}^{\infty} a_k$ сх. $\iff$ н.и. $\int_N^{\infty} f(x)dx$ сх. [1, стр. 220].
    * Док-во: $f(k+1) \le \int_k^{k+1} f(x)dx \le f(k)$. Суммируем.
* **Эталонные ряды**: $\sum \frac{1}{k^p}$ (обобщенный гармонический) сх. при $p>1$, расх. при $p \le 1$. Геометрический ряд $\sum q^k$ сх. при $|q|<1$.

**Абсолютная и условная сходимости рядов**

* **Абсолютная сх-ть**: Ряд $\sum a_k$ сх. абсолютно, если сх. ряд $\sum |a_k|$ [1, стр. 223].
* Из абс. сх-ти следует (просто) сх-ть. Док-во: $| \sum_{k=n+1}^{n+p} a_k | \le \sum_{k=n+1}^{n+p} |a_k|$. Применить критерий Коши.
* **Условная сх-ть**: Ряд сх., но не сх. абсолютно. Пример: $\sum (-1)^{k-1}/k$ (знакочередующийся гармонический, ряд Лейбница).

**Признаки Дирихле и Абеля (для знакопеременных рядов)**

* **Признак Дирихле**: Ряд $\sum a_k b_k$ сх., если:

1. Частичные суммы $A_n = \sum_{k=1}^n a_k$ ограничены ($|A_n| \le M$).
2. Посл-ть $b_k$ монотонно стремится к 0 ($b_k \ monotonically \to 0$) [1, стр. 225].
    * Док-во: Преобразование Абеля: $\sum_{k=n+1}^{n+p} a_k b_k = \sum_{k=n+1}^{n+p} (A_k - A_{k-1})b_k = ... = A_{n+p}b_{n+p+1} - A_n b_{n+1} - \sum_{k=n+1}^{n+p} A_k (b_{k+1}-b_k)$. Оценить.
* **Признак Абеля**: Ряд $\sum a_k b_k$ сх., если:

1. Ряд $\sum a_k$ сх.
2. Посл-ть $b_k$ монотонна и ограничена [1, стр. 225].
    * Док-во: $b_k \to L$. $b_k = L + (b_k-L)$. $\sum a_k L$ сх. К $\sum a_k (b_k-L)$ применить признак Дирихле.

**Перестановка членов рядов**

* **Теорема Дирихле**: Если ряд $\sum a_k$ сх. абсолютно, то любой ряд, полученный из него перестановкой членов, также сх. абсолютно и имеет ту же сумму [1, стр. 224].
* **Теорема Римана**: Если ряд $\sum a_k$ сх. условно, то $\forall S \in [-\infty, \infty]$ можно так переставить его члены, что новый ряд будет сх. к $S$. Также можно сделать его расходящимся (колеблющимся) [1, стр. 224].

**Произведение абсолютно сходящихся рядов (Теорема Коши-Мертенса)**
Если ряды $\sum_{n=0}^\infty a_n = A$ и $\sum_{n=0}^\infty b_n = B$ оба сх. абсолютно, то их произведение по Коши $\sum_{n=0}^\infty c_n$, где $c_n = \sum_{k=0}^n a_k b_{n-k}$, также сх. абсолютно и его сумма равна $AB$ [1, стр. 227]. (Утверждение верно, если хотя бы один из рядов сх. абс., а другой просто сх. Тогда произведение сх. к $AB$).

## 12. Равномерно сх. (р.сх.) функц. посл-ти и ряды.

**Равномерно сходящиеся (р.сх.) функциональные последовательности и ряды**

* **Р.сх. посл-ти**: $f_n(x) \rightrightarrows f(x)$ на мн-ве $E$, если $\forall \varepsilon > 0 \ \exists N \in \mathbb{N} : \forall n > N \ \forall x \in E \implies |f_n(x) - f(x)| < \varepsilon$.
Эквивалентно: $\lim_{n \to \infty} \sup_{x \in E} |f_n(x) - f(x)| = 0$ [1, стр. 232, 238].
* **Р.сх. ряда**: $\sum_{k=1}^\infty u_k(x)$ р.сх. на $E$, если посл-ть его частичных сумм $S_n(x) = \sum_{k=1}^n u_k(x)$ р.сх. на $E$ [1, стр. 239].

**Критерий Коши р.сх.**

* **Для посл-ти**: $f_n(x)$ р.сх. на $E \iff \forall \varepsilon > 0 \ \exists N : \forall m, n > N \ \forall x \in E \implies |f_n(x) - f_m(x)| < \varepsilon$ [1, стр. 239].
* **Для ряда**: $\sum u_k(x)$ р.сх. на $E \iff \forall \varepsilon > 0 \ \exists N : \forall n > N \ \forall p \ge 1 \ \forall x \in E \implies \left|\sum_{k=n+1}^{n+p} u_k(x)\right| < \varepsilon$ [1, стр. 240].

**Признаки Вейерштрасса, Дирихле и Абеля р.сх. функциональных рядов**

* **Признак Вейерштрасса (мажорантный)**: Если $\forall x \in E, |u_k(x)| \le c_k$ (для $k \ge K_0$) и числовой ряд $\sum c_k$ сх., то функц. ряд $\sum u_k(x)$ р.сх. (и абсолютно) на $E$ [1, стр. 240].
* **Признак Дирихле р.сх.**: Ряд $\sum a_k(x) b_k(x)$ р.сх. на $E$, если:

1. Частичные суммы $S_n(x) = \sum_{k=1}^n a_k(x)$ равномерно ограничены на $E$ ($\exists M: \forall n, \forall x \in E, |S_n(x)| \le M$).
2. $b_k(x)$ для каждого $x \in E$ монотонна по $k$ и $b_k(x) \rightrightarrows 0$ на $E$ (равномерно стремится к нулю) [1, стр. 242].
* **Признак Абеля р.сх.**: Ряд $\sum a_k(x) b_k(x)$ р.сх. на $E$, если:

1. Ряд $\sum a_k(x)$ р.сх. на $E$.
2. $b_k(x)$ для каждого $x \in E$ монотонна по $k$ и равномерно ограничена на $E$ ($\exists C: \forall k, \forall x \in E, |b_k(x)| \le C$) [1, стр. 242].

**Свойства р.сх. последовательностей и рядов**

* **Непрерывность предела/суммы**:
    * Если $f_n(x)$ непрерывны на $E$ и $f_n(x) \rightrightarrows f(x)$ на $E$, то $f(x)$ непрерывна на $E$.
    * Если $u_k(x)$ непрерывны на $E$ и ряд $\sum u_k(x)$ р.сх. к $S(x)$ на $E$, то $S(x)$ непрерывна на $E$ [1, стр. 234].
    * Док-во (для посл-ти): $|f(x)-f(x_0)| \le |f(x)-f_n(x)| + |f_n(x)-f_n(x_0)| + |f_n(x_0)-f(x_0)|$. Первое и третье слагаемые малы из-за р.сх. (выбрать $n$). Второе мало из-за непр. $f_n$ (выбрать $\delta$ для $x$ близких к $x_0$).
* **Почленное интегрирование**:
    * Если $f_n(x)$ интегрируемы на $[a,b]$ и $f_n(x) \rightrightarrows f(x)$ на $[a,b]$, то $f(x)$ интегрируема на $[a,b]$ и $\lim_{n \to \infty} \int_a^b f_n(x)dx = \int_a^b \lim_{n \to \infty} f_n(x)dx = \int_a^b f(x)dx$.
    * Если $u_k(x)$ интегрируемы на $[a,b]$ и ряд $\sum u_k(x)$ р.сх. к $S(x)$ на $[a,b]$, то $\int_a^b S(x)dx = \sum_{k=1}^\infty \int_a^b u_k(x)dx$ [1, стр. 235-236].
    * Док-во (для посл-ти): $|\int f_n dx - \int f dx| = |\int (f_n-f)dx| \le \int |f_n-f|dx \le \sup|f_n-f| \cdot (b-a)$.
* **Почленное дифференцирование**:
    * Для посл-ти: Если (1) $f_n(x)$ непрерывно диф-мы на $(a,b)$, (2) $f_n(x_0)$ сх. хотя бы в одной точке $x_0 \in (a,b)$, (3) посл-ть производных $f_n'(x) \rightrightarrows g(x)$ на $(a,b)$, ТО $f_n(x) \rightrightarrows f(x)$ на $(a,b)$, $f(x)$ диф-ма, и $f'(x) = g(x) = \lim_{n \to \infty} f_n'(x)$.
    * Для ряда: Если (1) $u_k(x)$ непрерывно диф-мы на $(a,b)$, (2) ряд $\sum u_k(x_0)$ сх. в $x_0 \in (a,b)$, (3) ряд производных $\sum u_k'(x)$ р.сх. к $g(x)$ на $(a,b)$, ТО ряд $\sum u_k(x)$ р.сх. к $S(x)$ на $(a,b)$, $S(x)$ диф-ма, и $S'(x) = g(x) = \sum u_k'(x)$ [1, стр. 236-237].
    * Док-во (идея для посл-ти): Применить т. Лагранжа к $f_n-f_m$. Использовать р.сх. $f_n'$ и сх-ть в точке.


## 13. Степенные ряды с комплексными членами.

**Степенной ряд (с.р.)**: $\sum_{n=0}^{\infty} c_n (z-z_0)^n$, где $c_n \in \mathbb{C}$ (коэффициенты), $z_0 \in \mathbb{C}$ (центр ряда), $z \in \mathbb{C}$ (переменная) [1, стр. 251]. Для простоты часто $z_0=0$: $\sum c_n z^n$.

**Первая теорема Абеля**

1. Если с.р. $\sum c_n (z-z_0)^n$ сх. в точке $z_1 \neq z_0$, то он сх. абсолютно для всех $z$ таких, что $|z-z_0| < |z_1-z_0|$.
2. Если с.р. расх. в точке $z_2$, то он расх. для всех $z$ таких, что $|z-z_0| > |z_2-z_0|$ [1, стр. 252].

* Док-во (1): Т.к. ряд сх. в $z_1$, то $c_n (z_1-z_0)^n \to 0$, значит $\exists M: |c_n (z_1-z_0)^n| \le M$.
Тогда $|c_n (z-z_0)^n| = |c_n (z_1-z_0)^n| \left| \frac{z-z_0}{z_1-z_0} \right|^n \le M q^n$, где $q = \left| \frac{z-z_0}{z_1-z_0} \right| < 1$. Ряд $\sum Mq^n$ сх. (геом. прогрессия). По признаку сравнения, $\sum |c_n (z-z_0)^n|$ сх.

**Круг и радиус сходимости (р.сх.)**
Для любого с.р. $\exists R \in [0, \infty]$ (радиус сх.) такое, что:

* Ряд сх. абсолютно при $|z-z_0| < R$.
* Ряд расх. при $|z-z_0| > R$.
* При $|z-z_0| = R$ (на окружности сх-ти) поведение ряда м.б. различным (требует доп. исследования).
Круг $K_R = \{z \in \mathbb{C} : |z-z_0| < R\}$ наз. кругом сх-ти [1, стр. 252].

**Формула Коши–Адамара для р.сх.**
$R = \frac{1}{L}$, где $L = \limsup_{n \to \infty} \sqrt[n]{|c_n|}$.
(Если $L=0$, то $R=\infty$. Если $L=\infty$, то $R=0$) [1, стр. 254].

* Док-во: Применить признак Коши (радикальный) к ряду $\sum |c_n (z-z_0)^n|$. $\limsup \sqrt[n]{|c_n (z-z_0)^n|} = |z-z_0| \limsup \sqrt[n]{|c_n|} = |z-z_0| L$. Ряд сх. абс., если $|z-z_0| L < 1$, т.е. $|z-z_0| < 1/L$.
* Если $\exists \lim_{n \to \infty} \left|\frac{c_n}{c_{n+1}}\right| = R$, то это также р.сх. (следует из признака Даламбера).

**Характер сходимости с.р. в круге сходимости**
С.р. $\sum c_n (z-z_0)^n$ с р.сх. $R>0$ сх. равномерно на любом замкнутом круге $K' = \{z \in \mathbb{C} : |z-z_0| \le \rho\}$, где $0 < \rho < R$ [1, стр. 252].

* Док-во: Для $z \in K'$, $|c_n (z-z_0)^n| \le |c_n| \rho^n$. Т.к. $\rho < R$, точка $z_1$ такая что $|z_1-z_0|=\rho$ лежит внутри круга сх-ти. Ряд $\sum c_n \rho^n$ сх. абсолютно. Применить признак Вейерштрасса.

**Непрерывность суммы с.р. в этом круге**
Сумма степенного ряда $S(z) = \sum c_n (z-z_0)^n$ является непрерывной функцией в его круге сх-ти $|z-z_0| < R$ [1, стр. 255].

* Док-во: Члены ряда $c_n (z-z_0)^n$ — непр. функции. Ряд р.сх. на любом замкнутом подкруге $|z-z_0| \le \rho < R$. По теореме о непр. суммы р.сх. ряда непр. функций, $S(z)$ непр. на $K'$. Т.к. $\rho$ сколь угодно близко к $R$, $S(z)$ непр. во всем открытом круге $K_R$.


## 14. Степенные ряды с действительными членами.

**Степенные ряды (с.р.) с действительными членами ($x \in R$)**: $\sum_{n=0}^\infty a_n (x-x_0)^n$.
Интервал сх-ти: $(x_0-R, x_0+R)$, где $R$ — р.сх. На концах интервала $x=x_0 \pm R$ требуется отдельное исследование.

**Теоремы об интегрировании и дифференцировании с.р. на интервале сх-ти**
Пусть $S(x) = \sum a_n (x-x_0)^n$ с р.сх. $R>0$.

* **Почленное дифференцирование**: С.р. можно почленно дифференцировать любое число раз внутри интервала сх-ти $(x_0-R, x_0+R)$. Полученный ряд $S'(x) = \sum_{n=1}^{\infty} n a_n (x-x_0)^{n-1}$ имеет тот же р.сх. $R$ [1, стр. 256].
    * Док-во: Р.сх. $R'$ для $\sum n a_n z^{n-1}$. $\limsup \sqrt[n]{n|a_n|} = \limsup (\sqrt[n]{n} \cdot \sqrt[n]{|a_n|}) = 1 \cdot \limsup \sqrt[n]{|a_n|} = 1/R$. Значит $R'=R$.
* **Почленное интегрирование**: С.р. можно почленно интегрировать на любом отрезке $[\alpha, \beta] \subset (x_0-R, x_0+R)$. Полученный ряд $\sum_{n=0}^{\infty} a_n \frac{(x-x_0)^{n+1}}{n+1}$ имеет тот же р.сх. $R$.
$\int_{x_0}^x S(t)dt = \sum_{n=0}^{\infty} \frac{a_n}{n+1} (x-x_0)^{n+1}$ для $x \in (x_0-R, x_0+R)$ [1, стр. 256].

**Единственность представления функции с.р. (рядом Тейлора)**
Если $f(x) = \sum_{n=0}^\infty a_n (x-x_0)^n$ в некоторой окрестности $U(x_0)$, то коэффициенты $a_n$ определяются однозначно: $a_n = \frac{f^{(n)}(x_0)}{n!}$ [1, стр. 257].
Таким образом, если функция разложима в с.р. по степеням $(x-x_0)$, то этот ряд является ее рядом Тейлора.

* Док-во: Положить $x=x_0 \implies a_0 = f(x_0)$. Продифференцировать ряд, положить $x=x_0 \implies a_1 = f'(x_0)$, и т.д.

**Достаточные условия разложимости функции в с.р. (ряд Тейлора)**
Функция $f(x)$ раскладывается в ряд Тейлора $\sum_{n=0}^{\infty} \frac{f^{(n)}(x_0)}{n!} (x-x_0)^n$ на интервале $I$ с центром $x_0$, если $f(x)$ бесконечно диф-ма на $I$ и остаточный член в формуле Тейлора $R_n(x) = f(x) - \sum_{k=0}^n \frac{f^{(k)}(x_0)}{k!} (x-x_0)^k$ стремится к нулю при $n \to \infty$ для $\forall x \in I$ ($\lim_{n \to \infty} R_n(x) = 0$) [1, стр. 258].

* Частое дост. условие: Если $\exists M > 0 : |f^{(n)}(x)| \le M$ для $\forall n$ и $\forall x \in I$, то $R_n(x) \to 0$. Более общее: $|f^{(n)}(x)| \le C \cdot K^n$ или $|f^{(n)}(x)| \le C \cdot n!$ на $I$.

**Разложение в ряд Тейлора основных элементарных функций (в окрестности $x_0=0$)**

1. $e^x = \sum_{n=0}^{\infty} \frac{x^n}{n!} = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + ...$, $x \in R$ ($R=\infty$) [1, стр. 259].
2. $\sin x = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n+1}}{(2n+1)!} = x - \frac{x^3}{3!} + \frac{x^5}{5!} - ...$, $x \in R$ ($R=\infty$) [1, стр. 259].
3. $\cos x = \sum_{n=0}^{\infty} (-1)^n \frac{x^{2n}}{(2n)!} = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - ...$, $x \in R$ ($R=\infty$) [1, стр. 259].
4. $\ln(1+x) = \sum_{n=1}^{\infty} (-1)^{n-1} \frac{x^n}{n} = x - \frac{x^2}{2} + \frac{x^3}{3} - ...$, $x \in (-1, 1]$ ($R=1$) [1, стр. 260].
5. $(1+x)^\alpha = 1 + \sum_{n=1}^{\infty} \frac{\alpha(\alpha-1)...(\alpha-n+1)}{n!} x^n$, $x \in (-1, 1)$ ($R=1$) (биномиальный ряд) [1, стр. 261].
    * $\binom{\alpha}{n} = \frac{\alpha(\alpha-1)...(\alpha-n+1)}{n!}$ — биномиальные коэффициенты.

## 15. Разложение в степенной ряд комплекснозначной функции $e^z$.

**Разложение $e^z$ в степенной ряд**
Для любого комплексного числа $z \in \mathbb{C}$:
$e^z = \sum_{n=0}^{\infty} \frac{z^n}{n!} = 1 + z + \frac{z^2}{2!} + \frac{z^3}{3!} + ...$
Радиус сходимости этого ряда $R=\infty$, т.е. ряд сх. (абсолютно) для всех $z \in \mathbb{C}$ [1, стр. 270].

* **Доказательство 1 (используя $e^z = e^x(\cos y + i \sin y)$)**:
Пусть $z = x+iy$.
$e^z = e^x e^{iy} = e^x (\cos y + i \sin y)$.
Используем известные ряды для действительных $e^x, \cos y, \sin y$:
$e^x = \sum_{k=0}^\infty \frac{x^k}{k!}$
$\cos y = \sum_{m=0}^\infty (-1)^m \frac{y^{2m}}{(2m)!}$
$\sin y = \sum_{m=0}^\infty (-1)^m \frac{y^{2m+1}}{(2m+1)!}$
Тогда $e^z = \left(\sum_{k=0}^\infty \frac{x^k}{k!}\right) \left( \sum_{m=0}^\infty (-1)^m \frac{y^{2m}}{(2m)!} + i \sum_{m=0}^\infty (-1)^m \frac{y^{2m+1}}{(2m+1)!} \right)$.
С другой стороны, $\sum_{n=0}^\infty \frac{z^n}{n!} = \sum_{n=0}^\infty \frac{(x+iy)^n}{n!}$.
По теореме о произведении абсолютно сходящихся рядов, произведение рядов для $e^x$ и $e^{iy}$ (который получается из рядов для $\cos y$ и $\sin y$) должно дать ряд для $e^z$.
Можно показать, что коэффициенты ряда $\sum \frac{(x+iy)^n}{n!}$ совпадают с коэффициентами, полученными при перемножении рядов для $e^x$ и $(\cos y + i\sin y)$. Это довольно громоздко.
Проще использовать тот факт, что ряд $\sum \frac{z^n}{n!}$ определяет целую аналитическую функцию.
* **Доказательство 2 (через свойства аналитических функций)**:
Ряд $S(z) = \sum_{n=0}^\infty \frac{z^n}{n!}$ имеет $R=\infty$ (по формуле Коши-Адамара, $\limsup \sqrt[n]{1/n!} = 0$).
Внутри круга сх-ти степенной ряд можно почленно дифференцировать:
$S'(z) = \sum_{n=1}^\infty \frac{n z^{n-1}}{n!} = \sum_{n=1}^\infty \frac{z^{n-1}}{(n-1)!} = \sum_{k=0}^\infty \frac{z^k}{k!} = S(z)$.
Итак, $S'(z) = S(z)$. Также $S(0) = \frac{0^0}{0!} = 1$.
Функция $e^z$ (определенная, например, как $e^x(\cos y + i\sin y)$) также удовлетворяет \$ (e^z)' = e^z \$ и $e^0 = 1$.
По теореме единственности решения дифференциального уравнения $f'(z)=f(z)$ с начальным условием $f(0)=1$ в классе аналитических функций, следует, что $S(z) = e^z$ для всех $z \in \mathbb{C}$.

<div style="text-align: center">⁂</div>

[^1]: matangus.pdf

