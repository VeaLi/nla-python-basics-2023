<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Импортирование-и-использование-библиотек" data-toc-modified-id="Импортирование-и-использование-библиотек-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Импортирование и использование библиотек</a></span></li><li><span><a href="#Что-значит-запись-import-something-as-..." data-toc-modified-id="Что-значит-запись-import-something-as-...-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>Что значит запись <code>import something as ...</code></a></span></li><li><span><a href="#Как-использовать-то,-что-мы-импортировали?" data-toc-modified-id="Как-использовать-то,-что-мы-импортировали?-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>Как использовать то, что мы импортировали?</a></span></li></ul></div>

# Импортирование и использование библиотек

Вы уже наверное встречали такой код:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from scipy import stats
```

Так в Pyhton импортируют библиотеки для дальнейшего использования. 
Эти команды аналогичны ```library(Package)``` in R. 

Основное отличие импорта в Python заключается в том, что чаще всего мы импортируем не все функции из библиотеки, как по умолчанию в R, а только отдельные "модули" (кстати, именно так на самом деле и называются "python-module") и обращаемся к ним за функциями и данными. Это, в первую очередь, позволяет нам всегда знать, откуда взялась используемая нами функция.

# Что значит запись `import something as ...`

Запись `as ..` означает, что вы хотите дать импортируемому модулю или функции, или данным, или объектам имя, которое вам удобнее использовать. Фактически вы создаете некую переменную, значением которой является то, что вы импортируете.

Имя, которое вы выбираете и записываете после `as ..`, обычно называется "псевдоним импорта" ("import alias"). Часто используемые библиотеки обычно имеют традиционные псевдонимы, как в приведенном выше примере. Именно поэтому мы чаще всего видим, что эти библиотеки импортируются таким образом, но это не значит, что вы обязательно должны импортировать их таким образом. 


```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from scipy import stats
```

# Как использовать то, что мы импортировали?

Чтобы импортировать класс или функцию из модуля, мы используем оператор `.`. aka DOT. Это и правда ТОЧКА:

```python
pd + . + function name ->
```

```python
pd.read_csv()
pd.DataFrame()
np.log()
plt.plot()
stats.mannwhitneyu()
```


```python

```
