#finePHP
Листиг PHP кода. Основан на [PrismJs](http://prismjs.com/).
## Установка
1. Создать HTML-код модуль. В поле **Заголовок** указать **finePHP**;
2. Наполнить модуль содержимым *finePHP.html*;
3. Загрузить на сервер *finePHP.js* и *finePHP.css*;
4. В тела модуля изменить пути до *finePHP.js* и *finePHP.css*:

```html
...
<script type="text/javascript">
...
		.setAttribute("href", '/templates/template/another/path/finePHP.css');
...
</script>
...
<script type="text/javascript" src="/templates/template/another/path/finePHP.js" defer></script>
...
```

## Использование
Наша цель получить такой листинг:
```php
<?php
...
this_function_very_major();
...
?>
```
Необходимо воспользоваться следующим:
```html
{lоadmodule mod_custom, finePHP} <!-- Подключение модуля finePHP -->
<pre class="line-numbers"> <!-- Обертка нумерации строк -->
	<code class="language-php"> <!-- Оберка подсветки ЯПа "php" -->
<!-- Тут то, что нам нужно вывести-->
		<?php
		...
		this_function_very_major();
		...
		?>
	</code>
</pre>
```