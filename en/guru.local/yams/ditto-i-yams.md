
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<h2>Yams: Ditto и YAMS</h2>

<p>С Ditto обстоит намного сложней, но без него никуда.</p>
<p>К вызову Ditto нужно подключать расширение:</p>
<pre class="brush: html;">&extenders=`@FILE assets/modules/yams/yams.extender.inc.php`</pre>
<p>Если вызов некэшируемый [!Ditto!], то в параметрах вызова надо указывать id и язык:</p>
<pre class="brush: html;">&id=`(yams_id)` &language=`(yams_mname)`</pre>
<p>А в шаблоне плейсхолдеры указываются тогда так:</p>
<pre class="brush: html;">[+(yams_id)_pagetitle+].</pre>
<p>Если вызов кэшируемый [[Ditto]], то автор предлагает поместить в каждый язык по вызову Ditto, также в вызове прописать &id=`id` &language=`имя языка`.</p>
<p>И третий способ по пути наименьшего сопротивления, расширение подключать не нужно, в вызове Ditto чанк с шаблоном имеет окончание соответствующее языку:</p>
<pre class="brush: html;">[[Ditto? &tpl=`news_(yams_id)`]]</pre>
<p>Существует два чанка news_ru, news_en. В зависимости от того, какой язык текущий, параметр (yams_id) подменяется обозначением языка.</p>
<p>А в самих чанках:</p>
<pre class="brush: html;">&lt;h1>[+introtext_ru+]&lt;/h1>&lt;p>[+content_ru+]&lt;/p></pre>
<p>Это прямой вызов TV-параметров, заменивших встроенные поля.</p>
<p>Неудобен этот способ тем, что нужно создавать большое количество чанков, но работает без осечек, с некоторыми сниппетами, например, eForm-ом иначе и не получится.</p>
<p>Это общая информация, не вдаваясь в мелкие детали, чтобы собрать мультиязычный сайт её вполне достаточно.</p>
<p>Сначала пришлось набить шишек и довольно много с ним помучиться, тем более, что версии постарше не работали так, как нужно, но после нескольких осечек, уже проще разобраться, как работает YAMS и использовать его совершенно не проблематично.</p>