# HTML-AND-CSS-BASICS
Test project answers on questions

Ответы на русском языке

Learning Outcomes
Look through these now and then use them to test yourself after doing the assignment:

Why do we separate HTML and CSS?
Разделение HTML и CSS на отдельные файлы делает их лучше кэшируемыми, т.е каждый компонент файла может быть в кэше(область памяти с быстрым доступом, содержащая информацию, которая может быть запрошена с наибольшей вероятностью, используемая для временного хранения данных при вводе или выводе).Доступ к данным в кэше осуществляется быстрее, чем выборка исходных данных из более медленной памяти или удалённого источника, однако её объём существенно ограничен по сравнению с хранилищем исходных данных.Таким образом разделение HTML и CSS на отдельные файлы влияет на время загрузки страницы, чем меньше страница, тем быстрее она загружается. Так же разделение HTML и CSS на отдельные файлы необходимо для лучшей читаемости кода и удобства обслуживания web прилжений.

What are classes and IDs (and how are they different)?
Классы и идентификаторы - это атрибуты тэга.Существенное отличие класса от идентификатора в том, что в коде документа каждый идентификатор уникален и должен быть включён лишь один раз, а классы могут использоваться в коде неоднократно.Классы можно комбинировать между собой, добавляя несколько классов к одному тегу.
 
What are elements?
Элементы HTML — это основная структурная единица веб-страницы, написанная на языке HTML

What are tags?
Тег — элемент языка разметки гипертекста (специальный символ разметки языка HTML)

What are attributes?
У тега могут быть свойства, называемые атрибутами, дающие дополнительные возможности форматирования текста. Они записываются в виде сочетания: имя атрибута="значение", причём текстовые значения заключаются в кавычки.
Все атрибуты состоят из двух частей — это имя(свойство) и значение.

What are forms?
Форма-раздел документа, который позволяет пользователю вводить информацию для последующей обработки системой(т.е это элементы управления, которые применяются для сбора информации от посетителей веб-сайта).

What is a div?
div (англ. division — раздел)- блочный элемент,предназначен для выделения фрагмента документа с целью изменения вида содержимого 

What are selectors?
селектор - это формальное описание того элемента или группы элементов, к которым применяется указанное правило стиля(т.е селектор определяет, к какому элементу применять то или иное CSS-правило).

What are properties?
Свойство - это имя,которое неоходимо установить для атрибута.

What are values?
Значение-это значение , которое необходимо установить для свойства(имя атирибута).Значение атрибута всегда помещается в кавычки.

What is the “query string” in a URL and what does it do?
Uniform Resource Locator ( URL )- унифицированного идентификатора ресурса в просторечии называется веб - адрес , является ссылкой на веб - ресурс , который определяет его местоположение на компьютерной сети и механизм для извлечения его.
“query string” - строка запроса является частью унифицированного указателя ресурса (URL),который содержит параметры поиска
Строки запроса не существуют, пока пользователь не введет данные которые небходимо найти в базу данных поиска, после чего поисковая система создаст динамический URL со строкой запроса на основе результатов введеннх искомых данных.

What is the difference between “pixels” and “ems”?
(px)Пиксели - это единицы фиксированного размера, которые используются на экранах монитора (например, для чтения на экране компьютера). Один пиксель равен размеру одной точки на экране монитора (самый малый элемент разрешения вашего экрана)
Em являются своего рода процентами. Em относится к размеру базового текста. Значение 1 em означает то же, что и значение 100 percent. Но вы также можете сказать это обратным образом: процентное значение - это просто Em, умноженное на 100.

How do CSS styles for a particular element get inherited? i.e. how does an element get its “default” styles?
При указании стиля для элемента часть свойств может быть унаследована его дочерними элементами и потомками, этот эффект называется наследованием.
Например, все элементы, расположенные внутри элемента <body>, являются его дочерними элементами и потомками. Если в стиле для <body> задать с помощью CSS свойства color красный цвет текста, то цвет текста всех его дочерних элементов и потомков тоже станет красным

What are two CSS attributes you can change to push an element around on the page?
margin и padding

What are the three different ways to include CSS in your project or use CSS to style a particular element?
Вариант 1 — Глобальный CSS
Глобальный CSS помещается в контейнер <head> конкретной страницы. При таком варианте подключения классы и идентификаторы (ID) могут быть использованы для обращения к CSS коду, однако, они будут активны только на этой конкретной странице. CSS стили подключенные таким путем загружаются при каждой повторной загрузке страницы, поэтому они могут повлиять на скорость ее загрузки. Тем не менее, существует несколько ситуаций в которых использование глобальных CSS может быть полезно. К примеру, если вам необходимо отправить кому-нибудь шаблон страницы – вам гораздо проще будет предоставить предварительный результат, если все будет на одной странице. Глобальные CSS помещаются между тегами <style></style>. Вот пример глобальной таблицы стилей
Вариант 2 — Внешний CSS
Возможно самый удобный вариант для подключения CSS к вашему сайту, это его привязка к внешнему .css файлу. В этом случае все изменения сделанные во внешнем CSS файле, будут в целом отражаться на вашем сайте. Ссылка на внешний CSS файл помещается в контейнер <head> страницы
Вариант 3 — Внутренний CSS
Внутренний CSS используется для конкретного тега HTML. Атрибут <style> используется для настройки этого тега. Этот вариант подключения CSS не является рекомендованным, так как в этом случае необходимо настраивать каждый тег HTML по отдельности. К тому же управление вашим сайтом может стать довольно трудным, если вы будете использовать только внутренний CSS. Однако в некоторых случаях этот способ может быть весьма полезным. К примеру, в случае если у вас нет доступа к CSS файлам, или вам необходимо применить правила только для одного элемента.

What is the “default stylesheet” or “user agent stylesheet”?
Это набор правил CSS, встроенныx в браузер(таблица стилей по умолчанию)для стандартного отображения HTML странии. 

Why use a CSS reset file?
Для того, чтобы убрать таблицу стилей по умолчанию и задать свои стили.В разных браузерах HTML документ с таблицей стилей по умолчанию отображается по разному.

Answers in english

Why do we separate HTML and CSS?
Efficiency and maintenance 'cost'. By keeping a separate CSS file it's possible to apply a single property/value to millions of classes/ID's/elements across thousands of separate HTML pages.

If individual styling had to be entered on every <p> tag on the BBC News website for instance, thousands of man hours would be wasted every month on the tedious task, let alone when any styling changes need to be made.

What are classes and IDs (and how are they different)?
Classes and ID's are both types of attribute that can be applied to HTML elements and can then be used to apply CSS to those elements.

Classes can be applied to multiple elements whereas IDs should only be applied to one specific element (not a type of element, just one single element)

Technically, you can actually apply multiple versions of the same ID attribute, there's nothing physically stopping you - it's just a near certainty that something will break on all but the most simple site and you'll be sad in the knowledge that you're creating invalid HTML.

So the rule is 'don't do it because it's wrong and you'll face problems' rather than 'you can physically put it on more than one'.

What are elements?
HTML elements are the basic building blocks of the HTML Document and consist of a start tag, content and an end tag.

Example elements: div, p, nav, section, a, img and footer.

What are tags?
Tags are the 'words' of the HTML 'language'. Tags consist of an opening angle bracket < the element name and a closing >. Example <p>.

What are attributes?
Attributes provide extra information about an HTML element. Attributes are always placed inside the <> of the start tag and have the form name="value".

What are forms?
A form is something that collects user input. Forms contain form elements like input boxes and radio buttons which allow different ways to collect user input.

What is a div?
A div is simply a type of HTML Element that acts like a container to hold the content within. It is used to divide the HTML document into sections and can be used to apply CSS to very large or very specific sections of the HTML document.

What are selectors?
Selectors are found in CSS. They are used to 'select' an HTML element/ID/class.

In the purest sense, they are elements/IDs/classes. For instance, the element/tag <p> can be 'selected' in CSS simply as p.

An ID would be prefixed by a # and a class would be prefixed with a .. These examples might make things clearer: ID #someID Class .someClass

What are properties?
Properties are found in CSS. They form part of the 'declaration block' along with 'values' and they come after the selector.

I find them hard to define without an example as a property is simply a 'thing' that can be applied to the selector (and by extension the element/ID/class) which when paired to a value will cause the element/ID/class to be altered in some way.

Here is an example:

selector {property:value;}

p {font-size:12px}

What are values?
With the last answer in mind, the value is the amount of the property to apply.

What is the "query string" in a URL and what does it do?
The standard definition is:

a query string is the part of a uniform resource locator (URL) containing data that does not fit conveniently into a hierarchical path structure. The query string commonly includes fields added to a base URI by a Web browser or other client application.

In the most specific sense it is a method of passing data to the 'appication' powering a website/webapp.

It can do a myrid of things from tracking URL clicks to passing form input to the 'backend'.

What is the difference between "pixels" and "ems"?
Pixels are an absolute measure and ems are a relative measure.

Ems are measured relative to the parent div, or to the HTML element, or to the browser defaults of the properties aren't included in the HTML document/CSS.

Pixels are exactly what they sound like, a font size of 16px will display 16px high on all screens. The problem comes when different screens have different sizes and pixel densities.

How do CSS styles for a particular element get inherited? ie. how does an element get its "default" styles?
The browser will have a default stylesheet which applies various declarations to the elements.

If this question is about how CSS inheritance is applied, the answer is too long for here and you can instead look here for more info.

What are two CSS attributes you can change to push an element around on the page?
Margin and padding are the basic ones. But you could also use position (and additional properties) or even translate to name two others.

What are the three different ways to include CSS in your project or use CSS to style a particular element?
Inline: Placed directly within the start tag of an HTML element as an 'attribute' and will be automatically applied.

Internal: Placed within <style> tags within the same HTML document as the elements (usually in the <head> section) and will be automatically applied.

External: Placed in a seperate text files save as .css and included/applied via a specifically formatted link in the <head> section.

What is the "default stylesheet" or "user agent stylesheet"?
It's simply a set of CSS rules that are inbuilt into the browser and which give HTML elements some default styling.

Why use a CSS reset file?
To neutralise the default stylesheet and allow you to start completely from a blank page. This can be useful in avoiding different browsers causing your markup to display differently.

