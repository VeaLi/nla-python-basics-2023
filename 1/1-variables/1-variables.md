<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Переменные-(Variables)" data-toc-modified-id="Переменные-(Variables)-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Переменные (Variables)</a></span></li><li><span><a href="#NB!-Python---динамически-типизированный-язык,-и-он-не-требует-специального-объявления-переменной-с-типом-данных" data-toc-modified-id="NB!-Python---динамически-типизированный-язык,-и-он-не-требует-специального-объявления-переменной-с-типом-данных-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>NB! Python - динамически типизированный язык, и он не требует специального объявления переменной с типом данных</a></span></li><li><span><a href="#В-Python---всё-является-объектом" data-toc-modified-id="В-Python---всё-является-объектом-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>В Python - всё является объектом</a></span><ul class="toc-item"><li><span><a href="#Отличительные-черта-&quot;объекта&quot;---метаданные-и-встроенная-функциональность" data-toc-modified-id="Отличительные-черта-&quot;объекта&quot;---метаданные-и-встроенная-функциональность-3.1"><span class="toc-item-num">3.1&nbsp;&nbsp;</span>Отличительные черта "объекта" - метаданные и встроенная функциональность</a></span></li><li><span><a href="#Как-узнать,-какие-метаданные-и-функциональность-есть-у-моего-объекта?" data-toc-modified-id="Как-узнать,-какие-метаданные-и-функциональность-есть-у-моего-объекта?-3.2"><span class="toc-item-num">3.2&nbsp;&nbsp;</span>Как узнать, какие метаданные и функциональность есть у моего объекта?</a></span></li></ul></li><li><span><a href="#Сложные-объекты" data-toc-modified-id="Сложные-объекты-4"><span class="toc-item-num">4&nbsp;&nbsp;</span>Сложные объекты</a></span></li></ul></div>

# Переменные (Variables)


Переменные  - это __имена__ объектов. Мы используем переменные для управления объектами. Значение переменной - может изменяться в зависимости от условий или информации программы. 


```python
a = 5 # Переменная а, очень простая
b = 5 # Переменная b, очень простая

c = a + b # Простую переменную а можно сложить с b, очень простая переменная с
c
```




    10



# NB! Python - динамически типизированный язык, и он не требует специального объявления переменной с типом данных

Имя "a" можно дать любому объекту, для дальнейшего удобства использования без указания типа данных переменной.

~int a~, ~float a~, ~str a~ etc.


```python
a = 1 # целое число
a = 1.5 # вещественное число
a = 1.5j # мнимое число
a = 2**10 # числовое выражение
a = 'nla' # строка
a = round # функция
a = a # другая переменная
a = object # какой-то базовый объект

a
```




    object



# В Python - всё является объектом

> "In Python - everything is an object"

Числовую переменную "a" можно назвать относительно простой переменной. Она позволяет нам ссылаться на число, которое в ней содержится. 

Интересно, что в Python все даже простые числа являются объектами.

Точнее говоря, в Python __все_ является объектом! 

## Отличительные черта "объекта" - метаданные и встроенная функциональность 
Каждый объект имеет некоторые метаданные (называемые атрибутами или свойствами) и связанные с ними функциональные возможности (называемые методами).

Например, объявим переменную `a='nla'`. Теперь переменная `a' содержит строку. Но теперь мы знаем, что `a' не только содержит строку, но и является объектом, поэтому она содержит метаданные о себе и обладает встроенная функциональностью!


## Как узнать, какие метаданные и функциональность есть у моего объекта?

Самый простой способ узнать больше о своем объекте - прочитать отрывок из документации, из которой вы скопировали свой код).

Но вы также можете распечатать все "свойства" объекта с помощью команды "dir".


```python
a = 'nla'
print(dir(a))
```

    ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isalnum', 'isalpha', 'isascii', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric', 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'maketrans', 'partition', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']
    

Как видно из ячейки выше, строковые объекты в Python, включая тот, который мы создали и записали в переменную 'a', имеют множество "свойств". Мы не будем сейчас проверять все из них. Рассмотрим 4, на мой взгляд, самых полезных:


```python
a.upper()
```




    'NLA'




```python
a = ' nla'
a.strip()
```




    'nla'




```python
a.replace('n', 'J')
```




    ' Jla'




```python
a = 'sentence to split'
a.split(' ')
```




    ['sentence', 'to', 'split']



# Сложные объекты

Как уже говорилось выше, в Python все является объектом, а сам Python не требует сложного объявления переменных для работы. Поэтому вы можете записать в переменную "a" и одно маленькое число, и результат статистического анализа!


```python
import seaborn as sns
import numpy as np

a = sns.histplot(np.random.normal(size=200));
```


    
![png](output_13_0.png)
    



```python
print(dir(a))
```

    ['ArtistList', '_PROPERTIES_EXCLUDED_FROM_SET', '__class__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getstate__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__module__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__setstate__', '__sizeof__', '__str__', '__subclasshook__', '__weakref__', '_add_text', '_adjustable', '_agg_filter', '_alias_map', '_alpha', '_anchor', '_animated', '_aspect', '_autoscaleXon', '_autoscaleYon', '_autotitlepos', '_axes', '_axes_class', '_axes_locator', '_axis_names', '_axisbelow', '_box_aspect', '_callbacks', '_check_no_units', '_children', '_clipon', '_clippath', '_cm_set', '_colorbars', '_convert_dx', '_current_image', '_default_contains', '_deprecate_noninstance', '_facecolor', '_fill_between_x_or_y', '_frameon', '_gci', '_gen_axes_patch', '_gen_axes_spines', '_get_axis_list', '_get_axis_map', '_get_clipping_extent_bbox', '_get_lines', '_get_pan_points', '_get_patches_for_fill', '_get_view', '_gid', '_gridOn', '_in_layout', '_init_axis', '_label', '_label_outer_xaxis', '_label_outer_yaxis', '_left_title', '_make_twin_axes', '_mouseover', '_mouseover_set', '_navigate', '_navigate_mode', '_originalPosition', '_parse_scatter_color_args', '_path_effects', '_pcolor_grid_deprecation_helper', '_pcolorargs', '_picker', '_position', '_prepare_view_from_bbox', '_process_unit_info', '_projection_init', '_quiver_units', '_rasterization_zorder', '_rasterized', '_remove_legend', '_remove_method', '_request_autoscale_view', '_right_title', '_sci', '_set_alpha_for_array', '_set_artist_props', '_set_gc_clip', '_set_lim_and_transforms', '_set_position', '_set_title_offset_trans', '_set_view', '_set_view_from_bbox', '_shared_axes', '_sharex', '_sharey', '_sketch', '_snap', '_stale', '_stale_viewlims', '_sticky_edges', '_subplotspec', '_tight', '_transform', '_transformSet', '_twinned_axes', '_unit_change_handler', '_unstale_viewLim', '_update_image_limits', '_update_line_limits', '_update_patch_limits', '_update_set_signature_and_docstring', '_update_title_position', '_update_transScale', '_url', '_use_sticky_edges', '_validate_converted_limits', '_viewLim', '_visible', '_xaxis_transform', '_xmargin', '_yaxis_transform', '_ymargin', 'acorr', 'add_artist', 'add_callback', 'add_child_axes', 'add_collection', 'add_container', 'add_image', 'add_line', 'add_patch', 'add_table', 'angle_spectrum', 'annotate', 'apply_aspect', 'arrow', 'artists', 'autoscale', 'autoscale_view', 'axes', 'axhline', 'axhspan', 'axis', 'axison', 'axline', 'axvline', 'axvspan', 'bar', 'bar_label', 'barbs', 'barh', 'bbox', 'boxplot', 'broken_barh', 'bxp', 'callbacks', 'can_pan', 'can_zoom', 'change_geometry', 'child_axes', 'cla', 'clabel', 'clear', 'clipbox', 'cohere', 'collections', 'containers', 'contains', 'contains_point', 'contour', 'contourf', 'convert_xunits', 'convert_yunits', 'csd', 'dataLim', 'drag_pan', 'draw', 'draw_artist', 'end_pan', 'errorbar', 'eventplot', 'figbox', 'figure', 'fill', 'fill_between', 'fill_betweenx', 'findobj', 'fmt_xdata', 'fmt_ydata', 'format_coord', 'format_cursor_data', 'format_xdata', 'format_ydata', 'get_adjustable', 'get_agg_filter', 'get_alpha', 'get_anchor', 'get_animated', 'get_aspect', 'get_autoscale_on', 'get_autoscalex_on', 'get_autoscaley_on', 'get_axes_locator', 'get_axisbelow', 'get_box_aspect', 'get_children', 'get_clip_box', 'get_clip_on', 'get_clip_path', 'get_cursor_data', 'get_data_ratio', 'get_default_bbox_extra_artists', 'get_facecolor', 'get_fc', 'get_figure', 'get_frame_on', 'get_geometry', 'get_gid', 'get_gridspec', 'get_images', 'get_in_layout', 'get_label', 'get_legend', 'get_legend_handles_labels', 'get_lines', 'get_navigate', 'get_navigate_mode', 'get_path_effects', 'get_picker', 'get_position', 'get_rasterization_zorder', 'get_rasterized', 'get_renderer_cache', 'get_shared_x_axes', 'get_shared_y_axes', 'get_sketch_params', 'get_snap', 'get_subplotspec', 'get_tightbbox', 'get_title', 'get_transform', 'get_transformed_clip_path_and_affine', 'get_url', 'get_visible', 'get_window_extent', 'get_xaxis', 'get_xaxis_text1_transform', 'get_xaxis_text2_transform', 'get_xaxis_transform', 'get_xbound', 'get_xgridlines', 'get_xlabel', 'get_xlim', 'get_xmajorticklabels', 'get_xminorticklabels', 'get_xscale', 'get_xticklabels', 'get_xticklines', 'get_xticks', 'get_yaxis', 'get_yaxis_text1_transform', 'get_yaxis_text2_transform', 'get_yaxis_transform', 'get_ybound', 'get_ygridlines', 'get_ylabel', 'get_ylim', 'get_ymajorticklabels', 'get_yminorticklabels', 'get_yscale', 'get_yticklabels', 'get_yticklines', 'get_yticks', 'get_zorder', 'grid', 'has_data', 'have_units', 'hexbin', 'hist', 'hist2d', 'hlines', 'ignore_existing_data_limits', 'images', 'imshow', 'in_axes', 'indicate_inset', 'indicate_inset_zoom', 'inset_axes', 'invert_xaxis', 'invert_yaxis', 'is_first_col', 'is_first_row', 'is_last_col', 'is_last_row', 'is_transform_set', 'label_outer', 'legend', 'legend_', 'lines', 'locator_params', 'loglog', 'magnitude_spectrum', 'margins', 'matshow', 'minorticks_off', 'minorticks_on', 'mouseover', 'name', 'numCols', 'numRows', 'patch', 'patches', 'pchanged', 'pcolor', 'pcolorfast', 'pcolormesh', 'phase_spectrum', 'pick', 'pickable', 'pie', 'plot', 'plot_date', 'properties', 'psd', 'quiver', 'quiverkey', 'redraw_in_frame', 'relim', 'remove', 'remove_callback', 'reset_position', 'scatter', 'secondary_xaxis', 'secondary_yaxis', 'semilogx', 'semilogy', 'set', 'set_adjustable', 'set_agg_filter', 'set_alpha', 'set_anchor', 'set_animated', 'set_aspect', 'set_autoscale_on', 'set_autoscalex_on', 'set_autoscaley_on', 'set_axes_locator', 'set_axis_off', 'set_axis_on', 'set_axisbelow', 'set_box_aspect', 'set_clip_box', 'set_clip_on', 'set_clip_path', 'set_facecolor', 'set_fc', 'set_figure', 'set_frame_on', 'set_gid', 'set_in_layout', 'set_label', 'set_navigate', 'set_navigate_mode', 'set_path_effects', 'set_picker', 'set_position', 'set_prop_cycle', 'set_rasterization_zorder', 'set_rasterized', 'set_sketch_params', 'set_snap', 'set_subplotspec', 'set_title', 'set_transform', 'set_url', 'set_visible', 'set_xbound', 'set_xlabel', 'set_xlim', 'set_xmargin', 'set_xscale', 'set_xticklabels', 'set_xticks', 'set_ybound', 'set_ylabel', 'set_ylim', 'set_ymargin', 'set_yscale', 'set_yticklabels', 'set_yticks', 'set_zorder', 'sharex', 'sharey', 'specgram', 'spines', 'spy', 'stackplot', 'stairs', 'stale', 'stale_callback', 'start_pan', 'stem', 'step', 'sticky_edges', 'streamplot', 'table', 'tables', 'text', 'texts', 'tick_params', 'ticklabel_format', 'title', 'titleOffsetTrans', 'transAxes', 'transData', 'transLimits', 'transScale', 'tricontour', 'tricontourf', 'tripcolor', 'triplot', 'twinx', 'twiny', 'update', 'update_datalim', 'update_from', 'update_params', 'use_sticky_edges', 'viewLim', 'violin', 'violinplot', 'vlines', 'xaxis', 'xaxis_date', 'xaxis_inverted', 'xcorr', 'yaxis', 'yaxis_date', 'yaxis_inverted', 'zorder']
    


```python
a.spines # attribute or property
```




    <matplotlib.spines.Spines at 0x21c788d92e0>




```python
a.set_title('New Title') # method
```




    Text(0.5, 1.0, 'New Title')


