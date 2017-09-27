#FineHTML
Листиг HTML кода. Основан на [PrismJs](http://prismjs.com/).
## Установка
1. Создать HTML-код модуль. В поле **Заголовок** указать **FineHTML**;
2. Наполнить модуль содержимым *FineHTML.html*;
3. Загрузить на сервер *FineHTML.js*;
4. В конце тела модуля изменить путь до *FineHTML.js*:

```html
...
<script type="text/javascript" src="/templates/template/another/path/FineHTML.js" defer></script>
...
```

## Использование
Наша цель получить такой листинг:
```html
<div class="HTML-code">Module name is FineHTML</div>
```
Необходимо воспользоваться следующим:
```html
{lоadmodule mod_custom,FineHTML} <!-- Подключение модуля FineHTML -->
<pre class="line-numbers"> <!-- Обертка нумерации строк -->
<code class="language-markup"> <!-- Оберка подсветки ЯПа "markup(html)" -->
<!-- Тут то, что нам нужно вывести-->
<div class="HTML-code">Module name is FineHTML</div>
</code></pre>
```