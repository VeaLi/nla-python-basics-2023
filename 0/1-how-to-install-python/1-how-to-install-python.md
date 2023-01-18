<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Как-мне-установить-Python?" data-toc-modified-id="Как-мне-установить-Python?-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Как мне установить Python?</a></span><ul class="toc-item"><li><span><a href="#Я-установливаю-Python-с-python.org" data-toc-modified-id="Я-установливаю-Python-с-python.org-1.1"><span class="toc-item-num">1.1&nbsp;&nbsp;</span>Я установливаю Python с python.org</a></span><ul class="toc-item"><li><span><a href="#Как-запустить-.py-скрипт?" data-toc-modified-id="Как-запустить-.py-скрипт?-1.1.1"><span class="toc-item-num">1.1.1&nbsp;&nbsp;</span>Как запустить .py скрипт?</a></span></li><li><span><a href="#Как-запустить-.ipynb----Python-код-из-Jupyter-Notebook?" data-toc-modified-id="Как-запустить-.ipynb----Python-код-из-Jupyter-Notebook?-1.1.2"><span class="toc-item-num">1.1.2&nbsp;&nbsp;</span>Как запустить .ipynb -  Python код из Jupyter Notebook?</a></span><ul class="toc-item"><li><span><a href="#У-меня-не-установлен-Jupyter-Notebook?" data-toc-modified-id="У-меня-не-установлен-Jupyter-Notebook?-1.1.2.1"><span class="toc-item-num">1.1.2.1&nbsp;&nbsp;</span>У меня не установлен Jupyter Notebook?</a></span></li></ul></li></ul></li><li><span><a href="#Я-установливаю-Python-используя-дистрибьютив-Anaconda-(miniconda)" data-toc-modified-id="Я-установливаю-Python-используя-дистрибьютив-Anaconda-(miniconda)-1.2"><span class="toc-item-num">1.2&nbsp;&nbsp;</span>Я установливаю Python используя дистрибьютив Anaconda (miniconda)</a></span><ul class="toc-item"><li><span><a href="#Как-запустить-.py-скрипт?" data-toc-modified-id="Как-запустить-.py-скрипт?-1.2.1"><span class="toc-item-num">1.2.1&nbsp;&nbsp;</span>Как запустить .py скрипт?</a></span></li><li><span><a href="#Как-запустить-.ipynb----Python-код-из-Jupyter-Notebook?" data-toc-modified-id="Как-запустить-.ipynb----Python-код-из-Jupyter-Notebook?-1.2.2"><span class="toc-item-num">1.2.2&nbsp;&nbsp;</span>Как запустить .ipynb -  Python код из Jupyter Notebook?</a></span></li></ul></li><li><span><a href="#Я-пока-не-готов-установть-Python---я-использую-Google-Collab" data-toc-modified-id="Я-пока-не-готов-установть-Python---я-использую-Google-Collab-1.3"><span class="toc-item-num">1.3&nbsp;&nbsp;</span>Я пока не готов установть Python - я использую Google Collab</a></span><ul class="toc-item"><li><span><a href="#Как-запустить-.ipynb----Python-код-из-Jupyter-Notebook?" data-toc-modified-id="Как-запустить-.ipynb----Python-код-из-Jupyter-Notebook?-1.3.1"><span class="toc-item-num">1.3.1&nbsp;&nbsp;</span>Как запустить .ipynb -  Python код из Jupyter Notebook?</a></span></li></ul></li></ul></li><li><span><a href="#У-меня-возникают-трудности-с-установкой-Python-и-запуском-Jupyter-Notebook" data-toc-modified-id="У-меня-возникают-трудности-с-установкой-Python-и-запуском-Jupyter-Notebook-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>У меня возникают трудности с установкой Python и запуском Jupyter Notebook</a></span></li></ul></div>

# Как мне установить Python?

## Я установливаю Python с python.org

Вы, вероятно, хотя бы раз устанавливали Python с сайта [python.org](https://www.python.org/). 
После установки у вас появилась IDLE, и теперь вы можете запускать скрипты с расширением .py с помощью python(.exe).
Возможно, вы не знаете, что делать дальше?

### Как запустить .py скрипт?

Запуск написанной вами программы из командной строки:

```bash
>python script.py
```

### Как запустить .ipynb -  Python код из Jupyter Notebook?

Просмотр Jupyter Notebook:

```bash
>jupyter notebook
```

#### У меня не установлен Jupyter Notebook?

Установите Jupyter Notebook:
```bash
>pip install jupyter
```

## Я установливаю Python используя дистрибьютив Anaconda (miniconda)



Вашим выбором для установки Python стал бесплатный дистрибутив Anaconda - специально разработанный для установки Python, и сопутствующих библиотек для анализа данных. Важно отметить, что Anaconda - это не только удобный дистрибутив, но и менеджер сред. Установив Python с помощью Anaconda, вы можете создавать виртуальные среды с разными версиями Python и разными версиями библиотек, использовать ядро R вместе с Python, а также использовать Python для установки различных биоинформатических инструментов. Например, https://anaconda.org/bioconda/mafft. 

[Установить Python с Anaconda - miniconda](https://docs.conda.io/en/latest/miniconda.html)

### Как запустить .py скрипт?

Запуск написанной вами программы из командной строки:

```bash
>python script.py
```

### Как запустить .ipynb -  Python код из Jupyter Notebook?

Просмотр Jupyter Notebook:

```bash
>jupyter notebook
```


## Я пока не готов установть Python - я использую Google Collab

[Google Collab](https://colab.research.google.com/), уникальный бесплатный сервис от Google, предоставляет пользователю виртуальную машину для запуска Jupyter Notebook. По собственному опыту могу сказать, что использование бесплатной версии Google Collab позволяет решить многие проблемы. Она не так удобна, как локальная версия, и не обладает высокой производительностью, но ее вполне достаточно, чтобы познакомиться с Python для анализа данных.


### Как запустить .ipynb -  Python код из Jupyter Notebook?

Просмотр блокнота Jupyter Notebook:

Загрузите файл с расширением .ipynb на страницу сервиса [Google Collab] (https://colab.research.google.com/) или загрузите .ipynb на Google Диск и дважды щелкните по нему.
Подсказка, для организации работы с Google Collab удобно создавать папки на Google Диске, Google Collab имеет возможность записи-чтения с Google Диска. NB! результаты вашей работы в Google Collab не сохранятся автоматически! Также перед началом работы с Google Collab необходимо убедиться, что политика конфиденциальности данных вашей компании позволяет вам его использовать.

# У меня возникают трудности с установкой Python и запуском Jupyter Notebook

Спроси у меня!
