
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<h2>ManagerManager: Виджеты</h2>

<h3 class="sub-header text-bold"><a id="312"></a>Ограничение ввода данных</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="313"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse313"><span class="text-bold">mm_ddMaxLength</span> - ограничить количество вводимых символов в TV</a></h4>
</div>
<div id="collapse313" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_ddMaxLength1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_ddMaxLength1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddMaxLength($fields, $roles, $templates, $length)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>length</td>
<td colspan="1">Максимальное количество символов, которые можно ввести.</td>
<td>{integer}</td>
<td>150</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Подключение виджета для TV «Slogan», ограничив количество вводимых символов до 140</p>
<pre class="brush: html;">mm_ddMaxLength('Slogan', '', '', 140);</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="314"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse314"><span class="text-bold">mm_ddNumericFields</span> - ввод в TV только цифр</a></h4>
</div>
<div id="collapse314" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddNumericFields($tvs, $roles, $templates, $allowFloat, $decimals)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tvs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена TV, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение –&nbsp;все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>allowFloat</td>
<td colspan="1">Можно ли вводить числа с плавающей запятой?</td>
<td>{0; 1}</td>
<td>1</td>
</tr>
<tr>
<td>decimals</td>
<td colspan="1">Количество цифр после запятой (0 –&nbsp;любое).</td>
<td>{integer}</td>
<td>0</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Сделать возможным ввод только цифр с точностью в 2 знака после запятой в TV «price» для шаблонов c id, равным 15 или 16 и всех ролей</p>
<pre class="brush: html;">mm_ddNumericFields('price', '', '15,16', 1, 2);</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="315"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse315"><span class="text-bold">mm_hideTemplates</span> - скрыть необходимые шаблоны из списка на странице редактирования документа</a></h4>
</div>
<div id="collapse315" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_hideTemplates($tplIds, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tplIds <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id шаблонов, которые необходимо скрыть из списка.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Скрыть шаблоны с id = 0 и 4 из списка во всех документах для пользователей с id роли = 1</p>
<pre class="brush: html;">mm_hideTemplates('0,4', '1');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="911"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse911"><span class="text-bold">mm_hideFields</span> - скрывать поля документа или TV</a></h4>
</div>
<div id="collapse911" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_hideFields($fields, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые необходимо скрыть.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Скрыть поле «псевдоним» у документов с id шаблона = 3 для пользователей с id роли = 1</p>
<pre class="brush: html;">mm_hideFields('alias', '1', '3');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="912"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse912"><span class="text-bold">mm_ddReadonly</span> - сделать поля документа и TV доступными только для чтения</a></h4>
</div>
<div id="collapse912" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_ddReadonly1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_ddReadonly1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddReadonly($fields, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Значения отображаются при редактировании, но их невозможно изменить. </p>
<p>Довольно редко, но иногда бывают случаи, когда мы храним какую-то информацию о документе в его TV (например, количество просмотров или скачиваний, рейтинг и т.д.). Такая информация обновляется автоматически (какой-нибудь сниппет/плагин просто сохраняет значение в TV соответствующего документа). И вот Петя вдруг решил отредактировать текст документа: открыл, начал писать, его отвлекли по работе, потом позвонили, потом срочно пришлось уехать, два часа ездил, вернулся, продолжил редактировать. Всё это время документ у него был открыт, данные о количестве скачиваний уже 100 раз успели поменяться (было 3, а стало 33), но у Пети до сих пор отображается 3. Петя закончил свою работу, нажимает «Сохранить» и… количество скачиваний перезаписывается на 3! Неприятная ситуация. Что можно сделать? Вариант 1: можно сделать какую-нибудь супер-системную группу и выставить её для тех TV, значения которых не должны редактироваться пользователями. Неплохой вариант, но не надёжный (может найтись кто-то, кто поставит себе эту группу и обязательно что-то испортит) и не подходит, если хочется видеть эти данные при редактировании документа. Именно для таких случаев и предназначен этот виджет.</p>
<p>Работа виджета делится на 3 части:</p>
<p>Перед сохранением документа OnBeforeDocFormSave) получаются и запоминаются актуальные значения необходимых полей (из базы).</p>
<p>После сохранения (OnDocFormSave) записываются обратно.</p>
<p>JS делает поля визуально не редактируемыми.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые необходимо сделать доступными только для чтения.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Сделать поле TV «myVar» доступным только для чтения для пользователей с id роли = 2</p>
<pre class="brush: html;">mm_ddReadonly('myVar', '2');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="128"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse128"><span class="text-bold">mm_requireFields</span> - сделать поля документа или TV обязательными для заполнения</a></h4>
</div>
<div id="collapse128" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_requireFields($fields, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Добавляет звёздочку красного цвета рядом с именем обязательного для заполнения поля, выдаёт сообщение при попытке сохранить не заполнив обязательные поля, предотвращая сохранение.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые должны быть обязательными.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Сделать обязательным для заполнения заголовки и даты публикации всех документов</p>
<pre class="brush: html;">mm_requireFields('pagetitle,pub_date');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="316"></a>Установка необходимых значений</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="317"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse317"><span class="text-bold">mm_inherit</span> - наследовать значения полей или TV от родителей для новых документов/папок</a></h4>
</div>
<div id="collapse317" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_inherit($fields, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые необходимо наследовать.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Выставлять всем новым документам заголовок как у родителя для пользователей с id ролью = 0 или 1</p>
<pre class="brush: html;">mm_inherit('pagetitle', '0,1');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="318"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse318"><span class="text-bold">mm_default</span> - задать значения по умолчанию для полей/TV новых документов/папок</a></h4>
</div>
<div id="collapse318" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_default($fields, $value, $roles, $templates, $eval)</p>
<p><span class="text-bold">Описание параметров:</span> Сейчас TV задаются как «tvN», где N – id TV.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), для которых необходимо установить значение по умолчанию.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>value</td>
<td colspan="1">Значение по умолчанию. Если в качестве поля указано «pub_date»&nbsp;или «unpup_date», а значение пустое, то выставится текущая дата. Также значение может являться строкой PHP-кода, который будет выполнен при параметре «eval» = true.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>eval</td>
<td colspan="1">Необходимо ли обрабатывать значение параметра «value»&nbsp;как PHP-код?</td>
<td>{bollean}</td>
<td>false</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Автоматически выставлять дату отмены публикации спустя 4 недели от текущей для документов с id шаблона = 4</p>
<pre class="brush: html;">mm_default('unpub_date', 'return date("d-m-Y H:i:s", now()+(60*60*24*28));', '', '4', true);</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="913"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse913"><span class="text-bold">mm_ddSetFieldValue</span> - жёстко устанавливать необходимые значения полям документа или TV</a></h4>
</div>
<div id="collapse913" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddSetFieldValue($fields, $value, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Похож на mm_default, но выставляет всегда.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена полей документа или TV, для которых необходимо установить значение.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>value</td>
<td colspan="1">Значение, которое необходимо установить.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> У документов с шаблонами id = 1 и 3 выставить значение TV «someTv» в 'this is some' для редакторов (роль с id = 2)</p>
<pre class="brush: html;">mm_ddSetFieldValue('someTv', 'this is some', '2', '1,3');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="914"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse914"><span class="text-bold">mm_synch_fields</span> - синхронизировать значения полей документа (или TV) при редактировании</a></h4>
</div>
<div id="collapse914" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_synch_fields($fields, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Например: чтобы заголовок и пункт меню документа были одинакомыми, – особенно удобно, когда одно из полей скрыто. Работает только с текстовыми полями (input, textarea).</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые необходимо синхронизировать. Необходимо задать минимум 2 поля.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Сделать значения этих полей всегда одинаковыми (для всех пользователей и документов)</p>
<pre class="brush: html;">mm_synch_fields('pagetitle,menutitle,longtitle');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="319"></a>Изменение названий и подсказок</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="320"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse320"><span class="text-bold">mm_renameField</span> - переименовать одно из стандартных полей документа или TV</a></h4>
</div>
<div id="collapse320" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_renameField($fields, $newlabel, $roles, $templates, $newhelp)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа или TV, которые необходимо переименовать.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">newlabel <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Новый текст для отображения.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>newhelp</td>
<td colspan="1">Новый текст подсказки, всплывающей при наведении на иконку рядом с полем, или описания для TV.</td>
<td>{string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Переименовать поле «заголовок» у документов с id шаблона = 3 для всех пользователей</p>
<pre class="brush: html;">mm_renameField('longtitle', 'ФИО', '', '3');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="915"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse915"><span class="text-bold">mm_changeFieldHelp</span> - изменить текст подсказки, появляющейся при наведении на иконку рядом с полем документа, или описания под TV</a></h4>
</div>
<div id="collapse915" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_changeFieldHelp($field, $helptext, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">field <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поле документа (или TV), у которого необходимо изменить подсказку.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">helptext <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Новый текст подсказки.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Изменить подсказку для поля «псевдоним» у всех документов для пользователей с id роли = 3</p>
<pre class="brush: html;">mm_changeFieldHelp('alias', 'Это последний фрагмент адреса страницы', '3');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="321"></a>Расширение функционала ввода данных</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="322"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse322"><span class="text-bold">mm_ddMultipleFields</span> - добавлять произвольное количество значений полей (TV) к одному документу</a></h4>
</div>
<div id="collapse322" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_ddMultipleFields3.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_ddMultipleFields3.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddMultipleFields($tvs, $roles, $templates, $columns, $columnsTitle, $templates, $colWidth, $splY, $splX, $imgW, $imgH, $minRow, $maxRow, $columnsData)</p>
<p><span class="text-bold">Описание параметров:</span> Значения записываются в одно через необходимые разделители, например: несколько изображений. Возможности:</p>
<p>Добавление к одному документу произвольного количества изображений, текстовых полей, списков (с возможностью выбора значений).</p>
<p>Задание нескольких колонок разных типов (или одинаковых), например: изображения и подписи к ним (параметр «coloumns»).</p>
<p>Вывод заголовков колонок (параметр «coloumnsTitle»).</p>
<p>Количество значений (строк) может быть как фиксированным, динамичным, так и в определённых диапазонах (параметры «minRow» и «maxRow»).</p>
<p>Сортировка (перетаскивание) строк между собой.</p>
<p>Генерация уникального идентификатора каждой строки (параметр «coloumns»).</p>
<p>Вывод предопределённых списков значений (параметры «coloumns» и «coloumnsData»). Внимание, это пока в бете!</p>
<p>Для вывода данных используйте сниппет <a href="ddgetmultiplefield/index.html" target="_blank">ddGetMultipleField</a>.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tvs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена TV, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>columns</td>
<td colspan="1">Типы колонок:
<ul>
<li>field – колонка типа поля;</li>
<li>text – текстовая колонка;</li>
<li>textarea – колонка с многострочным полем;</li>
<li>richtext – колонка с HTML-редактором (TinyMCE);</li>
<li>date – колонка с датой;</li>
<li>id – скрытая колонка с уникальным идентификатором;</li>
<li>select – список с выбором значений (см. параметр «coloumnsData»).</li>
</ul>
</td>
<td>{comma separated string}</td>
<td>'field'</td>
</tr>
<tr>
<td>columnsTitle</td>
<td colspan="1">Заголовки колонок.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>colWidth</td>
<td colspan="1">Ширины колонок (может быть задана одна ширина).</td>
<td>{comma separated string}</td>
<td>180</td>
</tr>
<tr>
<td>splY</td>
<td colspan="1">Разделитель между строками.</td>
<td>{string}</td>
<td>'||'</td>
</tr>
<tr>
<td>splX</td>
<td colspan="1">Разделитель между колонками.</td>
<td>{string}</td>
<td>'::'</td>
</tr>
<tr>
<td>imgW</td>
<td colspan="1">Максимальная ширина превьюшки (для изображений).</td>
<td>{integer}</td>
<td>300</td>
</tr>
<tr>
<td>imgH</td>
<td colspan="1">Максимальная высота превьюшки (для изображений).</td>
<td>{integer}</td>
<td>100</td>
</tr>
<tr>
<td>minRow</td>
<td colspan="1">Минимальное количество строк.</td>
<td>{integer}</td>
<td>0</td>
</tr>
<tr>
<td>maxRow</td>
<td colspan="1">Максимальное количество строк (0 –&nbsp;без лимита).</td>
<td>{integer}</td>
<td>0</td>
</tr>
<tr>
<td>columnsData</td>
<td colspan="1">Список возможных значений для полей в формате json, через ||.</td>
<td>{separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Возможность добавления контактов сотрудников, но не более 5 и не меньше 2, с разными размерами колонок (для текстовой tv «employees»)</p>
<pre class="brush: html;">mm_ddMultipleFields('employees', '', '', 'text,text,text', 'Имя,Телефон,Должность', '250,100,100', '||', '::', 300, 100, 2, 5);</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="323"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse323"><span class="text-bold">mm_ddSelectDocuments</span> - выбор id определённых документов в удобном виде</a></h4>
</div>
<div id="collapse323" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_ddSelectDocuments1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_ddSelectDocuments1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddSelectDocuments($tvs, $roles, $templates, $parentIds, $depth, $filter, $max, $labelMask)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tvs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена TV, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение –&nbsp;все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">parentIds <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id родительских документов, дочерние документы которых необходимо выбирать.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>depth</td>
<td colspan="1">Глубина поиска дочерних документов.</td>
<td>{integer}</td>
<td>1</td>
</tr>
<tr>
<td>filter</td>
<td colspan="1">Условия фильтрации документов (чем-то похож на фильтр Ditto), разделённые через '&' между парами и через '=' между ключом и значением. Например: 'template=15&published=1', – получим только опубликованные документы с id шаблона 15.</td>
<td>{separated string}</td>
<td>–</td>
</tr>
<tr>
<td>max</td>
<td colspan="1">Максимальное количество документов, которое пользователь может выбрать (при == 0 – без ограничений).</td>
<td>{integer}</td>
<td>0</td>
</tr>
<tr>
<td>labelMask</td>
<td colspan="1">Шаблон отображения элемента в списке выбора документов. Задаётся как строка, содержащая плэйсхолдеры с полями документа (и TV). Также доступен дополнительный плэйсхолдер '<span>[</span>+title+]', в который будет подставлено значение поля «menutitle», а если оно не заполнено, то «pagetitle».</td>
<td>{string}</td>
<td>'<span>[</span>+title+] (<span>[</span>+id+])'</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span></p>
<pre class="brush: html;">mm_ddSelectDocuments();</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="324"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse324"><span class="text-bold">mm_widget_tags</span> - добавлять теги к документам в удобной форме</a></h4>
</div>
<div id="collapse324" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_widget_tags1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_widget_tags1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_widget_tags($fields, $delimiter, $source, $display_count, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Для нужной TV автоматически формируется «список» выбора со всеми тегами, при этом, новые теги просто вписываются через разделитель здесь же) на странице редактирования документа.
TV должна быть текстового типа.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">TV, для которых необходимо отобразить теги.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>delimiter</td>
<td colspan="1">Разделитель между тегами в поле</td>
<td>{string}</td>
<td>','</td>
</tr>
<tr>
<td>source</td>
<td colspan="1">TV, из которых должны браться теги для списка выбра. Это позволяет использовать разные поля для ввода тегов и формирования списка выбора. По умолчанию значение берётся из параметра «fields». Не используйте этот параметр, если не уверены.</td>
<td>{comma separated string}</td>
<td>= fields</td>
</tr>
<tr>
<td>display_count</td>
<td colspan="1">Отображать ли в списке выбора количество документов, в которых используется тег (в скобочках после самого тега)?</td>
<td>{boolean}</td>
<td>false</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Сделать для TV «docTags» виджет тегов с отображением количества документов, использующих каждый тег рядом с ним у документов с id шаблона = 2 для всех ролей</p>
<pre class="brush: html;">mm_widget_tags('docTags', ',', '', '1', '', '2');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="325"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse325"><span class="text-bold">mm_widget_colors</span> - добавить инструмент выбора цвета из палитры для необходимой TV</a></h4>
</div>
<div id="collapse325" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_widget_colors1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_widget_colors1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_widget_colors($fields, $default, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Выбранный цвет сохраняется в TV в hex формате. TV должна быть текстового типа.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">TV, для которых необходимо отобразить палитру цветов.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>default</td>
<td colspan="1">Цвет по умолчанию, который будет вставляться при пустом значении в TV (в случае, если значение по умолчанию у TV не задано стандартными средствами MODx).</td>
<td>{string}</td>
<td>'#ffffff'</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Добавить палитру выбора цветов для TV «bgcolor» у документов с id шаблона = 2 для пользователей с id роли = 1 и выставить чёрный цвет по умолчанию</p>
<pre class="brush: html;">mm_widget_colors('bgcolor', '#000000', '1', '2');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="916"></a>Работа с секциями</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="917"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse917"><span class="text-bold">mm_ddCreateSection</span> - создать новую произвольную секцию на странице редактирования документа</a></h4>
</div>
<div id="collapse917" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddCreateSection($title, $id, $tabId, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">title <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Текст заголовка новой секции.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">id <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Уникальный id новой секции.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>tabId</td>
<td colspan="1">Id вкладки, в которую будет вставлена секция. Можно указать как id одной из стандартных вкладок, так и id вкладки, созданной при помощи mm_createTab.</td>
<td>{string}</td>
<td>'general'</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Создать секцию с заголовком «Категории» в основной вкладке у всех документов для всех пользователей</p>
<pre class="brush: html;">mm_ddCreateSection('Категории', 'mycats');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="918"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse918"><span class="text-bold">mm_ddMoveFieldsToSection</span> - переместить поля документа и TV в другую секцию</a></h4>
</div>
<div id="collapse918" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddMoveFieldsToSection($fields, $sectionId, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> К сожалению, невозможно переместить следующие поля: keywords, metatags, which_editor, show_in_menu, menuindex.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые необходимо переместить.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">sectionId <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id секции, в которую необходимо переместить поля. Можно указать как id одной из стандартных секций, так и id секции, созданной при помощи mm_ddCreateSection.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Переместить TV «profilePhoto» в секцию «images» для всех пользователей и шаблонов</p>
<pre class="brush: html;">mm_ddMoveFieldsToSection('profilePhoto', 'images');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="919"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse919"><span class="text-bold">mm_hideSections</span> - скрыть одну из секций на странице редактирования документа</a></h4>
</div>
<div id="collapse919" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_hideSections($sections, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> «Секции» – это такие области на странице редактирования документа, например: «Содержимое ресурса» или «Параметры (TV)».</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">$sections <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Секции, которые необходимо скрыть.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>$roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>$templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Скрыть секции «Содержимое ресурса» и «Параметры (TV)» у документов с id шаблона = 3 для пользователей с id роли = 1</p>
<pre class="brush: html;">mm_hideSections('content,tvs', '1', '3');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="920"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse920"><span class="text-bold">mm_renameSection</span> - переименовать одну из секций на странице редактирования документа</a></h4>
</div>
<div id="collapse920" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_renameSection($section, $newlabel, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> «Секции» – это такие области на странице редактирования документа, например: «Содержимое ресурса» или «Параметры (TV)».</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">$section <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Секция, которую необходимо переименовать.</td>
<td>{'content'; 'tvs'}</td>
<td>–</td>
</tr>
<tr>
<td class="em">$newlabel <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Новый текст заголовка секции.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>$roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>$templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Переименовать секцию контента документа для пользователей с id роли = 2</p>
<pre class="brush: html;">mm_renameSection('content', 'Текстик (отображается на страничке)', '2');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="921"></a>Работа с вкладками</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="922"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse922"><span class="text-bold">mm_createTab</span> - создать новую произвольную вкладку на странице редактирования документа</a></h4>
</div>
<div id="collapse922" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_createTab($name, $id, $roles, $templates, $intro, $width)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">name <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Текст заголовка новой вкладки.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">id <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Уникальный id новой вкладки.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>intro</td>
<td colspan="1">Описание новой вкладки, отображается в самом верху (можно использовать HTML).</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>width</td>
<td colspan="1">Ширина содержимого новой вкладки, можно использовать css значения (например: '100%', '450px', 'auto').</td>
<td>{string}</td>
<td>680</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Создать новую вкладку шириной 450px с описанием у документов с id шаблона = 3 или 4</p>
<pre class="brush: html;">mm_createTab('SEO', 'seoTab', '', '3,4', '  Здесь вы можете отредактировать всё, что касается поисковой оптимизации. ', '450');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="923"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse923"><span class="text-bold">mm_moveFieldsToTab</span> - переместить поля документа и TV в другую вкладку</a></h4>
</div>
<div id="collapse923" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_moveFieldsToTab($fields, $tabId, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> К сожалению, невозможно переместить следующие поля: keywords, metatags, which_editor, show_in_menu, menuindex.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), которые необходимо переместить.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">tabId <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id вкладки, в которую необходимо переместить поля. Можно указать как id одной из стандартных вкладок, так и id вкладки, созданной при помощи mm_createTab.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Переместить дату публикации документа в основную вкладку для пользователей с id роли = 2</p>
<pre class="brush: html;">mm_moveFieldsToTab('pub_date', 'general', '2');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="924"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse924"><span class="text-bold">mm_hideTabs</span> - скрыть одну из стандартных вкладок на странице редактирования документа</a></h4>
</div>
<div id="collapse924" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_hideTabs($tabs, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tabs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id вкладок, которые необходимо скрыть.</td>
<td>{'general'; 'settings'; 'access'}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Скрыть вкладку «Права доступа» у документов с id шаблона = 3 для пользователей с id роли = 1</p>
<pre class="brush: html;">mm_hideTabs('access', '1', '3');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="925"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse925"><span class="text-bold">mm_renameTab</span> - переименовать одну из стандартных вкладок на странице редактирования документа</a></h4>
</div>
<div id="collapse925" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_renameTab($tab, $newlabel, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tab <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id вкладки, которую необходимо переименовать.</td>
<td>{'general'; 'settings'; 'access'}</td>
<td>–</td>
</tr>
<tr>
<td class="em">newlabel <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Новый текст заголовка вкладки.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Переименовать вкладку «Общие» для пользователей с id роли = 2</p>
<pre class="brush: html;">mm_renameTab('general', 'Основное', '2');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="926"></a>Карты</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="927"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse927"><span class="text-bold">mm_ddGMap</span> - интегрировать карту Google Maps для получения координат</a></h4>
</div>
<div id="collapse927" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_ddGMap1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_ddGMap1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddGMap($tvs, $roles, $templates, $w, $h, $hideField)</p>
<p><span class="text-bold">Описание параметров:</span> Начальная позиция карты задаётся очень просто: достаточно указать необходимые координаты в качестве «значения по умолчанию» соответствующей TV.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tvs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена TV, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>w</td>
<td colspan="1">Ширина контейнера с картой.</td>
<td>{'auto'; integer}</td>
<td>'auto'</td>
</tr>
<tr>
<td>h</td>
<td colspan="1">Высота контейнера с картой.</td>
<td>{integer}</td>
<td>400</td>
</tr>
<tr>
<td>hideField</td>
<td colspan="1">Необходимо ли скрывать оригинальное текстовое поле с координатами.</td>
<td>{0; 1}</td>
<td>1</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Подключение виджета Google Maps для TV «LatLng»</p>
<pre class="brush: html;">mm_ddGMap('LatLng');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="928"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse928"><span class="text-bold">mm_ddYMap</span> - интегрировать карту Yandex Maps для получения координат</a></h4>
</div>
<div id="collapse928" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_ddYMap1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_ddYMap1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddYMap($tvs, $roles, $templates, $w, $h, $hideField)</p>
<p><span class="text-bold">Описание параметров:</span> Для простого вывода карты на страницу используйте сниппет <a href="141.html" target="_blank">ddYMap</a>. Начальная позиция карты задаётся очень просто: достаточно указать необходимые координаты в качестве «значения по умолчанию» соответствующей TV.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tvs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена TV, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>w</td>
<td colspan="1">Ширина контейнера с картой.</td>
<td>{'auto'; integer}</td>
<td>'auto'</td>
</tr>
<tr>
<td>h</td>
<td colspan="1">Высота контейнера с картой.</td>
<td>{integer}</td>
<td>400</td>
</tr>
<tr>
<td>hideField</td>
<td colspan="1">Необходимо ли скрывать оригинальное текстовое поле с координатами.</td>
<td>{0; 1}</td>
<td>1</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Подключение виджета Yandex Maps для TV «LngLat»</p>
<pre class="brush: html;">mm_ddYMap('LngLat');</pre>
</div>
</div>
</div>
</div>
<h3 class="sub-header text-bold"><a id="929"></a>Прочее</h3>
<div class="panel-group accordion">
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="930"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse930"><span class="text-bold">mm_widget_showimagetvs</span> - показать превьюшки изображений, выбранных в TV на странице редактирования документа</a></h4>
</div>
<div id="collapse930" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_widget_showimagetvs1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_widget_showimagetvs1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_widget_showimagetvs($fields, $maxWidth, $maxHeight, $thumbnailerUrl, $roles, $templates)</p>
<p><span class="text-bold">Описание параметров:</span> Аналогичен плагину ShowImageTVs, который не совместим с ManagerManager.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td>fields</td>
<td colspan="1">TV, для которых необходимо отобразить превьюшки.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>maxWidth</td>
<td colspan="1">Максимальная ширина превьюшки в px.</td>
<td>{integer}</td>
<td>300</td>
</tr>
<tr>
<td>maxHeight</td>
<td colspan="1">Максимальная высота превьюшки в px.</td>
<td>{integer}</td>
<td>100</td>
</tr>
<tr>
<td>thumbnailerUrl</td>
<td colspan="1">Если у вас установлен PHPThumb, вы можете указать url, где он находится, адрес превью будет обращён к нему с передачей url исходной картинки, ширины и высоты.</td>
<td>{string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Показать превью для TV «mypic» у документов с id шаблона = 2 и отправить за одно на генерацию в phpThumb для получения превьюшек размером 300×200 px</p>
<pre class="brush: html;">mm_widget_showimagetvs('mypic', '300', '200', '/assets/snippets/phpthumb/phpThumb.php', '', '2');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="931"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse931"><span class="text-bold">mm_ddResizeImage</span> - изменять размеры изображений (TV), например: делать маленькие превьюшки (thumbs)</a></h4>
</div>
<div id="collapse931" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddResizeImage($tvs, $roles, $templates, $width, $height, $cropping, $suffix, $replaceFieldVal, $background, $multipleField, $colNum, $splY, $splX, $num, $allowEnlargement)</p>
<p><span class="text-bold">Описание параметров:</span> Виджет срабатывает только в момент сохранения документов (событие «OnBeforeDocFormSave») и не создаёт изображений повторно, что обеспечивает минимальный расход ресурсов сервера.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">tvs <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Имена TV с изображениями, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">width <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Ширина создаваемого изображения в px. Пустое значение –&nbsp;автоматический расчёт исходя из высоты. Обязателен хотя бы один размер.</td>
<td>{integer}</td>
<td>–</td>
</tr>
<tr>
<td class="em">height <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Высота создаваемого изображения в px. Пустое значение –&nbsp;автоматический расчёт исходя из ширины. Обязателен хотя бы один размер.</td>
<td>{integer}</td>
<td>–</td>
</tr>
<tr>
<td>cropping</td>
<td colspan="1">Обрезать ли изображение, пытаясь добиться жесткого соответствия размерам.
<ul>
<li>0 – не обрезать;</li>
<li>1 –&nbsp;просто обрезать (не изменяя масштаб);</li>
<li>'crop_resized' –&nbsp;сначала уменьшить, затем обрезать;</li>
<li>'fill_resized' – пропорционально уменьшить, заполнив образовавшиеся поля цветом («background»).</li>
</ul>
</td>
<td>{0; 1; 'crop_resized'; 'fill_resized'}</td>
<td>'crop_resized'</td>
</tr>
<tr>
<td>suffix</td>
<td colspan="1">Суффикс для имен создаваемых изображений. При пустом значении заменяются исходные изображения!</td>
<td>{string}</td>
<td>'_ddthumb'</td>
</tr>
<tr>
<td>replaceFieldVal</td>
<td colspan="1">Нужно ли переписывать значения в TV на имена созданных изображений (те, что с учётом «suffix»). Не работает при multipleField = 1!</td>
<td>{0; 1}</td>
<td>0</td>
</tr>
<tr>
<td>background</td>
<td colspan="1">Цвет фона (используется при cropping = 'fill_resized').</td>
<td>{string}</td>
<td>'#FFFFFF'</td>
</tr>
<tr>
<td>multipleField</td>
<td colspan="1">Является ли поле множественным (для mm_ddMultipleFields).</td>
<td>{0; 1}</td>
<td>0</td>
</tr>
<tr>
<td>colNum</td>
<td colspan="1">Номер колонки, в которой находится изображение (для mm_ddMultipleFields).</td>
<td>{integer}</td>
<td>0</td>
</tr>
<tr>
<td>splY</td>
<td colspan="1">Разделитель строк (для mm_ddMultipleFields).</td>
<td>{string}</td>
<td>'||'</td>
</tr>
<tr>
<td>splX</td>
<td colspan="1">Разделитель колонок (для mm_ddMultipleFields).</td>
<td>{string}</td>
<td>'::'</td>
</tr>
<tr>
<td>num</td>
<td colspan="1">Номер строки, которую надо обрабатывать (для mm_ddMultipleFields).</td>
<td>{integer; 'all'}</td>
<td>'all'</td>
</tr>
<tr>
<td>allowEnlargement</td>
<td colspan="1">Разрешить увеличение изображения?</td>
<td>{0; 1}</td>
<td>1</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Создать для изображений, выставленных в TV «imageTV», уменьшенные копии, перезаписывая значения в TV</p>
<pre class="brush: html;">mm_ddResizeImage('imageTV', '', '', 200, 100, 'crop_resized', '_ddthumb', 1);</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="932"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse932"><span class="text-bold">mm_ddAutoFolders</span> - при сохранении документа (событие OnBeforeDocFormSave) автоматически перемещать его, основываясь на его дате (дате публикации, или любой дате в tv) в папку года и месяца</a></h4>
</div>
<div id="collapse932" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddAutoFolders($roles, $templates, $yearsParents, $dateSource, $yearFields, $monthFields, $yearPublished, $monthPublished, $numericMonth)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">templates <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td class="em">yearsParents <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">ID корневых родителей (непосредственных родителей документов-лет).</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>dateSource</td>
<td colspan="1">Поле документа, из которого необходимо брать дату.</td>
<td>{string}</td>
<td>'pub_date'</td>
</tr>
<tr>
<td>yearFields</td>
<td colspan="1">Поля документов (и TV), которые необходимо выставить документам-годам. Ассоциативный массив в JSON, где ключ –&nbsp;имя поля, значение –&nbsp;значение.</td>
<td>{string: JSON}</td>
<td>'{"template":0,"published":0}'</td>
</tr>
<tr>
<td>monthFields</td>
<td colspan="1">Поля документов (и TV), которые необходимо выставить документам-месяцам. Ассоциативный массив в JSON, где ключ –&nbsp;имя поля, значение –&nbsp;значение.</td>
<td>{string: JSON}</td>
<td>'{"template":0,"published":0}'</td>
</tr>
<tr>
<td>yearPublished</td>
<td colspan="1"><b>Внимание!</b> Устаревший параметр, используйте «$yearFields». Надо ли публиковать документы-годы?</td>
<td>{0; 1}</td>
<td>–</td>
</tr>
<tr>
<td>monthPublished</td>
<td colspan="1"><b>Внимание!</b> Устаревший параметр, используйте «$monthFields». Надо ли публиковать документы-месяцы?</td>
<td>{0; 1}</td>
<td>–</td>
</tr>
<tr>
<td>numericMonth</td>
<td colspan="1">Нужно ли документам-месяцам делать псевдонимы в виде порядкового номера с ведущим нолём (например: «03»).</td>
<td>{boolean}</td>
<td>false</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span></p>
<pre class="brush: html;">mm_ddAutoFolders();</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="933"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse933"><span class="text-bold">mm_ddFillMenuindex</span> - выставить минимальное свободное значение позиции меню (menuindex) для новых документов</a></h4>
</div>
<div id="collapse933" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddFillMenuindex($parent)</p>
<p><span class="text-bold">Описание параметров:</span> По умолчанию позиция меню в MODx для новых документов просто равна количеству дочерних документов на одном уровне, что не всегда удобно.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td>parent</td>
<td colspan="1">ID документа, для дочерних документов которого должен применяться виджет. Если оставить пустым (не указаывать), то виджет будет применён абсолютно ко всем документам.</td>
<td>{integer; ''}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span></p>
<pre class="brush: html;">mm_ddFillMenuindex();</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="934"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse934"><span class="text-bold">mm_widget_accessdenied</span> - запретить доступ к определённым документам по их ID (доступ к дочерним документам не запрещается)</a></h4>
</div>
<div id="collapse934" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href="assets/images/doc/mm/mm_widget_accessdenied1.jpg.html"><img class="img-thumbnail h140" src="assets/images/doc/mm/mm_widget_accessdenied1.jpg.html" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_widget_accessdenied($ids, $default, $roles)</p>
<p><span class="text-bold">Описание параметров:</span> Например, в родительском документе вызвыается сниппет «Ditto», и вы не хотите, чтобы пользователи редактировали этот документ, но хотите, чтобы пользователи могли создавать и редактировать дочерние документы.</p>
<p>Используйте этот виджет с осторожностью, т.к. он не обеспечивает такой защиты, как встроенная система прав MODx. Пользователь, обладающий техническими знаниями может обойти эту защиту через инструменты для разработки в браузере.</p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">ids <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Список документов, к которым необходимо запретить доступ.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>default</td>
<td colspan="1">Сообщение о запрете доступа (разрешён HTML).</td>
<td>{string}</td>
<td>'Access denied - Access to current document closed for security reasons.'</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span> Запретить доступ к документам с id = 1 и 15 пользователям с id роли = 2 и отобразить произвольное сообщение о запрете доступа</p>
<pre class="brush: html;">mm_widget_accessdenied('1,15', 'Этот документ запрещено редактировать. Давай, до свидания!' '2');</pre>
</div>
</div>
</div>
<div class="panel panel-default">
<div class="panel-heading">
<h4 class="panel-title"><a id="935"></a><a class="accordion-toggle collapsed" data-toggle="collapse" data-parent="#accordion" href="#collapse935"><span class="text-bold">mm_ddHTMLCleaner</span> - очистить лишние атрибуты и стили в HTML для необходимых полей документа (и TV)</a></h4>
</div>
<div id="collapse935" class="panel-collapse collapse">
<div class="panel-body">
<p><a class="fancybox" href=""><img class="img-thumbnail h140" src="" alt=""></a></p>
<p><span class="text-bold">Синтаксис:</span> mm_ddHTMLCleaner($fields, $roles, $templates, $validAttrsForAllTags, $validStyles, $validAttrs)</p>
<p><span class="text-bold">Описание параметров:</span></p>
<div class="flip-scroll">
<table class="table table-bordered table-vcenter flip-content">
<thead class="flip-content bordered-palegreen">
<tr><th>Название</th><th>Описание</th><th>Допустимые значения</th><th>Значение по умолчанию</th></tr>
</thead>
<tbody>
<tr>
<td class="em">fields <span class="help">*<span class="helpPopup"></span></span></td>
<td colspan="1">Поля документа (или TV), для которых необходимо применить виджет.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>roles</td>
<td colspan="1">Роли, для которых необходимо применить виждет, пустое значение – все роли.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>templates</td>
<td colspan="1">Id шаблонов, для которых необходимо применить виджет, пустое значение – все шаблоны.</td>
<td>{comma separated string}</td>
<td>–</td>
</tr>
<tr>
<td>validAttrsForAllTags</td>
<td colspan="1">Разрешённые атрибуты для для всех тегов (атрибуты, которые не нужно удалять, остальные удалятся).</td>
<td>{comma separated string}</td>
<td>'title,class'</td>
</tr>
<tr>
<td>validStyles</td>
<td colspan="1">Разрешённые стили для всех тегов (стили, которые не нужно удалять из атрибута «style»).</td>
<td>{comma separated string}</td>
<td>'word-spacing'</td>
</tr>
<tr>
<td>validAttrs</td>
<td colspan="1">Разрешённые атрибуты для тегов (они не будут удаляться). В качестве ключа используется имя тега, в качестве значения – разрешённые атрибуты (строка, разделённая через запятую).</td>
<td>{string: JSON}</td>
<td>'{"img":"src,alt,width,height","a":"href,target"}'</td>
</tr>
</tbody>
</table>
</div>
<p><span class="text-bold">Пример:</span></p>
<pre class="brush: html;">mm_ddHTMLCleaner();</pre>
</div>
</div>
</div>
</div>