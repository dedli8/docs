
<meta http-equiv="Content-Type" content="text/html; charset=utf-8">
<h2>FormLister: Отправка писем</h2>

<p>Контроллер <span class="text-bold">Form</span> позволяет отправлять данные формы в письме.</p>
<h2 class="page-header">Параметры отправки почты</h2>
<h3 class="sub-header text-bold">isHtml</h3>
<p>Разрешает отправлять письмо в формате html. Проверка корректности кода письма возлагается на разработчика.</p>
<p>Возможные значения - 1, 0.</p>
<p>Значение по умолчанию - 1.</p>
<h3 class="sub-header text-bold">to</h3>
<p>Адрес получателя. Если не указан, то письмо не отправляется, но считается успешно отправленным.</p>
<p>Возможные значения - email-адрес.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">from</h3>
<p>Возможные значения - email-адрес.</p>
<p>Значение по умолчанию - параметр конфигурации emailsender.</p>
<h3 class="sub-header text-bold">fromName</h3>
<p>Имя отправителя.</p>
<p>Возможное значение - строка.</p>
<p>Значение по умолчанию - параметр конфигурации site_name.</p>
<h3 class="sub-header text-bold">replyTo</h3>
<p>Заголовок replyTo.</p>
<p>Возможные значения - email-адрес.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">cc</h3>
<p>Заголовок сс.</p>
<p>Возможные значения - email-адрес.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">bcc</h3>
<p>Заголовок bcc.</p>
<p>Возможные значения - email-адрес.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">noemail</h3>
<p>Если параметр задан, то письмо не отправляется, но считается успешно отправленным.</p>
<p>Возможные значения - 1, 0.</p>
<p>Значение по умолчанию - 0.</p>
<h3 class="sub-header text-bold">ignoreMailerResult</h3>
<p>Если параметр задан, то письмо отправляется, но результат отправки игнорируется.</p>
<p>Возможные значения - 1, 0.</p>
<p>Значение по умолчанию - 0.</p>
<h3 class="sub-header text-bold">subject</h3>
<p>Тема письма.</p>
<p>Возможные значения - строка.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">subjectTpl</h3>
<p>Шаблон темы письма.</p>
<p>Возможные значения - имя шаблона, указанное по правилам задания шаблонов в DocLister.</p>
<p>Значение по умолчанию - значение параметра subject.</p>
<h3 class="sub-header text-bold">autosender</h3>
<p>Адрес на который отправляется дополнительное письмо.</p>
<p>Возможные значения - email-адрес.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">autosenderFromName</h3>
<p>Имя отправителя дополнительного письма.</p>
<p>Возможные значения - строка.</p>
<p>Значение по умолчанию - параметр конфигурации site_name.</p>
<h3 class="sub-header text-bold">ccSender</h3>
<p>Если параметр задан, то на адрес указанный в поле формы отправляется письмо.</p>
<p>Возможные значения - 1, 0.</p>
<p>Значение по умолчанию - 0.</p>
<h3 class="sub-header text-bold">ccSenderField</h3>
<p>Имя поля, в котором хранится адрес получателя.</p>
<p>Возможные значения - имя поля формы.</p>
<p>Значение по умолчанию - email.</p>
<h3 class="sub-header text-bold">ccSenderFromName</h3>
<p>Имя отправителя письма на заданный в поле формы адрес.</p>
<p>Возможные значения - строка.</p>
<p>Значение по умолчанию - не указано.</p>
<h2 class="page-header">Защита от повторной отправки</h2>
<h3 class="sub-header text-bold">protectSubmit</h3>
<p>Защита от повторной отправки письма.</p>
<p>Возможные значения - 1, 0 или список полей, по которым определяется уникальность письма. Если список не задан, то используются поля, обязательные для заполнения.</p>
<p>Значение по умолчанию - 1.</p>
<h3 class="sub-header text-bold">submitLimit</h3>
<p>Защита от частой отправки писем.</p>
<p>Значение - число секунд между повторной отправкой.</p>
<p>Значение по умолчанию - 60.</p>
<h2 class="page-header">Шаблоны</h2>
<h3 class="sub-header text-bold">reportTpl</h3>
<p>Основной шаблон письма.</p>
<p>Возможные значения - имя шаблона, указанное по правилам задания шаблонов в DocLister.</p>
<p>Значение по умолчанию - список полей и их значений.</p>
<h3 class="sub-header text-bold">automessageTpl</h3>
<p>Шаблон дополнительного письма.</p>
<p>Возможные значения - имя шаблона, указанное по правилам задания шаблонов в DocLister.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">ccSenderTpl</h3>
<p>Шаблон письма на заданный в поле формы адрес.</p>
<p>Возможные значения - имя шаблона, указанное по правилам задания шаблонов в DocLister.</p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">successTpl</h3>
<p>Шаблон сообщения об успешной отправке писем.</p>
<p>Возможные значения - имя шаблона, указанное по правилам задания шаблонов в DocLister.</p>
<p>Значение по умолчанию - пусто.</p>
<h2 class="page-header">Отправка файлов</h2>
<h3 class="sub-header text-bold">attachments</h3>
<p>Имена полей, в которых хранятся файлы. Поддерживаются только поля с одним файлом (name="field" type="file") и поля с одномерным массивом файлов (name="field[]" type="file" multiple). </p>
<p>Значение по умолчанию - пусто.</p>
<h3 class="sub-header text-bold">attachFiles</h3>
<p>Позволяет отправить произвольные файлы. </p>
<p>Возможные значения - массив:</p>
<pre class="brush: html;">&amp;attachFiles=`{
"имя поля1":{
	"filepath":"assets/images/logo.png",
	"filename":"logo.png"
},
"имя поля2":[
	{
	"filepath":"assets/images/file1.jpg",
	"filename":"отчет.jpg"
	},
	{
	"filepath":"assets/images/file2.jpg",
	"filename":"отчет2.jpg"
	}
]
}`</pre>
<h3 class="sub-header text-bold">deleteAttachments</h3>
<p>Позволяет удалить файлы вложений после успешной отправки.</p>
<p>Возможные значения - 0 или 1.</p>
<p>Значение по умолчанию - 0.</p>
<h3 class="sub-header text-bold">fileValidator</h3>
<p>Имя класса для валидации файлов. Если задано, то класс должен быть загружен заранее.</p>
<p>Значение по умолчанию - \FormLister\FileValidator</p>
<h3 class="sub-header text-bold">fileRules</h3>
<p>Правила валидации (см. раздел "Валидация данных"). Стандартный валидатор поддерживает правила:</p>
<ul>
<li>required: файлы успешно отправлены;</li>
<li>optional: аналогично required, но выполняется и в том случае, если пользователь не загружал файлы (то есть поле с файлами не является обязательным);</li>
<li>allowed: расширение файла входит в заданный массив;</li>
<li>images: расширение файла jpg, jpeg, gif, png, bmp;</li>
<li>minSize: размер файла в килобайтах больше заданного;</li>
<li>maxSize: размер файла в килобайтах меньше заданного;</li>
<li>sizeBetween: размер файла в килобайтах входит в диапазон;</li>
<li>minCount: количество файлов больше заданного;</li>
<li>maxCount: количество файлов меньше заданного;</li>
<li>countBetween: количество файлов входит в диапазон.</li>
</ul>
<p>Использовать конструкцию "!имя поля" в правилах валидации файлов нет смысла, так как значение поля с файлом не будет пустым, даже если файл не загружен. Следует использовать правило optional.</p>
<p>В шаблоне письма reportTpl доступен плейсхолдер [+attachments.value+] со списком всех приложенных к письму файлов. Можно также вывести по отдельности: [+имя поля.value+]. Файлы отправляются только в письме c шаблоном reportTpl.</p>