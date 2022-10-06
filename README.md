# Вопросы для собеседования на позицию фронтенд разработчик

## Секция 1. Вопросы по HTML

  <details><summary>Что такое и зачем нужен HTML?</summary>
  &nbsp;

HTML (от англ. _HyperText Markup Language_ — «язык гипертекстовой разметки») - это код, который используется для структурирования веб-страницы и её контента. HTML предоставляет средства для создания заголовков, абзацев, списков, ссылок, цитат и других элементов. Элементы HTML выделяются тегами, записанными с использованием угловых скобок. Например, `<img />`, `<input />` или `<p>`.

Прочитать:

1. [Основы HTML](https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/HTML_basics)
2. [Основы HTML](https://html5book.ru/osnovy-html/)
3. [Learn HTML Basics for Beginners in Just 15 Minutes](https://www.freecodecamp.org/news/html-basics-for-beginners/)

&nbsp;

</details>
  <details><summary>Что такое doctype и зачем он нужен?</summary>
  
  &nbsp;
  
  Тег DOCTYPE сообщает браузеру какую версию HTML вы используете. DOCTYPE должен находиться на первой строке каждого HTML документа. В HTML5 декларация типа документа выглядит очень просто: ```<!DOCTYPE html>```
  
  Прочитать:
  1. [DOCTYPE: история и варианты применения](https://htmlacademy.ru/blog/articles/doctype)
  2. [Что за загадочный доктайп и зачем он вообще нужен?](https://doka.guide/html/doctype/)
  3. [Document type declaration](https://en.wikipedia.org/wiki/Document_type_declaration)
  
  &nbsp;
  
</details>
  <details><summary>Обязательно ли писать теги head, body и html?</summary>

&nbsp;

[Согласно спецификации HTML](https://html.spec.whatwg.org/multipage/syntax.html#optional-tags) эти теги могут быть пропущены.
Кроме того, например, в [руководстве по стилю HTML](https://google.github.io/styleguide/htmlcssguide.html#HTML_Validity) от Google указано, что в целях оптимизации размера файла можно рассмотреть возможность исключения необязательных тегов:

```
<!-- Not recommended -->
<!DOCTYPE html>
<html>
 <head>
   <title>Spending money, spending bytes</title>
</head>
<body>
   <p>Sic.</p>
 </body>
</html>
```

```
<!-- Recommended -->
<!DOCTYPE html>
<title>Saving money, saving bytes</title>
<p>Qed.
```

Прочитать:

1. [Cпецификация HTML](https://html.spec.whatwg.org/multipage/syntax.html#optional-tags)
2. [Руководство по стилю HTML от Google](https://google.github.io/styleguide/htmlcssguide.html#HTML_Validity)

&nbsp;

</details>
  <details><summary>В чем отличие атрибутов от свойств в HTML тегах?</summary>

&nbsp;

Атрибут элемента HTML — это сущность, которая используется для определения поведения или отображения html-элемента. Атрибуты указываются в открывающем HTML теге и состоят из двух частей:

1. Имя атрибута (например, id, type, style и т.д.)
2. Значение атрибута (например, для атрибута type значением может быть "text")

Примеры:

```
  <tag_name attribute_name="value">Content</tag_name>
```

```
  <input id="input" type="text">
```

```
  <h1 style="font-size:40px;color:green;">Hello World</h1>
```

В то же время теги являются объектами (в соответствии с DOM). Поэтому, когда браузер парсит HTML документ атрибуты тегов становятся свойствами объектов DOM.

Прочитать:

1. [Атрибуты и свойства](https://learn.javascript.ru/dom-attributes-and-properties)
2. [Атрибуты и свойства элементов документа ](https://flagman.top/css/atributy-i-svojstva)
3. [Element](https://doka.guide/js/element/)

&nbsp;

</details>
  <details><summary>Что такое мета-теги?</summary>

&nbsp;

Мета-теги позволяют передавать поисковым системам дополнительную информацию о страницах, на которых они размещены.

Прочитать:

1. [Meta Tags for SEO: A Simple Guide for Beginners](https://ahrefs.com/blog/seo-meta-tags/)
2. [Meta Tags: The Definitive Guide to Meta-Data for SEO (2021)](https://seosherpa.com/meta-tags/)
3. [meta](https://doka.guide/html/meta/)

&nbsp;

</details>
  <details><summary>Что описывается в теге head?</summary>
  
  &nbsp;
  
  Тег ```head``` предназначен для хранения служебной информации о странице. Он располагается перед ```body```. Внутри ```head``` обычно содержится заголовок и описание страницы, подключаются внешние ресурсы, например, стили. Содержимое этого тега не отображается на странице напрямую.
  
  Прочитать:
  1. [Что можно положить в тег head](https://habr.com/ru/company/htmlacademy/blog/563894/)
  2. [What's in the head? Metadata in HTML](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)
  
  
  &nbsp;
  
  </details>
  <details><summary>Расскажите о meta-теге с name="viewport"?</summary>
  
  &nbsp;
  
  Viewport — это область, которую видит пользователь на экране, когда заходит на страницу сайта. Чтобы пользоваться сайтами было удобно, нужно правильно масштабировать страницы. Для этого используется метатег viewport. Он не делает верстку адаптивной. Его предназначение — контроль масштаба отображения страницы.
  
  Например:
  ```
  <meta name="viewport" content="width=device-width, initial-scale=1">
  ```
  
  Прочитать:
  1. [Метатег viewport: почему он важен и как его правильно использовать](https://timeweb.com/ru/community/articles/metateg-viewport-pochemu-on-vazhen-i-kak-ego-pravilno-ispolzovat)
  2. [Viewport meta tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag)
  
  &nbsp;
 
  </details>
  <details><summary>Что такое html entities?</summary>
    
  &nbsp;
  
  HTML-сущности — это части текста ("строки"), которые начинаются с символа амперсанда (&) и заканчиваются точкой с запятой (;). Некоторые специальные символы, если они появляются в документе HTML, могут вызвать недопонимание в синтаксическом анализаторе исходного кода HTML, например, символ "меньше" ( < ), при встрече с данным символом анализатор HTML может ошибочно принять этот символ за тег. Чтобы избежать данное недопонимание, можно использовать специальный объект (entity) &lt; чтобы заменить символ ( < ).
  
  Прочитать:
  1. [Мнемоники в HTML](https://ru.wikipedia.org/wiki/%D0%9C%D0%BD%D0%B5%D0%BC%D0%BE%D0%BD%D0%B8%D0%BA%D0%B8_%D0%B2_HTML)
  
  &nbsp;
 
  </details>
  <details><summary>Где можно найти списки с html entities? </summary>
  
  &nbsp;
  
  Списки html сущностей можно найти:
  1. [в спецификации](https://html.spec.whatwg.org/multipage/named-characters.html)
  2. [в Википедии](https://ru.wikipedia.org/wiki/%D0%9C%D0%BD%D0%B5%D0%BC%D0%BE%D0%BD%D0%B8%D0%BA%D0%B8_%D0%B2_HTML)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое data атрибуты?</summary>

&nbsp;

data-\* атрибуты позволяют хранить дополнительную информацию в стандартных элементах HTML без визуального представления.

Прочитать:

1. [Полное руководство по HTML-атрибутам data-\*](https://habr.com/ru/company/ruvds/blog/490626/)
2. [.dataset](https://doka.guide/js/element-dataset/)

&nbsp;

</details>
  <details><summary>Откуда берутся пробелы в HTML?</summary>

&nbsp;

Элемент со значением `display: inline-block` ведет себя, как обычная буква и простой текст — имеет пробелы между словами. Браузер создаёт пустой текстовый узел, который, по сути, может являться переводом строки, пробелом или табом. Все и эти перечисленные вещи превращаются в один единственный пробел и описывается следующей сущностью: &#x0020. Удалить пробелы можно удалив пробелы между HTML элементами.

Прочитать:

1. [«Загадочные отступы» между инлайн-элементами (+прочитать обсуждение под статьей)](https://habr.com/ru/post/137582/)
2. [Fighting the Space Between Inline Block Elements](https://css-tricks.com/fighting-the-space-between-inline-block-elements/)
3. [How whitespace is handled by HTML, CSS, and in the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Whitespace)

&nbsp;

</details>
  <details><summary>Типы input элементов в HTML?</summary>
  
  &nbsp;
  
  ```input``` — это контейнер для интерактивных элементов, с помощью которых пользователь может ввести данные, что-то выбрать, поставить галочку или нажать кнопку.
  Атрибут type указывает на его тип. Тип элемента определяет его отображение и функционал. Например, type="text" - текстовое поле, type="submit" - кнопка отправки, type="radio" - переключатель, type="checkbox" - чек-бокс, type="hidden" - скрытое поле, type="password" - пароль и т.д.
  
  Прочитать:
  1. [Многогранный тег input](https://doka.guide/html/input/)
  2. [<input> MDN](https://developer.mozilla.org/ru/docs/Web/HTML/Element/Input)
  
  &nbsp;
  
  </details>
  <details><summary>Какие глобальные атрибуты есть в HTML?</summary>
    
  &nbsp;
  
  Глобальные атрибуты - атрибуты, которые могут быть использованы со всеми HTML элементами.
  
  Прочитать:
  1. [Глобальные атрибуты](https://developer.mozilla.org/ru/docs/Web/HTML/Global_attributes)
  2. [HTML-атрибуты](https://html5book.ru/html-attributes/)
  
  &nbsp;
  
  </details>
  
  
  <details><summary>Почему у разных тегов есть одни и теже свойства?</summary>
  
  &nbsp;
  
  Интерфейс Element представляет собой один из объектов в Document. Этот интерфейс описывает методы и свойства, общие для всех видов элементов. Конкретные модели поведения описаны в интерфейсах, которые наследуют от Element, и добавляют дополнительную функциональность.
Например, интерфейс HTMLElement является базовым интерфейсом для HTML-элементов, SVGElement (en-US) является основой для всех SVG-элементов.
  
  Прочитать:
  1. (Свойства узлов: тип, тег и содержимое)[https://learn.javascript.ru/basic-dom-node-properties]
  2. (Element)[https://developer.mozilla.org/en-US/docs/Web/API/Element]
  
  &nbsp;
  
  </details>
  <details><summary>В чем смысл семантических тегов?</summary>
    
  &nbsp;
  
  Семантические элементы четко описывают, что они означают, как браузеру, так и веб-разработчику.
  
  Некоторые из преимуществ использования семантической разметки:
  1. Поисковые системы будут рассматривать содержимое такой разметки как важные ключевые слова, влияющие на рейтинг страницы в результатах поиска (смотри SEO)
  2. Программы для чтения с экрана могут использовать её как указатель, чтобы помочь слабовидящим пользователям ориентироваться на странице
  3. Среди бесконечных блоков div гораздо проще найти блок семантического кода, чем блок с семантическим классом или классом, принадлежащим пространству имён.
  4. Указывает разработчику на тип данных, которые будут размещены
  5. Семантическая разметка отражает правильное именование элементов / компонентов
  
  Прочитать:
  1. [Забудьте про div, семантика спасёт интернет](https://habr.com/ru/company/htmlacademy/blog/546500/)
  2. [Semantic HTML: The Unbearable Rightness of Being](https://ux.shopify.com/semantic-html-the-unbearable-rightness-of-being-9b3c493e1791#.97h35dx34)
  
  &nbsp;
  
  </details>
  <details><summary>Есть ли проблема если всю верстку делать на дивах?</summary>
    
  &nbsp;
  
  Элемент div оборачивает другие элементы и семантически ничего не значит. При этом при помощи ARIA атрибутов можно имитировать доступность или другие HTML теги.
  
  Прочитать:
  1. [Раздоры вокруг div](https://habr.com/ru/company/ruvds/blog/651557/)
  2. [Stop using so many divs! An intro to semantic HTML](https://dev.to/kenbellows/stop-using-so-many-divs-an-intro-to-semantic-html-3i9i)
  
  &nbsp;
  
  </details>
  <details><summary> Чем семантика отличается от доступности(a11y)?</summary>
  
  &nbsp;
  
  Доступность — это практика, позволяющая использовать сайты как можно большему числу людей. В это число входят не только люди с ограниченными возможностями, но и другие группы пользователей. Хотя мы обычно думаем о людях с ограниченными возможностями, как о людях, находящихся в этом состоянии постоянно, на самом деле любой может обрести временную потерю функциональности. Например, кто-то является слепым человеком, у кого-то временная глазная инфекция, а кто-то просто находится на улице под ярким ослепляющим солнцем. Всё это может быть причиной, почему пользователь в данный момент не способен увидеть, что отображено на экране. Любой может по какой-то причине на время стать ограниченным в возможностях, и поэтому улучшение доступности веб-сайтов улучшит удобство всех пользователей, независимо от их состояния.
  
  Семантическая вёрстка — подход к разметке, который опирается не на содержание сайта, а на смысловое предназначение каждого блока и логическую структуру документа.
Например, наличие заголовков помогает незрячим в навигации по странице. У скринридеров есть функция навигации по заголовкам, что ускоряет знакомство с информацией на сайте.

Прочитать:

1. [Что такое доступность?](https://developer.mozilla.org/ru/docs/Learn/Accessibility/What_is_accessibility)
2. [Web Almanac - Accessibility](https://almanac.httparchive.org/en/2019/accessibility)
3. [Semantic HTML: the foundation of web accessibility](https://uxdesign.cc/semantic-html-the-foundation-of-web-accessibility-e5bbecad7c17)
   &nbsp;

  </details>
  <details><summary>Как мы можем семантически разделять контент на странице?</summary>
    
  &nbsp;
  
  HTML5 предлагает набор секционных (структурных) элементов, используя которые вы добавляете смысловую или семантическую нагрузку своим страницам, тем самым позволяя компьютерным программам лучше понимать их содержание.
  
  Прочитать:
  1. [Как использовать секционные элементы HTML5](https://habr.com/ru/post/214407/)
  2. [How to Section Your HTML](https://css-tricks.com/how-to-section-your-html/)
  
  &nbsp;
  
  </details>
  <details><summary> Почему это не очень правильно вместо тегов section и header использовать обычный div?</summary>
    
  &nbsp;
  
  Такие теги, как: header, footer, aside, h1, nav, ul и другие, помогают людям с ограниченными возможностями воспринимать сайт полностью без проблем. Так же используя семантические теги вы показываете поисковому роботу структуру сайта, где у вас шапка сайта, где подвал, а где основной контент страницы.
  
  Прочитать:
  1. [Что такое доступность?](https://developer.mozilla.org/ru/docs/Learn/Accessibility/What_is_accessibility)
  2. [How to Section Your HTML](https://css-tricks.com/how-to-section-your-html/)
  
  &nbsp;
  
  </details>
  <details><summary>в чём отличие article от section</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Структура HTML5 — div, section и article](https://noteskeeper.ru/heritage/54/)
  2. [Difference between article tag and section tag](https://www.geeksforgeeks.org/difference-between-article-tag-and-section-tag/)
  2. [Why You Should Choose HTML5 article Over section](https://www.smashingmagazine.com/2020/01/html5-article-section/)
  
  &nbsp;
  
  </details>
  <details><summary>Как семантически правильно сверстать картинку с подписью?</summary>

&nbsp;

Прочитать:

1. [Доклад Яндекса](https://habr.com/ru/company/yandex/blog/559442/)
2. [Image Techniques On The Web](https://ishadeed.com/article/image-techniques/)
3. [Image SEO: Optimizing images for search engines](https://yoast.com/image-seo/)

&nbsp;

</details>

<details><summary>Зачем для картинок нужен атрибут alt?</summary>

&nbsp;

alt это обязательный атрибут. Текст в alt называется альтернативным описанием изображения и рассказывает словами, что изображено. Это полезно, если картинка не загрузилась или пользователь не видит изображения. Если забыть добавить атрибут, то скринридер попытается прочесть название файла: в лучшем случае это будет logo-large, но может быть и b764b84c, что не очень информативно. Если оставить значение атрибута пустым, то скринридер посчитает это изображение декоративным, а не контентным. Если вы добиваетесь именно этого — отлично, но тогда, возможно, стоит вставить его как фоновую картинку с помощью CSS. Когда картинка по какой-то причине не загружается, браузеры отображают вместо неё альтернативный текст. Его даже можно стилизовать, если задать текстовые стили тегу <img>.

Прочитать:

1. [Как правильно написать alt-текст](https://htmlacademy.ru/blog/articles/alt-text)
2. [6 простых правил хорошего alt-текста](https://habr.com/ru/company/htmlacademy/blog/667540/)
3. [Alt-texts: The Ultimate Guide](https://axesslab.com/alt-texts/)

&nbsp;

</details>
  <details><summary>Если у нас есть CSS, зачем существуют теги strong, center, etc?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Как правильно написать alt-текст](https://htmlacademy.ru/blog/articles/alt-text)
  2. [6 простых правил хорошего alt-текста](https://habr.com/ru/company/htmlacademy/blog/667540/)
  3. [Alt-texts: The Ultimate Guide](https://axesslab.com/alt-texts/)
  
  &nbsp;
  
  </details>
  <details><summary>В чем разница между тегами b и strong?</summary>
    
  &nbsp;
  
  Тег ```strong``` указывает на важность отмеченного текста. Он может использоваться для выделения предупреждений или части документа, которую пользователь должен увидеть раньше остального. При этом обозначение части текста тегом ```strong``` не должно изменять смысла предложения. Элемент ```b``` используется для привлечения внимания к тексту, не указывая на то, что это более важно. Скринридер при чтении сайта будет выделять слова с тегом ```strong``` интонационно, в отличие от простого выделения с помощью ```b```.
  
  Прочитать:
  1. [strong](https://developer.mozilla.org/ru/docs/Web/HTML/Element/strong)
  2. [Какие HTML теги правильные? Отличия b от strong](https://axivan.com/kakie-html-tegi-pravilnye-otlichiya-b-ot-strong/)
  
  &nbsp;
  
  </details>
  <details><summary>Откуда тег b или strong берут свою "жирность"?</summary>
    
  &nbsp;
  
  В большинстве браузеров дефолтные стили для тегов b и strong это font-weight: bold
  
  &nbsp;
  
  </details>
  <details><summary>Почему плохо верстать кнопки не с button, а с помощью div</summary>
    
  &nbsp;
  
  Кнопка созданная с помощью div потеряет много функционала, в т.ч. и семантику. Недостающие свойства придётся дописывать самому.
  
  Прочитать:
  1. [button](https://doka.guide/html/button/)
  2. [How (Not) to Build a Button](https://benmyers.dev/blog/clickable-divs/)
  3. [When role="button" is not enough](https://dev.to/tylerjdev/when-role-button-is-not-enough-dac)
  4. [A Complete Guide to Links and Buttons](https://css-tricks.com/a-complete-guide-to-links-and-buttons/)
  
  &nbsp;
  
  </details>
  <details><summary>зачем aria role button, если есть тэг button</summary>
    
  &nbsp;
  
  1. [ARIA: button role](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/button_role)
  2. [A Complete Guide to Links and Buttons](https://css-tricks.com/a-complete-guide-to-links-and-buttons/)
  
  &nbsp;
  
  </details>
  <details><summary>Когда нужно использовать кнопки а когда ссылки?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Что лучше использовать: ссылки или кнопки](https://htmlacademy.ru/blog/articles/links-or-buttons)
  2. [When Is A Button Not A Button?](https://www.smashingmagazine.com/2019/02/buttons-interfaces/)
  3. [A Complete Guide to Links and Buttons](https://css-tricks.com/a-complete-guide-to-links-and-buttons/)
  
  &nbsp;
  
  </details>
  <details><summary>Можем ли мы использовать h1 несколько раз на странице?</summary>
    
  &nbsp;
  
  Использование нескольких тегов h1 на одной странице не отразится на результатах ее ранжирования. В контенте можно размещать любое количество заголовков первого уровня, и это никак не отразится на позициях сайта в выдаче. ем не менее, не стоит злоупотреблять использованием большого количества этих тегов.
  
  Прочитать:
  1. [Multiple H1 Tags on Page is Perfectly Fine in SEO](https://www.stanventures.com/blog/multiple-h1-tags/)
  2. [What is an H1 Tag? SEO Best Practices](https://ahrefs.com/blog/h1-tag/)
  
  &nbsp;
  
  </details>
  <details><summary>Можем ли мы использовать тег header в нескольких местах?</summary>
    
  &nbsp;
  
  Тег header в HTML обычно используют для шапки (верхушки) сайта, но не только для нее. В него как правило помещают логотип, верхнее меню, контакты. Часто, вся информация, которая находится в header (лого, меню и т.д.) одинаково отображается на всех страницах сайта. Тегов header на странице может быть сколько угодно.
  
  Прочитать:
  1. [Learn What HTML Header (New Semantic Document Tag) Does](https://html.com/tags/header/)
  2. [html5: using header or footer tag twice?](https://stackoverflow.com/questions/4837269/html5-using-header-or-footer-tag-twice)
  
  &nbsp;
  
  </details>
  <details><summary>Что ты знаешь о тэге picture?</summary>
    
  &nbsp;
  
  Тег ```picture``` используется, когда для разных устройств или вариантов отображения нам нужны разные картинки.
  
  Прочитать:
  1. [picture](https://doka.guide/html/picture/)
  2. [Почему стоит использовать тег <picture> вместо <img>](https://habr.com/ru/company/vdsina/blog/555736/)
  3. [A Guide to the Responsive Images Syntax in HTML](https://css-tricks.com/a-guide-to-the-responsive-images-syntax-in-html/)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое srcset? Как работает srcset?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Responsive images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)
  2. [A Guide to the Responsive Images Syntax in HTML](https://css-tricks.com/a-guide-to-the-responsive-images-syntax-in-html/)
  
  &nbsp;
  
  </details>
  <details><summary>Как работает HTML форма и что нужно чтобы ее отправить?</summary>
  
  &nbsp;
    
  Прочитать:
  1. [Learn Forms](https://web.dev/learn/forms/)
  2. [Best Practices for Form Design: Structure, Inputs, Labels and Actions](https://xd.adobe.com/ideas/principles/web-design/best-practices-form-design/)
  3. [Creating Accessible Forms](https://webaim.org/techniques/forms/)
  4. [Best Practices For Mobile Form Design](https://www.smashingmagazine.com/2018/08/best-practices-for-mobile-form-design/)
  
  &nbsp;
  
  </details>
  <details><summary>С помощью каких тегов ты будешь делать html форму?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Learn Forms](https://web.dev/learn/forms/)
  2. [Best Practices for Form Design: Structure, Inputs, Labels and Actions](https://xd.adobe.com/ideas/principles/web-design/best-practices-form-design/)
  
  &nbsp;
  
  </details>
  <details><summary>Можем ли сделать html форму без тега form?</summary>
    
  &nbsp;
  
  Без тега form пропадает доступность, становится не ясно какие инпуты к чему относятся, пропадает событие submit. 
  
  &nbsp;
  
  </details>
  <details><summary>Что значит type submit на форме</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Отправка формы: событие и метод submit](https://learn.javascript.ru/forms-submit)
  2. [input type="submit"](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/submit)
  
  &nbsp;
  
  </details>
  <details><summary>Как очистить форму?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [HTMLFormElement.reset()](https://developer.mozilla.org/ru/docs/Web/API/HTMLFormElement/reset)
  
  &nbsp;
  
  </details>
  <details><summary>Особенности whitespace в HTML?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Свойство white-space](https://learn.javascript.ru/white-space)
  2. [white-space](https://doka.guide/css/white-space/)
  3. [white-space](https://css-tricks.com/almanac/properties/w/whitespace/)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое и зачем нужен iframe?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Исчерпывающий путеводитель по тегу iframe](https://habr.com/ru/post/488516/)
  2. [4 IFrame Security Concerns You Should Know](https://blog.bitsrc.io/4-security-concerns-with-iframes-every-web-developer-should-know-24c73e6a33e4)
  
  &nbsp;
  
  </details>
  <details><summary>Что произойдет если мы напишем невалидную разметку?</summary
    
  &nbsp;
  
  Прочитать:
  1. [Parse errors](https://html.spec.whatwg.org/multipage/parsing.html#parse-errors)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое HTML валидация? И какие типы проверок HTML документа вы знаете?</summary>
    
  &nbsp;

Прочитать:

1. [What is Markup Validation?](https://validator.w3.org/docs/help.html#validation_basics)
2. [Web Accessibility Evaluation Tools List](https://www.w3.org/WAI/ER/tools/)

&nbsp;

  </details>
  <details><summary>Как проверить правильную иерархию html заголовков?</summary>
    
  &nbsp;
  
  [the W3C Markup Validator](https://validator.w3.org/)
  
  &nbsp;
  
  </details>
  <details><summary>рассказать об аттрибутах тега script</summary>
    
  &nbsp;
  
  Прочитать:
  1. [script](https://doka.guide/html/script/)
  2. [Скрипты: async, defer](https://learn.javascript.ru/script-async-defer)
  3. [Эффективная загрузка стороннего кода JavaScript](https://web.dev/i18n/ru/efficiently-load-third-party-javascript/)
  4. [Everything I Know About The Script Tag](https://eager.io/blog/everything-I-know-about-the-script-tag/)
  
  &nbsp;
  
  </details>
  <details><summary>почему тег script нужно ставить перед закрывающим боди</summary>
    
  &nbsp;
  
  Браузер рендерит страницу сверху вниз, в случае когда скрипты располагаются в теге ```head``` рендеринг останавливается для того, что бы браузер скачал и выполнил эти скрипты и затем продолжает работу, для некоторых сайтов эта задержка чувствительная, в таком случае предпочитают сначала вывести контент сайта, а затем подгрузить скрипты.
Так же, когда какая-либо функция скрипта, работает с DOM-элементами сайта, то при подключении сверху эта функция будет пытаться обратится к DOM-элементу который еще не отрендерил браузер, что вызовет ошибку.
  
  &nbsp;
  
  </details>
  <details><summary>Как скрыть элемент с помощью HTML</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Атрибут hidden](https://doka.guide/html/hidden/)
  2. [The HTML5 hidden attribute](https://allyjs.io/tutorials/hiding-elements.html#the-html5-hidden-attribute)
  
  &nbsp;
  
  </details>
  <details><summary>что такое якорные ссылки</summary>
    
  &nbsp;
  
  
  
  &nbsp;
  
  </details>
  <details><summary>Что такое атрибут target? Какие значения он принимает?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [target](https://developer.mozilla.org/ru/docs/Web/HTML/Element/A#attr-target)
  
  &nbsp;
  
  </details>
  <details><summary>какие проблемы есть у _target</summary>
  
    &nbsp;
    
  Прочитать:
  1. [Опасный target="_blank"](https://habr.com/ru/post/282880/)
  2. [Web app security. Target="_blank" vulnerability](https://thecodest.co/blog/web-app-security-target-_blank-vulnerability)
    
    &nbsp;
  
  </details>
  <details><summary>Расскажи про опенграф и схема орг  разметку</summary>
  &nbsp;
  
  Прочитать:
  1. [Микроразметка Schema.org: полное руководство](https://kokoc.com/blog/schema-org-polnoe-rukovodstvo-po-semanticheskoy-razmetke/)
  2. [Что такое разметка Open Graph и как ее внедрить без программиста](https://habr.com/ru/company/click/blog/492258/)
  3. [Open Graph Meta Tags: Everything You Need to Know](https://ahrefs.com/blog/open-graph-meta-tags/)
  4. [What Is Schema Markup? How to Use It for SEO](https://ahrefs.com/blog/schema-markup/)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое элемент canvas? И для чего он используется?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [CANVAS шаг за шагом: Основы](https://habr.com/ru/post/111308/)
  
  &nbsp;
  
  </details>
  <details><summary>Для чего используется элемент datalist?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [datalist](https://webref.ru/html/datalist)
  2. [HTML5 Datalist: What You Need To Know](https://www.jotform.com/blog/html5-datalists-what-you-need-to-know-78024/)
  3. [A Look into: HTML5 Datalist](https://www.hongkiat.com/blog/html5-datalist/)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое SVG и canvas и в чём между ними разница?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [SVG или canvas?](https://habr.com/ru/company/ruvds/blog/476292/)
  2. [Using SVG vs. Canvas: A short guide](https://blog.logrocket.com/svg-vs-canvas/)
  
  &nbsp;
  
  </details>
  <details><summary>Когда использоваьб canvas, а когда SVG?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [SVG или canvas?](https://habr.com/ru/company/ruvds/blog/476292/)
  2. [Using SVG vs. Canvas: A short guide](https://blog.logrocket.com/svg-vs-canvas/)
  
  &nbsp;
  
  </details>
  <details><summary>Плюсы и минусы canvas и SVG?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [SVG или canvas?](https://habr.com/ru/company/ruvds/blog/476292/)
  2. [Using SVG vs. Canvas: A short guide](https://blog.logrocket.com/svg-vs-canvas/)
  
  &nbsp;
  
  </details>
  <details><summary>Для чего нужен атрибут autocomplete?</summary>
    
  &nbsp;
  
    Прочитать:
  1. [Атрибут autocomplete](https://doka.guide/html/autocomplete/)
  2. [HTML attribute: autocomplete](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/autocomplete)
  2. [Autofill](https://web.dev/learn/forms/autofill/)
  
  &nbsp;
  
  </details>
  <details><summary>Для чего используют атрибут novalidate?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Атрибут novalidate](https://doka.guide/html/novalidate/)
  2. [Валидация форм на стороне клиента](https://developer.mozilla.org/ru/docs/Learn/Forms/Form_validation)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое свойство valueAsNumber?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Input valueAsNumber](https://davidwalsh.name/input-valueasnumber)
  2. [HTMLInputElement.valueAsNumber](https://dev.to/js_bits_bill/htmlinputelement-valueasnumber-js-bits-3pfl)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое ApplicationCache в HTML5?</summary>
    
  &nbsp;
  
  AppCache is documented as [deprecated](https://chromestatus.com/feature/6192449487634432) and under removal in [MDN](https://developer.mozilla.org/en-US/docs/Web/API/Window/applicationCache) and in the WHATWG standard, and marked as obsolete in W3C's HTML 5.1.
  
  Прочитать:
  1. [Application Cache API — новые возможности и проблемы](https://habr.com/ru/post/151815/)
  2. [A beginner's guide to using the application cache](https://web.dev/appcache-beginner/)
  
  &nbsp;
  
  </details>
  <details><summary>Как можно сгруппировать опции внутри тэга select?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [select](https://doka.guide/html/select/)
  2. [optgroup](https://doka.guide/html/optgroup/)
  
  &nbsp;
  
  </details>
  <details><summary>Для чего используют атрибут inputmode?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Атрибут inputmode](https://doka.guide/html/inputmode/)
  2. [Everything You Ever Wanted to Know About inputmode](https://css-tricks.com/everything-you-ever-wanted-to-know-about-inputmode/)
  
  &nbsp;
  
  </details>
  <details><summary>Что такое #shadow-root в инспекторе HTML-страницы?</summary>
    
  &nbsp;
  
  Прочитать:
  1. [Shadow DOM](https://learn.javascript.ru/shadow-dom)
  2. [Shadow DOM v1 - Self-Contained Web Components](https://web.dev/shadowdom-v1/)
  3. [A complete guide on shadow DOM and event propagation](https://pm.dartus.fr/blog/a-complete-guide-on-shadow-dom-and-event-propagation/)
  
  &nbsp;
  
  </details>

## Секция 2. Вопросы по CSS

  <details><summary>Как расшифровывается аббревиатура CSS?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Основы CSS](https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/CSS_basics)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как ты понимаешь что такое каскад?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Принцип каскада](https://doka.guide/css/cascade/)
  2. [The cascade](https://web.dev/learn/css/the-cascade/)
  
  &nbsp;
  
  </details>
  
  <details><summary>что такое блочная модель</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Блочная модель](https://web.dev/learn/css/box-model/)
  2. [Блочная модель](https://doka.guide/css/box-model/)
  3. [CSS Box Model Properties – Explained With Examples](https://www.freecodecamp.org/news/css-box-model-explained-with-examples/)
  
  &nbsp;
  
  </details>
  
  <details><summary>значения box-sizing и чем они отличаются</summary>
  
  &nbsp;
  
  Прочитать:
  1. [box-sizing](https://doka.guide/css/box-sizing/)
  2. [box-sizing](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)

&nbsp;

  </details>
  
  <details><summary>Как работает наследование в CSS?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Наследование](https://doka.guide/css/inheritance/)
  2. [Inheritance](https://web.dev/learn/css/inheritance/)
  3. [CSS Inheritance, The Cascade And Global Scope](https://www.smashingmagazine.com/2016/11/css-inheritance-cascade-global-scope-new-old-worst-best-friends/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Способы изоляции стилей в CSS?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Способы организации CSS-кода](https://habr.com/ru/post/256109/)
  2. [CSS Architecture with SASS, SMACSS, and BEM](https://itnext.io/css-architecture-with-sass-smacss-and-bem-cc618392c148)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие знаешь подходы по написанию CSS?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Способы организации CSS кода](https://habr.com/ru/post/256109/)
  2. [CSS Architecture with SASS, SMACSS, and BEM](https://itnext.io/css-architecture-with-sass-smacss-and-bem-cc618392c148)
  
  &nbsp;
  
  </details>
  
  <details><summary>Почему плохо писать все стили в одном файле или теге style?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Подключение стилей](https://doka.guide/css/adding-styles/)
  2. [How To Apply CSS Styles to HTML with Cascade and Specificity](https://www.digitalocean.com/community/tutorials/how-to-apply-css-styles-to-html-with-cascade-and-specificity)
  
  &nbsp;
  
  </details>
  
  <details><summary>В чем отличия разных подходов подключения стилей?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Подключение стилей](https://doka.guide/css/adding-styles/)
  2. [How To Apply CSS Styles to HTML with Cascade and Specificity](https://www.digitalocean.com/community/tutorials/how-to-apply-css-styles-to-html-with-cascade-and-specificity)
  
  &nbsp;
  
  </details>
  
  <details><summary>рассказать о достоинствах и недостатках подхода CSS-in-JS</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Всё, что вам нужно знать о CSS-in-JS](https://css-live.ru/articles/vsyo-chto-vam-nuzhno-znat-o-css-in-js.html)
  2. [A Thorough Analysis of CSS-in-JS](https://css-tricks.com/a-thorough-analysis-of-css-in-js/)
  3. [An Introduction to CSS-in-JS](https://webdesign.tutsplus.com/articles/an-introduction-to-css-in-js-examples-pros-and-cons--cms-33574)
  
  &nbsp;
  
  </details>
  
  <details><summary>рассказать о критическом css</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Как и почему вы должны инлайнить критический CSS](https://webformyself.com/kak-i-pochemu-vy-dolzhny-inlajnit-kriticheskij-css/)
  2. [Критический CSS и прогрессивный CSS ](https://medium.com/web-standards/critical-and-progressive-css-d6611f034d7d)
  3. [Understanding Critical CSS](https://www.smashingmagazine.com/2015/08/understanding-critical-css/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Специфичность в CSS</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Специфичность](https://doka.guide/css/specificity/)
  2. [Как CSS специфичность работает в браузере](https://habr.com/ru/post/436610/)
  3. [Specifics on CSS Specificity](https://css-tricks.com/specifics-on-css-specificity/)
  
  &nbsp;
  
  </details>
  
  <details><summary>зачем иногда селектора перечисляют через запятую?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Перечисление селекторов](https://doka.guide/css/selector-list/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как в CSS работают разные приоритеты стилей?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Каскад и наследование](https://developer.mozilla.org/ru/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)
  2. [Специфичность](https://doka.guide/css/specificity/)
  3. [Как CSS специфичность работает в браузере](https://habr.com/ru/post/436610/)
  4. [Specifics on CSS Specificity](https://css-tricks.com/specifics-on-css-specificity/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Рассказать про схлопывание отступов</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Схлопывание внешних отступов](https://developer.mozilla.org/ru/docs/Web/CSS/CSS_Box_Model/Mastering_margin_collapsing)
  2. [Схлопывающиеся margin](https://webref.ru/course/block-model/margin-collapse)
  3. [What is Margin Collapse in CSS? And How to Avoid It](https://www.freecodecamp.org/news/what-is-margin-collapse-and-how-to-avoid-it/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое адаптивная верстка?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Отзывчивый дизайн](https://developer.mozilla.org/ru/docs/Learn/CSS/CSS_layout/Responsive_Design)
  2. [Отзывчивый веб-дизайн](https://webref.ru/layout/advanced-html-css/responsive-web-design)
  3. [Адаптивная вёрстка](https://htmlacademy.ru/blog/articles/short-16)
  4. [Learn Responsive Design](https://web.dev/learn/design/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие ты знаешь подходы по созданию адаптивных сайтов?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Адаптивная вёрстка](https://htmlacademy.ru/blog/articles/short-16)
  2. [The Beginner’s Guide to Responsive Web Design (Code Samples & Layout Examples)](https://kinsta.com/blog/responsive-web-design/)
      
  &nbsp;
  
  </details>
  
  <details><summary>рассказать о подходах mobile-first и desktop-first</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Почему Mobile First?](https://habr.com/ru/post/269419/)
  2. [The State Of Mobile First and Desktop First](https://ishadeed.com/article/the-state-of-mobile-first-and-desktop-first/)
  3. [Mobile-First CSS: Is It Time for a Rethink?](https://alistapart.com/article/mobile-first-css-is-it-time-for-a-rethink/)
  4. [How to Take the Right Approach to Responsive Web Design](https://www.freecodecamp.org/news/taking-the-right-approach-to-responsive-web-design/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое media запросы?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [@media](https://doka.guide/css/media/)
  2. [A Complete Guide to CSS Media Queries](https://css-tricks.com/a-complete-guide-to-css-media-queries/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какими параметрами нужно манипулировать чтобы адаптировать сайт?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [The Beginner’s Guide to Responsive Web Design (Code Samples & Layout Examples)](https://kinsta.com/blog/responsive-web-design/)
  
  &nbsp;
  
  </details>
  
  <details><summary>В чем отличие адаптивного дизайна от отзывчивого?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Адаптивная вёрстка](https://htmlacademy.ru/blog/articles/short-16)
  2. [The Beginner’s Guide to Responsive Web Design (Code Samples & Layout Examples)](https://kinsta.com/blog/responsive-web-design/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Проблема адаптации таблицы?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Accessible, Simple, Responsive Tables](https://css-tricks.com/accessible-simple-responsive-tables/)
  2. [Responsive Data Tables](https://css-tricks.com/responsive-data-tables/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что ты знаешь о БЭМ?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [БЭМ-методология: с чего всё начиналось и зачем это всё нужно](https://habr.com/ru/company/yandex/blog/276035/)
  2. [BEM For Beginners: Why You Need BEM](https://www.smashingmagazine.com/2018/06/bem-for-beginners/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие способы выравнить элемент по горизонтали и вертикали ты знаешь?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Центрирование горизонтальное и вертикальное](https://learn.javascript.ru/css-center)
  2. [Centering in CSS](https://ishadeed.com/article/learn-css-centering/)
  3. [Centering in CSS: A Complete Guide](https://css-tricks.com/centering-css-complete-guide/)

&nbsp;

  </details>
  
  <details><summary>способы, чтобы задать расстояние между несколькими колонками</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Руководство по созданию удобных и отзывчивых CSS-колонок](https://webformyself.com/rukovodstvo-po-sozdaniyu-udobnyx-i-otzyvchivyx-css-kolonok/)
  1. [gap](https://css-tricks.com/almanac/properties/g/gap/)
  2. [Spacing in CSS](https://ishadeed.com/article/spacing-in-css/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как растянуть элемент на 100%?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Full Width Containers in Limited Width Parents](https://css-tricks.com/full-width-containers-limited-width-parents/)
  2. [CSS gotcha: How to fill page with a div?](https://dev.to/lennythedev/css-gotcha-how-to-fill-page-with-a-div-270j)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое псевдоэлементы?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Псевдоэлементы](https://doka.guide/css/pseudoelements/)
  2. [An Ultimate Guide To CSS Pseudo Classes And Pseudo Elements](https://www.smashingmagazine.com/2016/05/an-ultimate-guide-to-css-pseudo-classes-and-pseudo-elements/)
  3. [A guide to CSS pseudo-elements](https://blog.logrocket.com/a-guide-to-css-pseudo-elements/)
  4. [Pseudo-elements](https://web.dev/learn/css/pseudo-elements/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое псевдоклассы?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Псевдоклассы](https://doka.guide/css/pseudoclasses/)
  2. [Pseudo-classes](https://web.dev/learn/css/pseudo-classes/)
  3. [An Ultimate Guide To CSS Pseudo Classes And Pseudo Elements](https://www.smashingmagazine.com/2016/05/an-ultimate-guide-to-css-pseudo-classes-and-pseudo-elements/)
  4. [A Guide To Newly Supported, Modern CSS Pseudo-Class Selectors](https://www.smashingmagazine.com/2021/04/guide-supported-modern-css-pseudo-class-selectors/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как сбросить фон у элемента?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [background-color](https://doka.guide/css/background-color/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Ключевое отличие гридов от флексов</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Выбор CSS макета — Grid или Flexbox?](https://habr.com/ru/company/ruvds/blog/523808/)
  2. [When to use flexbox and when to use CSS grid](https://blog.logrocket.com/flexbox-vs-css-grid/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Объясни для каких задач подойдут флексы, а для каких гриды</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Выбор CSS макета — Grid или Flexbox?](https://habr.com/ru/company/ruvds/blog/523808/)
  2. [When to use flexbox and when to use CSS grid](https://blog.logrocket.com/flexbox-vs-css-grid/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Рассказажи какие бывают значения у свойства display?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Все значения свойства display](https://learn.javascript.ru/display)
  2. [display](https://doka.guide/css/display/)
  3. [display](https://css-tricks.com/almanac/properties/d/display/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Чем отличается блочный от инлайнового элемента?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Блочные элементы](https://webref.ru/course/block-inline/block)
  2. [Строчные элементы](https://webref.ru/course/block-inline/inline)
  3. [Строчно-блочные элементы](https://webref.ru/course/block-inline/inline-block)
  4. [Block Level Elements vs Inline Level Elements in HTML & CSS](https://blog.hubspot.com/website/block-level-elements-vs-inline-level-elements)
  
  &nbsp;
  
  </details>
  
  <details><summary>Рассказажи какие бывают значения у свойства position?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [position](https://doka.guide/css/position/)
  2. [position](https://css-tricks.com/almanac/properties/p/position/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое position: sticky?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [position: sticky](https://doka.guide/css/position-sticky/)
  2. [CSS Position Sticky - How It Really Works!](https://elad.medium.com/css-position-sticky-how-it-really-works-54cd01dc2d46)
  3. [How To Make Elements Stick with CSS position: sticky](https://www.digitalocean.com/community/tutorials/css-position-sticky)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как бы ты эмулировал поведение position: sticky?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Scroll Sidebar, Multiple Techniques](https://css-tricks.com/scrollfollow-sidebar/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Расскажи про поведение top,left,bottom,right при различных значениях position</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Типы позиционирования](https://developer.mozilla.org/ru/docs/Web/CSS/position#%D1%82%D0%B8%D0%BF%D1%8B_%D0%BF%D0%BE%D0%B7%D0%B8%D1%86%D0%B8%D0%BE%D0%BD%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F)
  2. [top bottom left right](https://css-tricks.com/almanac/properties/t/top-right-bottom-left/)
  
  &nbsp;
  
  </details>
  
  <details><summary>что будет когда position absolute внутри position absolute?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Absolute positioning inside absolute position](https://stackoverflow.com/questions/5928059/absolute-positioning-inside-absolute-position)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие есть способы подключения шрифтов?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Как подключить и оптимизировать нестандартные шрифты](https://htmlacademy.ru/blog/best/fonts-loading)
  2. [Оптимизация загрузки и рендеринга веб-шрифтов](https://web.dev/optimize-webfont-loading/)
  3. [How To Load and Use Custom Fonts with CSS](https://www.digitalocean.com/community/tutorials/how-to-load-and-use-custom-fonts-with-css)
  4. [Optimizing Google Fonts Performance](https://www.smashingmagazine.com/2019/06/optimizing-google-fonts-performance/)
  5. [Best practices for fonts](https://web.dev/optimize-webfont-loading/)
  
  &nbsp;
  
  </details>
  
  <details><summary>в чём отличие вариативных шрифтов от обычных</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Введение в вариативные шрифты](https://web.dev/i18n/ru/variable-fonts/)
  2. [Вариативные веб шрифты](https://habr.com/ru/post/413297/)
  3. [Variable fonts guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Fonts/Variable_Fonts_Guide)
  4. [Variable Fonts on the Web Using CSS](https://www.digitalocean.com/community/tutorials/css-variable-fonts)
  
  &nbsp;
  
  </details>
  
  <details><summary>Назови способы оптимизации шрифтов</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Оптимизация загрузки и рендеринга веб-шрифтов](https://web.dev/optimize-webfont-loading/)
  2. [Optimizing Google Fonts Performance](https://www.smashingmagazine.com/2019/06/optimizing-google-fonts-performance/)
  3. [Best practices for fonts](https://web.dev/optimize-webfont-loading/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Назови способы оптимизации иконок</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Tools for Optimizing SVG](https://css-tricks.com/tools-for-optimizing-svg/)
  2. [A Practical Guide](https://svgontheweb.com/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Расскажи какие форматы графических изображений ты знаешь</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Форматы изображений для веба](https://htmlacademy.ru/blog/articles/image-formats)
  2. [Актуальные форматы изображений в вебе](https://habr.com/ru/post/594211/)
  3. [Using Modern Image Formats: AVIF And WebP](https://www.smashingmagazine.com/2021/09/modern-image-formats-avif-webp/)
  4. [A Developer’s Guide to Understanding Image Types](https://docs.imgix.com/best-practices/guide-to-image-types)
  5. [AVIF has landed](https://jakearchibald.com/2020/avif-has-landed/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какой популярный браузер только недавно начал поддерживать webp?</summary>
  
  &nbsp;
  
  Safari 14.0 – 15.6 has full support of WebP, but requires macOS 11 Big Sur or later
  
  Прочитать:
  1. [Safari 14 ships webp support](https://dev.to/ben/safari-14-ships-webp-support-are-we-nearing-the-end-of-png-on-the-web-2f53)
  
  &nbsp;
  
  </details>
  
  <details><summary>Зачем нужно указывать ширину и высоту для картинок?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Задавать Height и Width для изображений снова важно](https://habr.com/ru/post/524918/) - в п.2 оригинал этой статьи на английском языке
  2. [Setting Height And Width On Images Is Important Again](https://www.smashingmagazine.com/2020/03/setting-height-width-images-important-again/)
  3. [Optimize Cumulative Layout Shift](https://web.dev/i18n/en/optimize-cls/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как мы можем сделать webp с фолбеком?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Using WebP Images with Fallback](https://usefulangle.com/post/114/webp-image-in-html-with-fallback)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что ты знаешь про концепцию optimistic ui?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Кратко про оптимистичный UI. Оптимистичные интерфейсы в картинках](https://habr.com/ru/company/productivity_inside/blog/317664/)
  2. [True Lies Of Optimistic User Interfaces](https://www.smashingmagazine.com/2016/11/true-lies-of-optimistic-user-interfaces/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Можно ли с помощью JS поменять значение псевдоэлемента?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Two different ways to style Pseudo-elements with Javascript](https://medium.com/codex/two-different-ways-to-style-pseudo-elements-with-javascript-3d9260d9c61b)
  2. [How to Change Look & Feel of Pseudo Elements using JavaScript and CSS Custom Properties](https://blog.shhdharmen.me/how-to-change-look-and-feel-of-pseudo-elements-using-javascript-and-css-custom-properties)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как можно скрыть элемент не используя display: none?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Методы скрытия элементов веб-страниц](https://habr.com/ru/company/ruvds/blog/485640/)
  
  &nbsp;
  
  </details>
  
  <details><summary>как скрыть элемент, но чтобы поисковики его видели?</summary>
  
  &nbsp;
  
  Элемент с атрибутом hidden остаётся виден поисковым роботам и индексируется ими. Так же можно использовать display none, но скрытый контент всегда будет обладать меньшим весом и хуже ранживаться, т.е. не стоит прятать важную часть контента, содержащую ключи по которым пользователи могут искать этот материал.
      
  
  &nbsp;
  
  </details>
  
  <details><summary>Как найти все скрытые элементы на странице?</summary>
  
  &nbsp;
  
  document.querySelectorAll("[style='display:none']") и другие вариации в зависимости от метода скрытия элемента.
  
  &nbsp;
  
  </details>
  
  <details><summary>Как ты стилизуешь чекбоксы, инпуты etc? </summary>
  
  &nbsp;
  
  Прочитать:
  1. [Custom Checkbox](https://www.w3schools.com/howto/howto_css_custom_checkbox.asp)
  2. [How to style a checkbox using CSS](https://stackoverflow.com/questions/4148499/how-to-style-a-checkbox-using-css)
  3. [How to style forms with CSS: A beginner’s guide](https://blog.logrocket.com/how-to-style-forms-with-css-a-beginners-guide/)
  4. [How To Style Common Form Elements with CSS](https://www.digitalocean.com/community/tutorials/how-to-style-common-form-elements-with-css)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое User agent стили</summary>
  
  &nbsp;
  
  Прочитать:
  1. [User-agent stylesheets](https://developer.mozilla.org/en-US/docs/Web/CSS/Cascade#user-agent_stylesheets)
  
  &nbsp;
  
  </details>
  
  <details><summary>Импорты и модульность в CSS</summary>
  
  &nbsp;
  
  Прочитать:
  1. [import](https://doka.guide/css/import/)
  2. [import](https://developer.mozilla.org/en-US/docs/Web/CSS/@import)
  3. [Практическое руководство по использованию CSS Modules в React приложениях](https://habr.com/ru/post/335244/)
  4. [What are CSS Modules and why do we need them?](https://css-tricks.com/css-modules-part-1-need/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие препроцессоры ты используешь или знаешь?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Popular CSS Preprocessors With Examples: Sass, Less & Stylus](https://raygun.com/blog/css-preprocessors-examples/)
  2. [What is PostCSS? How to Use Plugins to Automate CSS Tasks](https://www.freecodecamp.org/news/what-is-postcss/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Для чего ты используешь SASS?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Препроцессор Sass. Полное руководство и зачем он нужен](https://medium.com/@stasonmars/%D0%BF%D1%80%D0%B5%D0%BF%D1%80%D0%BE%D1%86%D0%B5%D1%81%D1%81%D0%BE%D1%80-sass-%D0%BF%D0%BE%D0%BB%D0%BD%D0%BE%D0%B5-%D1%80%D1%83%D0%BA%D0%BE%D0%B2%D0%BE%D0%B4%D1%81%D1%82%D0%B2%D0%BE-%D0%B8-%D0%B7%D0%B0%D1%87%D0%B5%D0%BC-%D0%BE%D0%BD-%D0%BD%D1%83%D0%B6%D0%B5%D0%BD-20fb638e29e3)
  2. [The definitive guide to SCSS](https://blog.logrocket.com/the-definitive-guide-to-scss/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Минус использования амперсанда в препроцессорах?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Leading Ampersands for modifiers in Sass: An anti-pattern](https://chipcullen.com/leading-ampersands-in-sass-an-anti-pattern/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как мы можем заставить элемент быть поверх другого?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Контекст наложения](https://doka.guide/css/stacking-context/)
  2. [Z-index and stacking contexts](https://web.dev/learn/css/z-index/)
  3. [Understanding Z-Index in CSS](https://ishadeed.com/article/understanding-z-index/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое и когда создаётся новый контекс наложения?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Контекст наложения](https://doka.guide/css/stacking-context/)
  2. [Z-index and stacking contexts](https://web.dev/learn/css/z-index/)
  3. [Understanding Z-Index in CSS](https://ishadeed.com/article/understanding-z-index/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как бороться с переполнением контентом?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Переполнение содержимого](https://developer.mozilla.org/ru/docs/Learn/CSS/Building_blocks/Overflowing_content)
  2. [CSS Overflow: What It Is & How It Works](https://blog.hubspot.com/website/css-overflow)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие есть единицы измерения в CSS?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Единицы измерения](https://learn.javascript.ru/css-units)
  2. [Единицы измерения](https://doka.guide/css/numeric-types/)
  3. [vw, vh, vmin, vmax](https://doka.guide/css/vw-vh/)
  4. [rem, em](https://doka.guide/css/rem-em/)
  5. [CSS Units Explained](https://www.digitalocean.com/community/tutorials/css-css-units-explained)
  
  &nbsp;
  
  </details>
  
  <details><summary>Когда брать абсолютные величины а когда относительные?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Should I use px or rem value units in my CSS?](https://stackoverflow.com/questions/11799236/should-i-use-px-or-rem-value-units-in-my-css)
  2. [Pixels vs. Relative Units in CSS: why it’s still a big deal](https://www.24a11y.com/2019/pixels-vs-relative-units-in-css-why-its-still-a-big-deal/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие есть варианты указания цвета?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Цвета в CSS](https://habr.com/ru/company/ruvds/blog/505626/)
  2. [currentColor](https://doka.guide/css/currentcolor/)
  3. [Defining Colors in CSS](http://web.simmons.edu/~grovesd/comm244/notes/week3/css-colors)
  4. [A Guide To Modern CSS Colors With RGB, HSL, HWB, LAB And LCH](https://www.smashingmagazine.com/2021/11/guide-modern-css-colors/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какие есть способы модификации цвета?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [filter](https://css-tricks.com/almanac/properties/f/filter/)
  2. [backdrop-filter](https://css-tricks.com/almanac/properties/b/backdrop-filter/)
  2. [Dynamic Color Manipulation with CSS Relative Colors](https://blog.jim-nielsen.com/2021/css-relative-colors/)
  3. [The CSS color-mod Function](https://www.digitalocean.com/community/tutorials/css-color-function)
  
  &nbsp;
  
  </details>
  
  <details><summary>Особенности свойства color?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [currentColor](https://doka.guide/css/currentcolor/)
  2. [Делаем CSS короче с помощью currentColor](https://webformyself.com/delaem-css-koroche-s-pomoshhyu-currentcolor/)
  3. [Understanding the currentColor Keyword in CSS](https://www.digitalocean.com/community/tutorials/css-currentcolor)
  
  &nbsp;
  
  </details>
  
  <details><summary>Какое количество цветов поддерживает GIF?</summary>
  
  &nbsp;
  
  The maximum color depth of a GIF is 256 colors, because each pixel is represented as a single byte, which can be an index to at most 2^8 = 256 colors.
  
  &nbsp;
  
  </details>
  
  <details><summary>Доступность цвета</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Contrast and Color Accessibility](https://webaim.org/articles/contrast/)
  2. [Color Contrast And Why You Should Rethink It](https://www.smashingmagazine.com/2014/10/color-contrast-tips-and-tools-for-accessibility/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое вендорные префиксы? И для чего они используются?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Вендорные префиксы](https://doka.guide/css/vendor-prefixes/)
  2. [Autoprefixer](https://css-tricks.com/autoprefixer/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Зачем нам нужен autoprefixer?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Автопрефиксер — окончательное решение проблемы префиксов в CSS](https://habr.com/ru/company/evilmartians/blog/176909/)
  2. [Autoprefixer](https://css-tricks.com/autoprefixer/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Как автопрефиксер понимает где поставить префиксы?</summary>
  
  &nbsp;
  
  База данных Автопрефиксера обновляется с помощью библиотек browserslist и caniuse-lite. 
  
  &nbsp;
  
  </details>
  
  <details><summary>Как выбирать свойство основываясь на поддержке браузерами?</summary>
  
  &nbsp;

Можно посмотреть поддержку различных свойств браузерами на сайте [Can I Use](https://caniuse.com/)

Прочитать:

1. [Ускоряемся с помощью Browserslist](https://web-standards.ru/articles/speed-up-with-browserslist/)
2. [A Guide To CSS Support In Browsers](https://www.smashingmagazine.com/2019/02/css-browser-support/)

&nbsp;

  </details>
  
  <details><summary>что за свойство isolation в css</summary>
  
  &nbsp;
  
  Прочитать:
  1. [isolation](https://developer.mozilla.org/ru/docs/Web/CSS/isolation)
  2. [isolation](https://css-tricks.com/almanac/properties/i/isolation/)
  
  &nbsp;
  
  </details>
  
  <details><summary>какие в CSS есть ключевые слова (initial, inherit, unset, revert)</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Глобальные ключевые слова](https://doka.guide/css/global-keywords/)
  2. [Understanding the “Initial”, “Inherit” and “Unset” CSS Keywords](https://elad.medium.com/understanding-the-initial-inherit-and-unset-css-keywords-2d70b7121695)
  
  &nbsp;
  
  </details>
  
  <details><summary>что такое функция attr</summary>
  
  &nbsp;
  
  Прочитать:
  1. [attr](https://doka.guide/css/attr/)
  2. [attr](https://developer.mozilla.org/en-US/docs/Web/CSS/attr)
  3. [The CSS attr() function got nothin’ on custom properties](https://css-tricks.com/css-attr-function-got-nothin-custom-properties/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Разница между Reset.css и Normalize.css?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Нормальный сброс](https://htmlacademy.ru/blog/articles/short-13)
  2. [Normalize CSS or CSS Reset?!](https://elad.medium.com/normalize-css-or-css-reset-9d75175c5d1e)
  3. [Joshua Comeau - My Custom CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Разница между margin и padding?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [https://doka.guide/css/margin/](https://doka.guide/css/margin/)
  2. [padding](https://doka.guide/css/padding/)
  3. [CSS Margin vs. Padding: What's the Difference?](https://blog.hubspot.com/website/css-margin-vs-padding)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое CSS спрайт и для чего он используется</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Как использовать CSS-спрайты для увеличения скорости загрузки веб-страниц](https://ru.hexlet.io/blog/posts/kak-ispolzovat-css-sprayty-dlya-uvelicheniya-skorosti-zagruzki-veb-stranits)
  2. [CSS Sprites: What They Are, Why They’re Cool, and How To Use Them](https://css-tricks.com/css-sprites/)
  
  &nbsp;
  
  </details>
  
  <details><summary>Что такое #shadow-root в инспекторе HTML-страницы?</summary>
  
  &nbsp;
  
  Прочитать:
  1. [Shadow DOM](https://learn.javascript.ru/shadow-dom)
  2. [Как работает JS: технология Shadow DOM и веб-компоненты](https://habr.com/ru/company/ruvds/blog/415881/)
  3. [Shadow DOM v1 - Self-Contained Web Components](https://web.dev/shadowdom-v1/)
  
  &nbsp;
  
  </details>

## Секция 3. Вопросы по JavaScript

  <details><summary>Какие типы данных есть в JS?</summary>

&nbsp;

Прочитать:

1. [Типы данных](https://learn.javascript.ru/types)
2. [Data types](https://javascript.info/types)

&nbsp;

  </details>

  <details><summary>Разница между null и undefined?</summary>

&nbsp;

Прочитать:

1. [null & undefined](https://learn.javascript.ru/types#znachenie-null)
2. [What is the difference between null and undefined in JavaScript?](https://stackoverflow.com/questions/5076944/what-is-the-difference-between-null-and-undefined-in-javascript)

&nbsp;

  </details>

  <details><summary>Мутабельные и имутабельные типы данных</summary>

&nbsp;

Прочитать:

1. [Хранение по ссылке и по значению](https://doka.guide/js/ref-type-vs-value-type/)
2. [Копирование объектов и ссылки](https://learn.javascript.ru/object-copy)
3. [Mutable and immutable in JavaScript](https://blog.devgenius.io/mutable-and-immutable-in-javascript-78a3cbc6187c)

&nbsp;

  </details>

<details><summary>Какие есть типы переменных?</summary>

&nbsp;

Прочитать:

1. [Переменные](https://learn.javascript.ru/variables)
2. [Устаревшее ключевое слово "var"](https://learn.javascript.ru/var)
3. [Переменные const, let и var](https://doka.guide/js/var-let/)

&nbsp;

  </details>

  <details><summary>в каких случаях можно изменить значение в const</summary>

&nbsp;

Прочитать: 1.[const](https://doka.guide/js/const/)

&nbsp;

  </details>

  <details><summary>Что такое поднятие (Hoisting)?</summary>

&nbsp;

Прочитать:

1. [Разбираемся с “поднятием” (hoisting) в JavaScript](https://medium.com/@stasonmars/%D1%80%D0%B0%D0%B7%D0%B1%D0%B8%D1%80%D0%B0%D0%B5%D0%BC%D1%81%D1%8F-%D1%81-%D0%BF%D0%BE%D0%B4%D0%BD%D1%8F%D1%82%D0%B8%D0%B5%D0%BC-hoisting-%D0%B2-javascript-7d2d27bc51f1)
2. [What is Hoisting in JavaScript?](https://www.freecodecamp.org/news/what-is-hoisting-in-javascript/)
3. [Understanding Hoisting in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-hoisting-in-javascript)

&nbsp;

  </details>

  <details><summary>Чему равен и какой тип у NaN?</summary>

&nbsp;

Прочитать:

1. [NaN в JavaScript](https://webformyself.com/nan-v-javascript/)

&nbsp;

  </details>

  <details><summary>почему typeof NaN - число?</summary>

&nbsp;

Прочитать:

1. [Why does typeof NaN return 'number'?](https://stackoverflow.com/questions/2801601/why-does-typeof-nan-return-number)

&nbsp;

  </details>

  <details><summary>Зачем нужна блочная область видимости если уже есть функциональная?</summary>

&nbsp;

Прочитать:

1. [Области видимости](https://doka.guide/js/closures/)
2. [A Simple Explanation of Scope in JavaScript](https://dmitripavlutin.com/javascript-scope/)

&nbsp;

  </details>

  <details><summary>Какие есть операторы в JS?</summary>

&nbsp;

Прочитать:

1. [Базовые операторы, математика](https://learn.javascript.ru/operators)
2. [Операторы сравнения](https://learn.javascript.ru/comparison)
3. [Логические операторы](https://learn.javascript.ru/logical-operators)
4. [Оператор нулевого слияния](https://learn.javascript.ru/nullish-coalescing-operator)
5. [Тернарный оператор](https://doka.guide/js/ternary-operator/)

&nbsp;

  </details>

  <details><summary>Чем отличаются друг от друга унарные, бинарные и тернарные операторы?</summary>

&nbsp;

Прочитать:

1. [Термины: «унарный», «бинарный», «операнд»](https://learn.javascript.ru/operators#terminy-unarnyy-binarnyy-operand)
2. [Тернарный оператор](https://doka.guide/js/ternary-operator/)

&nbsp;

  </details>

  <details><summary>Какие есть операторы сравнения?</summary>

&nbsp;

Прочитать:

1. [Операторы сравнения](https://learn.javascript.ru/comparison)
2. [Understanding Comparison and Logical Operators in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-comparison-and-logical-operators-in-javascript)

&nbsp;

  </details>

  <details><summary>Разница между == и === (нестрогое/строгое равенство)?</summary>

&nbsp;

Прочитать:

1. [Строгое сравнение](https://learn.javascript.ru/comparison#strogoe-sravnenie)
2. [Строгое и нестрогое равенство](https://doka.guide/js/typecasting/#strogoe-i-nestrogoe-ravenstvo)

&nbsp;

  </details>

<details><summary>В чем есть особенность логических операторов?</summary>

&nbsp;

Прочитать:

1. [Логические операторы](https://learn.javascript.ru/logical-operators)
2. [Логические операторы](https://doka.guide/js/logic-operators/)
3. [Understanding Comparison and Logical Operators in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-comparison-and-logical-operators-in-javascript)

&nbsp;

  </details>

  <details><summary>В чем особенность выполнения логического "И"</summary>

&nbsp;

Прочитать:

1. [&&](https://learn.javascript.ru/logical-operators#i)
2. [И, &&](https://doka.guide/js/logic-operators/#i)

&nbsp;

  </details>

  <details><summary>Какие есть falsy значения?</summary>

&nbsp;

Прочитать:

1. [Логическое преобразование](https://learn.javascript.ru/type-conversions#logicheskoe-preobrazovanie)
2. [Falsy](https://developer.mozilla.org/en-US/docs/Glossary/Falsy)

&nbsp;

  </details>

  <details><summary>Зачем нужен use strict?</summary>

&nbsp;

Прочитать:

1. [use strict](https://doka.guide/js/use-strict/)
2. [Зачем в JavaScript нужен строгий режим?](https://habr.com/ru/company/ruvds/blog/477284/)
3. [JavaScript Use Strict Statement: A Guide to Use the Strict Mode](https://www.positioniseverything.net/javascript-use-strict/)

&nbsp;

  </details>

  <details><summary>Что такое Map и Set?</summary>

&nbsp;

Прочитать:

1. [Set](https://doka.guide/js/set/)
2. [Map](https://doka.guide/js/map/)
3. [Map and Set](https://javascript.info/map-set)
4. [Understanding Map and Set Objects in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-map-and-set-objects-in-javascript)

&nbsp;

  </details>

  <details><summary>Какие есть и как работают циклы в JS?</summary>

&nbsp;

Прочитать:

1. [Циклы while и for](https://learn.javascript.ru/while-for)
2. [Цикл "for..in"](https://learn.javascript.ru/object#forin)
3. [for...of](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...of)
4. [Loops and iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

&nbsp;

  </details>

  <details><summary>В чем разница циклов for .. in и for .. of?</summary>

&nbsp;

Прочитать:

1. [Различия между for...of и for...in](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...of#%D1%80%D0%B0%D0%B7%D0%BB%D0%B8%D1%87%D0%B8%D1%8F_%D0%BC%D0%B5%D0%B6%D0%B4%D1%83_for...of_%D0%B8_for...in)
2. [What is the difference between ( for... in ) and ( for... of ) statements?](https://stackoverflow.com/questions/29285897/what-is-the-difference-between-for-in-and-for-of-statements)

&nbsp;

  </details>

  <details><summary>Что за метод hasOwnProperty?</summary>

&nbsp;

Прочитать:

1. [Цикл "for..in"](https://learn.javascript.ru/object#forin)
2. [hasOwnProperty](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty)
3. [hasOwn](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwn)

&nbsp;

  </details>

  <details><summary>Можем ли мы создать объект который будет себя иначе вести в for of?</summary>

&nbsp;

Прочитать:

1. [Перебираемые объекты](https://learn.javascript.ru/iterable)
2. [Обход итерируемых объектов](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Statements/for...of#%D0%BE%D0%B1%D1%85%D0%BE%D0%B4_%D0%B8%D1%82%D0%B5%D1%80%D0%B8%D1%80%D1%83%D0%B5%D0%BC%D1%8B%D1%85_%D0%BE%D0%B1%D1%8A%D0%B5%D0%BA%D1%82%D0%BE%D0%B2)
3. [Symbol.iterator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Symbol/iterator)

&nbsp;

  </details>

  <details><summary>Отличие цикла for от while?</summary>

&nbsp;

Прочитать:

1. [Циклы while и for](https://learn.javascript.ru/while-for)

&nbsp;

  </details>

  <details><summary>Разница между forEach и map?</summary>

&nbsp;

Прочитать:

1. [forEach](https://doka.guide/js/array-foreach/)
2. [map](https://doka.guide/js/array-map/)
3. [Difference between forEach and map](https://stackoverflow.com/questions/34426458/javascript-difference-between-foreach-and-map)

&nbsp;

  </details>

  <details><summary>как работают методы reduce и filter</summary>

&nbsp;

Прочитать:

1. [reduce](https://doka.guide/js/array-reduce/)
2. [filter](https://doka.guide/js/array-filter/)

&nbsp;

  </details>

  <details><summary>как проверить что массив это массив</summary>

&nbsp;

Прочитать:

1. [Array.isArray](https://doka.guide/js/array-isarray/)
2. [How do I check if a variable is an array in JavaScript?](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/isArray)

&nbsp;

  </details>

  <details><summary>Как можно добавить элемент в начало и в конец массива?</summary>

&nbsp;

Прочитать:

1. [Методы pop/push, shift/unshift](https://learn.javascript.ru/array#metody-pop-push-shift-unshift)
2. [Array.prototype.splice](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)
3. [Array.prototype.concat](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)
4. [Spread в литералах массива](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/Spread_syntax#spread_%D0%B2_%D0%BB%D0%B8%D1%82%D0%B5%D1%80%D0%B0%D0%BB%D0%B0%D1%85_%D0%BC%D0%B0%D1%81%D1%81%D0%B8%D0%B2%D0%B0)

&nbsp;

  </details>

  <details><summary>Какие ты знаешь способы клонирования объектов?</summary>

&nbsp;

Прочитать:

1. [Копирование объектов и ссылки](https://learn.javascript.ru/object-copy)
2. [What is the most efficient way to deep clone an object in JavaScript?](https://stackoverflow.com/questions/122102/what-is-the-most-efficient-way-to-deep-clone-an-object-in-javascript)

&nbsp;

  </details>

  <details><summary>Для чего используется оператор !! (двойного отрицания)?</summary>

&nbsp;

Прочитать:

1. [Двойное НЕ (!!)](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/Logical_NOT#%D0%B4%D0%B2%D0%BE%D0%B9%D0%BD%D0%BE%D0%B5_%D0%BD%D0%B5_!!)
1. [What is the !! (not not) operator in JavaScript?](https://stackoverflow.com/questions/784929/what-is-the-not-not-operator-in-javascript)

&nbsp;

  </details>

  <details><summary>Разница между Rest и Spread операторами?</summary>

&nbsp;

Прочитать:

1. [Спред-синтаксис](https://doka.guide/js/spread/)
2. [Остаточные параметры](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Functions/Rest_parameters)
3. [JavaScript Rest vs Spread Operator – What’s the Difference?](https://www.freecodecamp.org/news/javascript-rest-vs-spread-operators)

&nbsp;

  </details>

  <details><summary>Как можно работать с датами в JS?</summary>

&nbsp;

Прочитать:

1. [Дата и время](https://learn.javascript.ru/date)
2. [Everything You Need to Know About Date in JavaScript](https://css-tricks.com/everything-you-need-to-know-about-date-in-javascript/)

&nbsp;

  </details>

  <details><summary>Можем ли мы замерить скорость работы участка кода с Date.now?</summary>

&nbsp;

Прочитать:

1. [Date.now](https://learn.javascript.ru/date#date-now)
2. [An Introduction to performance.now()](https://blog.bitsrc.io/a-very-quick-introduction-to-performance-now-c95493e77d06)

&nbsp;

  </details>

  <details><summary>Что такое function expression и function declaration?</summary>

&nbsp;

Прочитать:

1. [Function Expression в сравнении с Function Declaration](https://learn.javascript.ru/function-expressions#function-expression-v-sravnenii-s-function-declaration)
2. [Don't Confuse Function Expressions and Function Declarations in JavaScript](https://dmitripavlutin.com/javascript-function-expressions-and-declarations/)

&nbsp;

  </details>

  <details><summary>Что такое чистая функция?</summary>

&nbsp;

Прочитать:

1. [«Чистые» и «нечистые» функции в JavaScript](https://frontend-stuff.com/blog/pure-and-impure-functions-in-js/)
2. [What Is a Pure Function in JavaScript?](https://www.freecodecamp.org/news/what-is-a-pure-function-in-javascript-acb887375dfe/)

&nbsp;

  </details>

  <details><summary>Что такое функция первого порядка?</summary>

&nbsp;

Прочитать:

1. [Функции высшего порядка в JavaScript](https://medium.com/webbdev/func-1afa4a8220a7)
2. [What are Higher-Order Functions in JavaScript?](https://dmitripavlutin.com/javascript-higher-order-functions/)

&nbsp;

  </details>

  <details><summary>Что такое псевдомассив arguments?</summary>

&nbsp;

Прочитать:

1. [Переменная "arguments"](https://learn.javascript.ru/rest-parameters-spread-operator#the-arguments-variable)
2. [The arguments object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments)

&nbsp;

  </details>

  <details><summary>Что такое рекурсия?</summary>

&nbsp;

Прочитать:

1. [Рекурсия и стек](https://learn.javascript.ru/recursion)
2. [What is Recursion? A Recursive Function Explained with JavaScript Code Examples](https://www.freecodecamp.org/news/what-is-recursion-in-javascript/)

&nbsp;

  </details>

  <details><summary>Что такое замыкание?</summary>

&nbsp;

Прочитать:

1. [Замыкания в JavaScript для начинающих](https://habr.com/ru/company/ruvds/blog/424967/)
2. [Замыкание](https://learn.javascript.ru/closure)
3. [Понимаем замыкания в JavaScript. Раз и навсегда](https://medium.com/@stasonmars/%D0%BF%D0%BE%D0%BD%D0%B8%D0%BC%D0%B0%D0%B5%D0%BC-%D0%B7%D0%B0%D0%BC%D1%8B%D0%BA%D0%B0%D0%BD%D0%B8%D1%8F-%D0%B2-javascript-%D1%80%D0%B0%D0%B7-%D0%B8-%D0%BD%D0%B0%D0%B2%D1%81%D0%B5%D0%B3%D0%B4%D0%B0-c211805b6898)
4. [A Simple Explanation of JavaScript Closures](https://dmitripavlutin.com/simple-explanation-of-javascript-closures/)

&nbsp;

  </details>

  <details><summary>Что такое контекст у функции?</summary>

&nbsp;

Прочитать:

1. [this](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Operators/this)
2. [Контекст выполнения и стек вызовов в JavaScript](https://habr.com/ru/company/ruvds/blog/422089/)
3. [The many faces of `this` in javascript](https://blog.pragmatists.com/the-many-faces-of-this-in-javascript-5f8be40df52e)

&nbsp;

  </details>

  <details><summary>Какой контекст у стрелочных функций?</summary>

&nbsp;

Прочитать:

1. [Повторяем стрелочные функции](https://learn.javascript.ru/arrow-functions)
2. [Understanding Arrow Functions in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-arrow-functions-in-javascript)

&nbsp;

  </details>

  <details><summary>Как мы можем изменить контекст у функции?</summary>

&nbsp;

Прочитать:

1. [Привязка контекста к функции](https://learn.javascript.ru/bind)
2. [Явное указание this: "call", "apply"](https://learn.javascript.ru/call-apply)
3. [Javascript call() & apply() vs bind()?](https://stackoverflow.com/questions/15455009/javascript-call-apply-vs-bind)

&nbsp;

  </details>

  <details><summary>В чём разница между bind, call, apply?</summary>

&nbsp;

Прочитать:

1. [Привязка контекста к функции](https://learn.javascript.ru/bind)
2. [Явное указание this: "call", "apply"](https://learn.javascript.ru/call-apply)
3. [Javascript call() & apply() vs bind()?](https://stackoverflow.com/questions/15455009/javascript-call-apply-vs-bind)

&nbsp;

  </details>

  <details><summary>Что будет если забиндить два контекста подряд?</summary>

&nbsp;

Прочитать:

1. [Повторный bind](https://learn.javascript.ru/bind#povtornyy-bind)
2. [Bind more arguments of an already bound function in Javascript](https://stackoverflow.com/questions/20925138/bind-more-arguments-of-an-already-bound-function-in-javascript)

&nbsp;

  </details>

  <details><summary>Чем область видимости отличается от контекста?</summary>

&nbsp;

Прочитать:

1. [Different in "scope" and "context" in this Javascript code](https://stackoverflow.com/questions/14328519/different-in-scope-and-context-in-this-javascript-code)

&nbsp;

  </details>

  <details><summary>Как передаются параметры в функцию: по ссылке или по значению?</summary>

&nbsp;

Прочитать:

1. [Передача параметров по значению и по ссылке](https://metanit.com/web/javascript/3.7.php)
2. [Is JavaScript a pass-by-reference or pass-by-value language?](https://stackoverflow.com/questions/518000/is-javascript-a-pass-by-reference-or-pass-by-value-language)

&nbsp;

  </details>

  <details><summary>что такое каррирование?</summary>

&nbsp;

Прочитать:

1. [Каррирование](https://learn.javascript.ru/currying-partials)
2. [Каррирование функций в JavaScript](https://habr.com/ru/company/ruvds/blog/427295/)
3. [Understanding JavaScript currying](https://blog.logrocket.com/understanding-javascript-currying/)
4. [JavaScript Functional Programming Explained: Partial Application and Currying](https://www.digitalocean.com/community/tutorials/javascript-functional-programming-explained-partial-application-and-currying)

&nbsp;

  </details>

  <details><summary>что такое частичное применение?</summary>

&nbsp;

Прочитать:

1. [Частичное применение](https://doka.guide/js/fp/#chastichnoe-primenenie)
2. [Частичное применение или partial application в JavaScript](https://frontend-stuff.com/blog/partial-application/)
3. [JavaScript Functional Programming Explained: Partial Application and Currying](https://www.digitalocean.com/community/tutorials/javascript-functional-programming-explained-partial-application-and-currying)

&nbsp;

  </details>

  <details><summary>Что такое eval и почему его следует избегать?</summary>

&nbsp;

Прочитать:

1. [Eval: выполнение строки кода](https://learn.javascript.ru/eval)
2. [Never use eval](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/eval#never_use_eval!)

&nbsp;

  </details>

  <details><summary>Что такое регулярное выражение (Regular Expression)?</summary>

&nbsp;

Прочитать:

1. [Регулярные выражения](https://learn.javascript.ru/regular-expressions)
2. [Выразительный JavaScript: Регулярные выражения](https://habr.com/ru/post/242695/)
3. [A Practical Guide to Regular Expressions (RegEx) In JavaScript](https://blog.bitsrc.io/a-beginners-guide-to-regular-expressions-regex-in-javascript-9c58feb27eb4)
4. [Regular Expressions](https://eloquentjavascript.net/09_regexp.html)

&nbsp;

  </details>

  <details><summary>Что такое цепочка вызовов (chaining)?</summary>

&nbsp;

Прочитать:

1. [Цепочка вызовов](https://ru.hexlet.io/courses/js-basics/lessons/methods-chain/theory_unit)
2. [Understanding Method Chaining In Javascript](https://blog.segunolalive.com/posts/understanding-method-chaining-in-javascript/)
3. [What Method Chaining in JavaScript Is, How It Works and How to Use It](https://blog.alexdevero.com/method-chaining-in-javascript/)

&nbsp;

  </details>

  <details><summary>Что такое генераторы? Когда стоит использовать генераторы?</summary>

&nbsp;

Прочитать:

1. [Генераторы](https://learn.javascript.ru/generators)
2. [Углублённое руководство по JavaScript: генераторы](https://habr.com/ru/company/vk/blog/539194/)
3. [Generators](https://exploringjs.com/es6/ch_generators.html)

&nbsp;

  </details>

  <details><summary>Разница между host-объектами и нативными объектами?</summary>

&nbsp;

Прочитать:

1. [Объектно-ориентированное программирование в ванильном JavaScript](https://habr.com/ru/company/raiffeisenbank/blog/340584/)
2. [What is the difference between native objects and host objects?](https://stackoverflow.com/questions/7614317/what-is-the-difference-between-native-objects-and-host-objects)

&nbsp;

  </details>

  <details><summary>Что такое объектная обертка (Wrapper Objects)?</summary>

&nbsp;

Прочитать:

1. [Методы примитивов](https://learn.javascript.ru/primitives-methods)
2. [What are wrapper objects for primitive values?](https://2ality.com/2022/02/wrapper-objects.html)
3. [JavaScript Boxing Wrappers](https://javascript.plainenglish.io/javascript-boxing-wrappers-5b5ff9e5f6ab)

&nbsp;

  </details>

  <details><summary>Как работает boxing/unboxing в JavaScript?</summary>

&nbsp;

Прочитать:

1. [JavaScript Boxing Wrappers](https://javascript.plainenglish.io/javascript-boxing-wrappers-5b5ff9e5f6ab)

&nbsp;

  </details>

  <details><summary>Что такое прототипы и прототипное наследование?</summary>

&nbsp;

Прочитать:

1. [Прототипное наследование](https://learn.javascript.ru/prototype-inheritance)
2. [Прототипы в JS и малоизвестные факты](https://habr.com/ru/post/518360/)
3. [Understand Prototypes and Prototypal Inheritance in JavaScript](https://www.telerik.com/blogs/understand-prototypes-prototypal-inheritance-javascript)

&nbsp;

  </details>

  <details><summary>что такое **proto**</summary>

&nbsp;

Прочитать:

1. [Prototype](https://learn.javascript.ru/prototype-inheritance#prototype)
2. [proto](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/proto)

&nbsp;

  </details>

  <details><summary>Что происходит когда мы пишем ключевое слово new?</summary>

&nbsp;

Прочитать:

1. [Конструктор, оператор "new"](https://learn.javascript.ru/constructor-new)
2. [F.prototype](https://learn.javascript.ru/function-prototype)
3. [new operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/new)
4. [What is the 'new' keyword in JavaScript?](https://stackoverflow.com/questions/1646698/what-is-the-new-keyword-in-javascript)

&nbsp;

  </details>

  <details><summary>Откуда у примитива появляются методы (.toSting() и т.д.)?</summary>

&nbsp;

Прочитать:

1. [Методы примитивов](https://learn.javascript.ru/primitives-methods)
2. [What are wrapper objects for primitive values?](https://2ality.com/2022/02/wrapper-objects.html)
3. [JavaScript Boxing Wrappers](https://javascript.plainenglish.io/javascript-boxing-wrappers-5b5ff9e5f6ab)

&nbsp;

  </details>

  <details><summary>Как бы ты добавлял статический метод в prototype?</summary>

&nbsp;

Прочитать:

1. [Изменение встроенных прототипов](https://learn.javascript.ru/native-prototypes#native-prototype-change)
2. [Monkey patching in JavaScript](https://www.audero.it/blog/2016/12/05/monkey-patching-javascript/)

&nbsp;

  </details>

  <details><summary>Почему патчинг прототипа это плохо?</summary>

&nbsp;

Прочитать:

1. [Изменение встроенных прототипов](https://learn.javascript.ru/native-prototypes#native-prototype-change)
2. [Monkey patching in JavaScript](https://www.audero.it/blog/2016/12/05/monkey-patching-javascript/)

&nbsp;

  </details>

  <details><summary>Откуда берется свойство length у массива?</summary>

&nbsp;

Прочитать:

1. [Array.prototype.length](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/length)
2. [Внутреннее устройство массива](https://learn.javascript.ru/array#vnutrennee-ustroystvo-massiva)

&nbsp;

  </details>

  <details><summary>Как сделать какое либо свойство объекта неизменяемым?</summary>

&nbsp;

Прочитать:

1. [Флаги и дескрипторы свойств](https://learn.javascript.ru/property-descriptors)
2. [Object.defineProperty()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty)

&nbsp;

  </details>

  <details><summary>Как можно запретить изменение объекта?</summary>

&nbsp;

Прочитать:

1. [Глобальное запечатывание объекта](https://learn.javascript.ru/property-descriptors#globalnoe-zapechatyvanie-obekta)
2. [JavaScript Object Immutability](https://blog.bitsrc.io/javascript-object-immutability-1794b49c5255)
3. [JavaScript object immutability: Object.freeze vs. Object.seal](https://blog.logrocket.com/javascript-object-immutability-object-freeze-vs-object-seal/)

&nbsp;

  </details>

  <details><summary>Разниц между Object.freeze() и Object.seal()?</summary>

&nbsp;

Прочитать:

1. [Глобальное запечатывание объекта](https://learn.javascript.ru/property-descriptors#globalnoe-zapechatyvanie-obekta)
2. [JavaScript Object Immutability](https://blog.bitsrc.io/javascript-object-immutability-1794b49c5255)
3. [JavaScript object immutability: Object.freeze vs. Object.seal](https://blog.logrocket.com/javascript-object-immutability-object-freeze-vs-object-seal/)

&nbsp;

  </details>

  <details><summary>Разница между typeof и instanceof?</summary>

&nbsp;

Прочитать:

1. [What is the difference between typeof and instanceof and when should one be used vs. the other?](https://stackoverflow.com/questions/899574/what-is-the-difference-between-typeof-and-instanceof-and-when-should-one-be-used)
2. [Type checking in JavaScript: typeof and instanceof operators](https://dmitripavlutin.com/javascript-typeof-instanceof/)

&nbsp;

  </details>

  <details><summary>Как работает метод Object.create()?</summary>

&nbsp;

Прочитать:

1. [Object.create()](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Object/create)

&nbsp;

  </details>

  <details><summary>Как объекты преобразовываются в примитивы?</summary>

&nbsp;

Прочитать:

1. [Преобразование объектов в примитивы](https://learn.javascript.ru/object-toprimitive)
2. [Converting Object to Primitives in JavaScript](https://www.codingninjas.com/codestudio/library/converting-object-to-primitives-in-javascript)

&nbsp;

  </details>

  <details><summary>Что такое event loop?</summary>

&nbsp;

Прочитать:

1. [Что ты такое, Event Loop? Или как устроен цикл событий в браузере Chrome](https://habr.com/ru/post/461401/)
2. [Событийный цикл: микрозадачи и макрозадачи](https://learn.javascript.ru/event-loop)
3. [How JavaScript works: Event loop and the rise of Async programming + 5 ways to better coding with async/await](https://blog.sessionstack.com/how-javascript-works-event-loop-and-the-rise-of-async-programming-5-ways-to-better-coding-with-2f077c4438b5)
4. [Understanding the Event Loop, Callbacks, Promises, and Async/Await in JavaScript](https://www.digitalocean.com/community/tutorials/understanding-the-event-loop-callbacks-promises-and-async-await-in-javascript)

&nbsp;

  </details>

  <details><summary>Что такое и как работают ES модули?</summary>

&nbsp;

Прочитать:

1. [Модули, введение](https://learn.javascript.ru/modules-intro)
2. [Глубокое погружение в ES-модули в картинках](https://medium.com/web-standards/es-modules-cartoon-dive-71f42c1e851a)
3. [The JavaScript Modules Handbook – Complete Guide to ES Modules and Module Bundlers](https://www.freecodecamp.org/news/javascript-es-modules-and-module-bundlers/)

&nbsp;

  </details>

  <details><summary>В чем разница между ES и commonjs модулями?</summary>

&nbsp;

Прочитать:

1. [Понимание (всех) «модульных» форматов и инструментов JavaScript](https://habr.com/ru/post/501198/)
1. [CommonJS vs. ES modules in Node.js](https://blog.logrocket.com/commonjs-vs-es-modules-node-js/)

&nbsp;

  </details>

  <details><summary>Можем ли мы поменять переменную в модуле извне?</summary>

&nbsp;

Прочитать:

1. [Своя область видимости переменных](https://learn.javascript.ru/modules-intro#svoya-oblast-vidimosti-peremennyh)

&nbsp;

  </details>

  <details><summary>Как мы можем эмулировать модули не используя ES modules/require?</summary>

&nbsp;

Прочитать:

1. [IIFE](https://learn.javascript.ru/closure#iife)
2. [Brief history of JavaScript Modules](https://medium.com/sungthecoder/javascript-module-module-loader-module-bundler-es6-module-confused-yet-6343510e7bde)

&nbsp;

  </details>

  <details><summary>что такое iife?</summary>

&nbsp;

Прочитать:

1. [IIFE](https://learn.javascript.ru/closure#iife)
2. [Essential JavaScript: Mastering Immediately-invoked Function Expressions](https://vvkchandra.medium.com/essential-javascript-mastering-immediately-invoked-function-expressions-67791338ddc6)

&nbsp;

  </details>

  <details><summary>В чем смысл оборачивания всего содержимого JavaScript-файла в функцию?</summary>

&nbsp;

Прочитать:

1. [The Revealing Module Pattern](https://www.oreilly.com/library/view/learning-javascript-design/9781449334840/ch09s03.html)
2. [The Revealing Module Pattern in Javascript](https://gist.github.com/zcaceres/bb0eec99c02dda6aac0e041d0d4d7bf2)

&nbsp;

  </details>

  <details><summary>Что такое и как работает Promise?</summary>

&nbsp;

Прочитать:

1. [Промисы](https://learn.javascript.ru/promise-basics)
2. [Promise](https://doka.guide/js/promise/)
3. [JavaScript Promise Tutorial – How to Resolve or Reject Promises in JS](https://www.freecodecamp.org/news/javascript-promise-tutorial-how-to-resolve-or-reject-promises-in-js/)
4. [JavaScript Promises: an introduction](https://web.dev/i18n/en/promises/)

&nbsp;

  </details>

  <details><summary>как увидеть какой статус у промиса</summary>

&nbsp;

Прочитать:

1. [How can I synchronously determine a JavaScript Promise's state?](https://stackoverflow.com/questions/30564053/how-can-i-synchronously-determine-a-javascript-promises-state)

&nbsp;

  </details>

  <details><summary>какие методы есть у промисов?</summary>

&nbsp;

Прочитать:

1. [Promise API](https://learn.javascript.ru/promise-api)
2. [Static methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise#static_methods)

&nbsp;

  </details>

  <details><summary>что будет, если в промисе вызвать несколько резолвов подряд?</summary>

&nbsp;

Состояние промиса может быть изменено только один раз. Все последующие вызовы resolve и reject будут проигнорированы.

&nbsp;

  </details>

  <details><summary>В чём разница между макро- и микро- тасками</summary>

&nbsp;

Прочитать:

1. [Событийный цикл: микрозадачи и макрозадачи](https://learn.javascript.ru/event-loop)
2. [Difference between microtask and macrotask within an event loop context](https://stackoverflow.com/questions/25915634/difference-between-microtask-and-macrotask-within-an-event-loop-context)

&nbsp;

  </details>

  <details><summary>что такое async/await</summary>

&nbsp;

Прочитать:

1. [https://learn.javascript.ru/async-await](Async/await)
2. [async/await](https://doka.guide/js/async-in-js/#svyazka-async-await)

&nbsp;

  </details>

  <details><summary>Что такое Callback Hell?</summary>

&nbsp;

Прочитать:

1. [Адская пирамида вызовов](https://learn.javascript.ru/callbacks#adskaya-piramida-vyzovov)
2. [How to deal with nested callbacks and avoid “callback hell”](https://www.freecodecamp.org/news/how-to-deal-with-nested-callbacks-and-avoid-callback-hell-1bc8dc4a2012/)

&nbsp;

  </details>

  <details><summary>В чём отличия между setTimeOut и setInterval</summary>

&nbsp;

Прочитать:

1. [Планирование: setTimeout и setInterval](https://learn.javascript.ru/settimeout-setinterval)
2. [How To Schedule Tasks With setTimeout() and setInterval() in JavaScript](https://www.digitalocean.com/community/tutorials/js-settimeout-setinterval)
3. [setTimeout or setInterval?](https://stackoverflow.com/questions/729921/settimeout-or-setinterval)

&nbsp;

  </details>

  <details><summary>Что такое сборщик мусора?</summary>

&nbsp;

Прочитать:

1. [Сборка мусора](https://learn.javascript.ru/garbage-collection)
2. [Управление памятью](https://developer.mozilla.org/ru/docs/Web/JavaScript/Memory_Management)
3. [garbage.collect()](https://habr.com/ru/company/oleg-bunin/blog/433318/)

&nbsp;

  </details>

  <details><summary>Можем ли мы повлиять на сборку мусора?</summary>

&nbsp;

Прочитать:

1. [garbage.collect()](https://habr.com/ru/company/oleg-bunin/blog/433318/)
2. [Can I trigger JavaScript's garbage collection?](https://stackoverflow.com/questions/8032928/can-i-trigger-javascripts-garbage-collection)
3. [How to request the Garbage Collector in node.js to run?]()

&nbsp;

  </details>

  <details><summary>Как мы будем через JS анимировать что либо?</summary>

&nbsp;

Прочитать:

1. [JavaScript-анимации](https://learn.javascript.ru/js-animation)
2. [Как работает JS: анимация средствами CSS и JavaScript](https://habr.com/ru/company/ruvds/blog/354438/)

&nbsp;

  </details>

  <details><summary>Расскажи про requestAnimationFrame</summary>

&nbsp;

Прочитать:

1. [Использование requestAnimationFrame](https://learn.javascript.ru/js-animation#ispolzovanie-requestanimationframe)
2. [JavaScript: заметка о requestAnimationFrame и requestIdleCallback](https://habr.com/ru/company/timeweb/blog/587908/)
3. [Window.requestAnimationFrame](https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame)

&nbsp;

  </details>

  <details><summary>Зачем нужны сборщики во фронтенде?</summary>

&nbsp;

Прочитать:

1. [Системы сборки](https://doka.guide/tools/bundlers/)
2. [The top latest build tools for JavaScript](https://blog.logrocket.com/the-top-latest-build-tools-for-javascript/)
3. [JavaScript Bundlers: An in-depth comparative](https://dev.to/underscorecode/javascript-bundlers-an-in-depth-comparative-is-webpack-still-the-best-bundler-in-2021-59jk)

&nbsp;

  </details>

  <details><summary>Как ты понимаешь что код написан хорошо?</summary>

&nbsp;

Прочитать:

1. [clean-code-javascript](https://github.com/ryanmcdermott/clean-code-javascript)
2. [Static analysis in JavaScript](https://blog.logrocket.com/static-analysis-in-javascript-11-tools-to-help-you-catch-errors-before-users-do/)

&nbsp;

  </details>

  <details><summary>Зачем нужен REST?</summary>

&nbsp;

Прочитать:

1. [REST, что же ты такое?](https://habr.com/ru/post/590679/)
2. [REST vs SOAP](https://habr.com/ru/post/131343/)
3. [Microsoft REST API Guidelines](https://github.com/microsoft/api-guidelines/blob/vNext/Guidelines.md)

&nbsp;

  </details>

  <details><summary>Что такое ООП?</summary>

&nbsp;

Прочитать:

1. [Объектно-ориентированное программирование](https://doka.guide/js/oop/)
2. [ООП в картинках](https://habr.com/ru/post/463125/)
3. [Object-oriented programming](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object-oriented_programming)

&nbsp;

  </details>

  <details><summary>Чем ООП в JS отличается от ООП в других языках?</summary>

&nbsp;

Прочитать:

1. [ООП в JavaScript](https://doka.guide/js/oop/#oop-v-javascript)
2. [Объектно-ориентированный JavaScript простыми словами](https://habr.com/ru/post/522380/)
3. [Знакомство с ООП на примере JavaScript](https://habr.com/ru/company/ruvds/blog/665290/)

&nbsp;

  </details>

  <details><summary>В чем заключается отличие классов в JS от классов в других языках?</summary>

&nbsp;

Прочитать:

1. [Как работают классы в JavaScript](https://medium.com/front-stories/%D0%BA%D0%B0%D0%BA-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0%D1%8E%D1%82-%D0%BA%D0%BB%D0%B0%D1%81%D1%81%D1%8B-%D0%B2-javascript-7978c0003f1d)

&nbsp;

  </details>

  <details><summary>Какие еще знаешь парадигмы программирования?</summary>

&nbsp;

Прочитать:

1. [Парадигмы программирования](https://doka.guide/js/programming-paradigms/)
2. [Programming paradigm](https://en.wikipedia.org/wiki/Programming_paradigm)

&nbsp;

  </details>

  <details><summary>Чем описание класса отличается от экземпляра класса?</summary>

&nbsp;

Класс включает описание полей данных, а также методов, которые работают с этими полями данных. Экземпляр — это объект, содержащий данные и поведение, описанные классом. В JavaScript оператор new создает экземпляр класса (const instance = new Class ()).

&nbsp;

  </details>

  <details><summary>Что такое SOLID?</summary>

&nbsp;

Прочитать:

1. [Принципы SOLID, о которых должен знать каждый разработчик](https://habr.com/ru/company/ruvds/blog/426413/)
2. [The SOLID Principles of Object-Oriented Programming Explained in Plain English](https://www.freecodecamp.org/news/solid-principles-explained-in-plain-english/)

&nbsp;

  </details>

  <details><summary>Что такое CQRS?</summary>

&nbsp;

Прочитать:

1. [Основы CQRS](https://habr.com/ru/company/simbirsoft/blog/329970/)
2. [CQRS](https://martinfowler.com/bliki/CQRS.html)

&nbsp;

  </details>

  <details><summary>Что такое GRASP?</summary>

&nbsp;

Прочитать:

1. [GRASP паттерны проектирования](https://habr.com/ru/post/92570/)
2. [GRASP – General Responsibility Assignment Software Patterns Explained](https://www.kamilgrzybek.com/design/grasp-explained/)

&nbsp;

  </details>

  <details><summary>Что такое DRY, KISS?</summary>

&nbsp;

Прочитать:

1. [Три ключевых принципа ПО, которые вы должны понимать](https://habr.com/ru/post/144611/)
2. [A Better Definition of the DRY Programming Principle](https://blog.devgenius.io/a-better-definition-of-the-dry-programming-principle-13a3d0af4d40)

&nbsp;

  </details>

  <details><summary>Пишешь ли тесты и что о них знаешь?</summary>

&nbsp;

Прочитать:

1. [Фундаментальная теория тестирования](https://habr.com/ru/post/549054/)
1. [Автоматическое тестирование c использованием фреймворка Mocha](https://learn.javascript.ru/testing-mocha)
1. [Лучшие методики тестирования в JavaScript и Node.js](https://habr.com/ru/company/vk/blog/466879/)

&nbsp;

  </details>

  <details><summary>Что такое полифил (polyfill)?</summary>

&nbsp;

Прочитать:

1. [Полифил](https://developer.mozilla.org/ru/docs/Glossary/Polyfill)
2. [Полифилы](https://learn.javascript.ru/polyfills)
3. [What is the difference between polyfill and transpiler?](https://stackoverflow.com/questions/31205640/what-is-the-difference-between-polyfill-and-transpiler)

&nbsp;

  </details>

  <details><summary>Что такое временная мёртвая зона (temporal dead zone)?</summary>

&nbsp;

Прочитать:

1. [ES6: Let, Const и «Временная мёртвая зона» (ВМЗ) изнутри](https://css-live.ru/articles/es6-let-const-i-vremennaya-myortvaya-zona-vmz-iznutri.html)
2. [What is the Temporal Dead Zone (TDZ) in JavaScript?](https://www.freecodecamp.org/news/what-is-the-temporal-dead-zone/)
3. [Why is there a “temporal dead zone” in ES6?](https://2ality.com/2015/10/why-tdz.html)

&nbsp;

  </details>

  <details><summary>Плюсы и минусы BFF (Backend for Frontend)</summary>

&nbsp;

Прочитать:

1. [Паттерны Gateway и Backend-for-Frontend](https://doka.guide/tools/gateway-bff/)
2. [The BFF Pattern (Backend for Frontend): An Introduction](https://blog.bitsrc.io/bff-pattern-backend-for-frontend-an-introduction-e4fa965128bf)

&nbsp;

  </details>

  <details><summary>Что такое Babel и для чего он используется?</summary>

&nbsp;

Прочитать:

1. [What is Babel?](https://babeljs.io/docs/en/)
2. [Understanding the Modern Web Stack: Babel](https://dev.to/alexeagleson/building-a-modern-web-stack-babel-3hfp)

&nbsp;

  </details>

## JavaScript в браузере

<details><summary>Что такое DOM?</summary>

&nbsp;

Прочитать:

1. [Выразительный JavaScript: Document Object Model (объектная модель документа)](https://habr.com/ru/post/243815/)
2. [What is the DOM?](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

&nbsp;

</details>

<details><summary>Пропадет ли DOM если мы отключим JS?</summary>

&nbsp;

DOM — это независящий от платформы и языка программный интерфейс.

&nbsp;

</details>

<details><summary>Что такое всплытие событий и какие есть фазы жизненного цикла событий?</summary>

&nbsp;

Прочитать:

1. [Всплытие и погружение](https://learn.javascript.ru/bubbling-and-capturing)
2. [Event Bubbling and Event Catching in JavaScript and React – A Beginner's Guide](https://www.freecodecamp.org/news/event-propagation-event-bubbling-event-catching-beginners-guide/)

&nbsp;

</details>

<details><summary>Что такое делегирование событий?</summary>

&nbsp;

Прочитать:

1. [Делегирование событий](https://learn.javascript.ru/event-delegation)
2. [A Simple Explanation of Event Delegation in JavaScript](https://dmitripavlutin.com/javascript-event-delegation/)

&nbsp;

</details>

<details><summary>В чем отличие .getElementsByClassName от .querySelectrorAll?</summary>

&nbsp;

Прочитать:

1. [querySelector and querySelectorAll vs getElementsByClassName and getElementById in JavaScript](https://stackoverflow.com/questions/14377590/queryselector-and-queryselectorall-vs-getelementsbyclassname-and-getelementbyid)

&nbsp;

</details>

<details><summary>Как понять что DOM загружен?</summary>

&nbsp;

Прочитать:

1. [Страница: DOMContentLoaded, load, beforeunload, unload](https://learn.javascript.ru/onload-ondomcontentloaded)

&nbsp;

</details>

<details><summary>Что за событие DOM Content Loaded?</summary>

&nbsp;

Прочитать:

1. [Страница: DOMContentLoaded, load, beforeunload, unload](https://learn.javascript.ru/onload-ondomcontentloaded)

&nbsp;

</details>

<details><summary>Чем отличается событие DOM Content Loaded от load?</summary>

&nbsp;

Прочитать:

1. [Страница: DOMContentLoaded, load, beforeunload, unload](https://learn.javascript.ru/onload-ondomcontentloaded)
2. [load и DOMContentLoaded](https://doka.guide/js/event-load-and-domcontentloaded/)

&nbsp;

</details>

<details><summary>Сталкивался ли ты c shadow dom?</summary>

&nbsp;

Прочитать:

1. [Shadow DOM](https://learn.javascript.ru/shadow-dom)
2. [Shadow DOM v1 - Self-Contained Web Components](https://web.dev/shadowdom-v1/)

&nbsp;

</details>

<details><summary>Разница между event.target и event.currentTarget?</summary>

&nbsp;

Прочитать:

1. [event.target](https://learn.javascript.ru/bubbling-and-capturing#event-target)
2. [What is the exact difference between currentTarget property and target property in JavaScript](https://stackoverflow.com/questions/10086427/what-is-the-exact-difference-between-currenttarget-property-and-target-property)

&nbsp;

</details>

<details><summary>Разница между HTMLCollection и NodeList?</summary>

&nbsp;

Прочитать:

1. [В чём разница между HTMLCollection и NodeList](https://ru.hexlet.io/blog/posts/nodelist-htmlcollection)
2. [HTMLCollection vs NodeList](https://medium.com/@layne_celeste/htmlcollection-vs-nodelist-4b83e3a4fb4b)

&nbsp;

</details>

<details><summary>Как добавить элемент на HTML-страницу?</summary>

&nbsp;

Прочитать:

1. [Изменение документа](https://learn.javascript.ru/modifying-document)
2. [How to Manipulate the DOM - the Ultimate Beginner's Guide](https://www.freecodecamp.org/news/how-to-manipulate-the-dom-beginners-guide/)

&nbsp;

</details>

<details><summary>Какие есть способы добавить обработчик события на DOM-элемент?</summary>

&nbsp;

Прочитать:

1. [Обработчики событий](https://learn.javascript.ru/introduction-browser-events#obrabotchiki-sobytiy)
2. [addEventListener vs onclick](https://stackoverflow.com/questions/6348494/addeventlistener-vs-onclick)

&nbsp;

</details>

<details><summary>Сколько аргументов принимает addEventListener?</summary>

&nbsp;

Прочитать:

1. [addEventListener](https://learn.javascript.ru/introduction-browser-events#addeventlistener)
2. [EventTarget.addEventListener()](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener)

&nbsp;

</details>

<details><summary>Как удалить обработчик события с DOM-элемента?</summary>

&nbsp;

Прочитать:

1. [removeEventListener()](https://doka.guide/js/element-removeeventlistener/)
2. [EventTarget.removeEventListener()](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/removeEventListener)

&nbsp;

</details>

<details><summary>Почему нам нужно отписываться от обработчиков?</summary>

&nbsp;

Прочитать:

1. [removeEventListener()](https://doka.guide/js/element-removeeventlistener/#kak-eto-ponyat)

&nbsp;

</details>

<details><summary>Утечки памяти, что это такое и почему плохо?</summary>

&nbsp;

Прочитать:

1. [4 вида утечек памяти в JavaScript и как с ними бороться](https://habr.com/ru/post/309318/)
2. [Eradicating Memory Leaks In Javascript](https://www.lambdatest.com/blog/eradicating-memory-leaks-in-javascript/)
3. [Memory issues](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener#memory_issues)

&nbsp;

</details>

<details><summary>Как происходит процесс утечки?</summary>

&nbsp;

Прочитать:

1. [4 вида утечек памяти в JavaScript и как с ними бороться](https://habr.com/ru/post/309318/)
2. [Memory issues](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener#memory_issues)

&nbsp;

</details>

<details><summary>Как исправить утечку памяти?</summary>

&nbsp;

Прочитать:

1. [4 вида утечек памяти в JavaScript и как с ними бороться](https://habr.com/ru/post/309318/)
2. [Memory issues](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener#memory_issues)

&nbsp;

</details>

<details><summary>Способы фокусировки на элементе?</summary>

&nbsp;

Прочитать:

1. [focus()](https://doka.guide/js/element-focus/)
2. [Включаем фокусировку на любом элементе: tabindex](https://learn.javascript.ru/focus-blur#vklyuchaem-fokusirovku-na-lyubom-elemente-tabindex)

&nbsp;

</details>

<details><summary>Как закрыть модалку по клику вне нее?</summary>

&nbsp;

Прочитать:

1. [Работа с событиями мыши](https://ru.reactjs.org/docs/accessibility.html#mouse-and-pointer-events)
2. [Detect click outside div using javascript](https://stackoverflow.com/questions/36695438/detect-click-outside-div-using-javascript)
3. [How do I detect a click outside an element?](https://stackoverflow.com/questions/152975/how-do-i-detect-a-click-outside-an-element?rq=1)

&nbsp;

</details>

<details><summary>Как выполнить действие когда произошел скролл до нужного места?</summary>

&nbsp;

Прочитать:

1. [Intersection Observer API: примеры использования](https://habr.com/ru/post/494670/)
2. [How can I tell if a DOM element is visible in the current viewport?](https://stackoverflow.com/questions/123999/how-can-i-tell-if-a-dom-element-is-visible-in-the-current-viewport)
3. [An Explanation of How the Intersection Observer Watches](https://css-tricks.com/an-explanation-of-how-the-intersection-observer-watches/)
4. [Now You See Me: How To Defer, Lazy-Load And Act With IntersectionObserver](https://www.smashingmagazine.com/2018/01/deferring-lazy-loading-intersection-observer-api/)

&nbsp;

</details>

<details><summary>Как определить что элемент во вьюпорте?</summary>

&nbsp;

Прочитать:

1. [Intersection Observer API: примеры использования](https://habr.com/ru/post/494670/)
2. [How can I tell if a DOM element is visible in the current viewport?](https://stackoverflow.com/questions/123999/how-can-i-tell-if-a-dom-element-is-visible-in-the-current-viewport)
3. [An Explanation of How the Intersection Observer Watches](https://css-tricks.com/an-explanation-of-how-the-intersection-observer-watches/)
4. [Now You See Me: How To Defer, Lazy-Load And Act With IntersectionObserver](https://www.smashingmagazine.com/2018/01/deferring-lazy-loading-intersection-observer-api/)

&nbsp;

</details>

<details><summary>Как оптимизировать частый вызов обработчиков?</summary>

&nbsp;

Прочитать:

1. [Throttle на примере изменения страницы при прокрутке](https://doka.guide/js/throttle/)
2. [Debounce на примере формы поиска](https://doka.guide/js/debounce/)
3. [Difference Between throttling and debouncing a function](https://stackoverflow.com/questions/25991367/difference-between-throttling-and-debouncing-a-function)

&nbsp;

</details>

<details><summary>Методы оптимизации скролла</summary>

&nbsp;

Прочитать:

1. [Throttle на примере изменения страницы при прокрутке](https://doka.guide/js/throttle/)
2. [Virtual scrolling: Core principles and basic implementation in React](https://blog.logrocket.com/virtual-scrolling-core-principles-and-basic-implementation-in-react/)

&nbsp;

</details>

<details><summary>что такое и зачем throttling</summary>

&nbsp;

Прочитать:

1. [Throttle на примере изменения страницы при прокрутке](https://doka.guide/js/throttle/)

&nbsp;

</details>

<details><summary>что такое и зачем debouncing</summary>

&nbsp;

Прочитать:

1. [Debounce на примере формы поиска](https://doka.guide/js/debounce/)

&nbsp;

</details>

<details><summary>Что такое и зачем нужен Ajax?</summary>

&nbsp;

Прочитать:

1. [AJAX для новичков](https://habr.com/ru/post/14246/)
2. [Сетевые запросы](https://learn.javascript.ru/network)
3. [Ajax](https://developer.mozilla.org/en-US/docs/Web/Guide/AJAX)

&nbsp;

</details>

<details><summary>Приватные поля</summary>

&nbsp;

Прочитать:

1. [Приватное свойство](https://learn.javascript.ru/private-protected-properties-methods#privatnoe-svoystvo-waterlimit)
2. [JavaScript: Публичные и приватные поля классов](https://habr.com/ru/post/438202/)
3. [Private syntax FAQ](https://github.com/tc39/proposal-class-fields/blob/main/PRIVATE_SYNTAX_FAQ.md)

&nbsp;

</details>

<details><summary>Разница между JSON и XML?</summary>

&nbsp;

Прочитать:

1. [JSON и XML. Что лучше?](https://habr.com/ru/post/31225/)
2. [JSON и XML](https://webref.ru/dev/json-tutorial/json-vs-xml)

&nbsp;

</details>

<details><summary>В чем опасность работы с innerHTML?</summary>

&nbsp;

Прочитать:

1. [XSS-атаки: Что нужно использовать вместо innerHTML / insertAdjacentHTML?](https://ru.stackoverflow.com/questions/1142971/xss-%D0%B0%D1%82%D0%B0%D0%BA%D0%B8-%D0%A7%D1%82%D0%BE-%D0%BD%D1%83%D0%B6%D0%BD%D0%BE-%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D1%8C-%D0%B2%D0%BC%D0%B5%D1%81%D1%82%D0%BE-innerhtml-insertadjacenthtml)
2. [What is the Disadvantage of using innerHTML in JavaScript ?](https://www.geeksforgeeks.org/what-is-the-disadvantage-of-using-innerhtml-in-javascript/)

&nbsp;

</details>

## React

<details><summary>Что такое React?</summary>

&nbsp;

Прочитать:

1. [Зачем фронтендерам React, если есть JavaScript](https://htmlacademy.ru/blog/articles/react-js#:~:text=%D0%98%D1%82%D0%B0%D0%BA%2C%20%D0%BA%D0%B0%D0%BA%D0%B8%D0%B5%20%D1%83%20React%20%D0%BF%D1%80%D0%B5%D0%B8%D0%BC%D1%83%D1%89%D0%B5%D1%81%D1%82%D0%B2%D0%B0,JavaScript.%20%D0%A3%20React%20%D0%BE%D1%82%D0%BB%D0%B8%D1%87%D0%BD%D0%B0%D1%8F%20%D0%B4%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D0%B0%D1%86%D0%B8%D1%8F)
2. [What Is React.js? A Look at the Popular JavaScript Library](https://kinsta.com/knowledgebase/what-is-react-js/)

&nbsp;

</details>

<details><summary>Чем SPA отличается от классического сайта?</summary>

&nbsp;

Прочитать:

1. [Single-page application](https://en.wikipedia.org/wiki/Single-page_application)
2. [Single-page application vs. multiple-page application](https://medium.com/@NeotericEU/single-page-application-vs-multiple-page-application-2591588efe58)

&nbsp;

</details>

<details><summary>Что такое и зачем нужен virtual DOM?</summary>

&nbsp;

Прочитать:

1. [Немного о том, как работает виртуальный DOM в React](https://habr.com/ru/company/macloud/blog/558682/)
2. [What is a virtual DOM in React?](https://blog.logrocket.com/what-virtual-dom-react/)
3. [Exploring how virtual DOM is implemented in React](https://indepth.dev/posts/1501/exploring-how-virtual-dom-is-implemented-in-react)

&nbsp;

</details>

<details><summary>недостатки виртуального dom</summary>

&nbsp;

Прочитать:

1. [Why Virtual DOM is slower](https://medium.com/@hayavuk/why-virtual-dom-is-slower-2d9b964b4c9e)
2. [Incremental vs Virtual DOM](https://blog.bitsrc.io/incremental-vs-virtual-dom-eb7157e43dca)

&nbsp;

</details>

<details><summary>почему операции над дом деревом дорогие</summary>

&nbsp;

Прочитать:

1. [Why do developers think the DOM is slow?](https://www.reddit.com/r/javascript/comments/6115ay/why_do_developers_think_the_dom_is_slow/)
2. [But why's the browser DOM still so slow after 10 years of effort?](https://stackoverflow.com/questions/6817093/but-whys-the-browser-dom-still-so-slow-after-10-years-of-effort)

&nbsp;

</details>

<details><summary>перерисуются ли дочерние компоненты, если перерисовался родительский и почему</summary>

&nbsp;

Прочитать:

1. [A (Mostly) Complete Guide to React Rendering Behavior](https://blog.isquaredsoftware.com/2020/05/blogged-answers-a-mostly-complete-guide-to-react-rendering-behavior/)
2. [React re-renders guide: everything, all at once](https://www.developerway.com/posts/react-re-renders-guide)
3. [A Visual Guide to React Rendering - It Always Re-renders](https://alexsidorenko.com/blog/react-render-always-rerenders/)

&nbsp;

</details>

<details><summary>при перерисовке ветки в виртуальном доме что будет с этой веткой в браузерном доме</summary>

&nbsp;

Прочитать:

1. [Understanding Reconciliation: React Rendering Phases](https://dev.to/thee_divide/reconciliation-react-rendering-phases-56g2)

&nbsp;

</details>

<details><summary>расскажи про фазу согласования</summary>

&nbsp;

Прочитать:

1. [Fiber изнутри: Погружение в новый алгоритм согласования React](https://habr.com/ru/post/662549/)

&nbsp;

</details>

<details><summary>Что Такое JSX?</summary>

&nbsp;

Прочитать:

1. [Знакомство с JSX](https://ru.reactjs.org/docs/introducing-jsx.html)
2. [You don’t need React to use JSX](https://adostes.medium.com/you-dont-need-react-to-use-jsx-b78dd2a95c27)

&nbsp;

</details>

<details><summary>Что такое React Fiber?</summary>

&nbsp;

Прочитать:

1. [Fiber изнутри: Погружение в новый алгоритм согласования React](https://habr.com/ru/post/662549/)

&nbsp;

</details>

<details><summary>Что такое строгий режим в React? Его преимущества?</summary>

&nbsp;

Прочитать:

1. [Строгий режим](https://ru.reactjs.org/docs/strict-mode.html)
2. [Does strict mode work differently with React 18?](https://stackoverflow.com/questions/72112028/does-strict-mode-work-differently-with-react-18)

&nbsp;

</details>

<details><summary>Что такое синтетические события в React?</summary>

&nbsp;

Прочитать:

1. [SyntheticEvent](https://ru.reactjs.org/docs/events.html)

&nbsp;

</details>

<details><summary>Что такое условный рендеринг (Conditional Rendering)? Как его выполнить?</summary>

&nbsp;

Прочитать:

1. [Условный рендеринг](https://ru.reactjs.org/docs/conditional-rendering.html)
2. [React conditional rendering: 9 methods with examples](https://blog.logrocket.com/react-conditional-rendering-9-methods/)

&nbsp;

</details>

<details><summary>Что такое компонент?</summary>

&nbsp;

Прочитать:

1. [Компоненты и пропсы](https://ru.reactjs.org/docs/components-and-props.html)

&nbsp;

</details>

<details><summary>Разница между элементом и компонентом?</summary>

&nbsp;

Прочитать:

1. [React Element vs Component](https://www.robinwieruch.de/react-element-component/)

&nbsp;

</details>

<details><summary>Зачем мы разбиваем код на компоненты?</summary>

&nbsp;

Прочитать:

1. [When to break up a component into multiple components](https://kentcdodds.com/blog/when-to-break-up-a-component-into-multiple-components)

&nbsp;

</details>

<details><summary>Какие есть способы общения между компонентами?</summary>

&nbsp;

Прочитать:
1. [Однонаправленный поток данных](https://ru.reactjs.org/docs/state-and-lifecycle.html#the-data-flows-down)
2. [Подъём состояния](https://ru.reactjs.org/docs/lifting-state-up.html)
3. [Перенаправление рефов](https://ru.reactjs.org/docs/forwarding-refs.html)

&nbsp;

</details>

<details><summary>В чем разница между управляемыми (controlled) и не управляемыми (uncontrolled) компонентами?</summary>

&nbsp;

Прочитать:
1. [Управляемые компоненты](https://ru.reactjs.org/docs/forms.html#controlled-components)
2. [Неуправляемые компоненты](https://ru.reactjs.org/docs/uncontrolled-components.html)

&nbsp;

</details>

<details><summary>Какие методы жизненного цикла компонента существуют в React?</summary>

&nbsp;

Прочитать:
1. [Жизненный цикл компонента](https://ru.reactjs.org/docs/react-component.html#the-component-lifecycle)
2. [React 16 Lifecycle Methods: How and When to Use Them](https://blog.bitsrc.io/react-16-lifecycle-methods-how-and-when-to-use-them-f4ad31fb2282)

&nbsp;

</details>

<details><summary>Стадии жизненного цикла компонента в React?</summary>

&nbsp;

Прочитать:
1. [События жизненного цикла в React](https://frontend-stuff.com/blog/react-lifecycle-events/)
2. [The React lifecycle: methods and hooks explained](https://retool.com/blog/the-react-lifecycle-methods-and-hooks-explained/)

&nbsp;

</details>

<details><summary>Что такое PureComponent?</summary>

&nbsp;

Прочитать:
1. [React.PureComponent](https://ru.reactjs.org/docs/react-api.html#reactpurecomponent)
2. [Разбор: как и зачем применять PureComponent в React](https://habr.com/ru/company/redmadrobot/blog/318222/)

&nbsp;

</details>

<details><summary>Что такое Компонент высшего порядка (Higher-Order Component, HOC)?</summary>

&nbsp;

Прочитать:
1. [Компоненты высшего порядка](https://ru.reactjs.org/docs/higher-order-components.html)
2. [Higher-Order Components In React](https://www.smashingmagazine.com/2020/06/higher-order-components-react/)

&nbsp;

</details>

<details><summary>Что такое компонент-переключатель (Switching Component)?</summary>

&nbsp;

Прочитать:
1. [Multiple conditional renderings in React](https://www.robinwieruch.de/conditional-rendering-react/#multiple-conditional-renderings-in-react)

&nbsp;

</details>

<details><summary>в чём разница между пропсами и стейтом</summary>

&nbsp;

Прочитать:
1. [Состояние компонента](https://ru.reactjs.org/docs/faq-state.html)
2. [React Fundamentals: Props vs State](https://kentcdodds.com/blog/props-vs-state)
3. [What is the difference between state and props in React?](https://stackoverflow.com/questions/27991366/what-is-the-difference-between-state-and-props-in-react)

&nbsp;

</details>

<details><summary>Двустороннее и однонаправленное связывание данных?</summary>

&nbsp;

Прочитать:
1. [Однонаправленный поток данных](https://ru.reactjs.org/docs/state-and-lifecycle.html#the-data-flows-down)
2. [Data binding in React](https://stackoverflow.com/questions/42217579/data-binding-in-react)
3. [ReactJS Data Binding](https://www.geeksforgeeks.org/reactjs-data-binding/)
4. [Difference between One-way Binding and Two-way Binding](https://www.geeksforgeeks.org/difference-between-one-way-binding-and-two-way-binding/)

&nbsp;

</details>

<details><summary>Что такое поднятие состояния вверх (Lifting State Up)?</summary>

&nbsp;

Прочитать:
1. [Подъём состояния](https://ru.reactjs.org/docs/lifting-state-up.html)
2. [What Is "Lifting State Up" in React?](https://www.freecodecamp.org/news/what-is-lifting-state-up-in-react/)

&nbsp;

</details>

<details><summary>Как работает проп children?</summary>

&nbsp;

Прочитать:
1. [Композиция против наследования](https://ru.reactjs.org/docs/composition-vs-inheritance.html)
2. [props.children](https://ru.reactjs.org/docs/glossary.html#propschildren)

&nbsp;

</details>

<details><summary>Что такое порталы в React?</summary>

&nbsp;

Прочитать:
1. [Порталы](https://ru.reactjs.org/docs/portals.html)
2. [Building a modal in React with React Portals](https://blog.logrocket.com/build-modal-with-react-portals/)

&nbsp;

</details>

<details><summary>назови основные хуки в реакте</summary>

&nbsp;

Прочитать:
1. [Хуки](https://ru.reactjs.org/docs/react-api.html#hooks)

&nbsp;

</details>

<details><summary>назови 2 правила написания хуков</summary>

&nbsp;

Прочитать:
1. [Правила хуков](https://ru.reactjs.org/docs/hooks-rules.html)

&nbsp;

</details>

<details><summary>почему нельзя использовать хуки в условных выражениях</summary>

&nbsp;

Прочитать:
1. [Объяснение](https://ru.reactjs.org/docs/hooks-rules.html#explanation)

&nbsp;

</details>

<details><summary>Разница между useEffect() и componentDidMount()?</summary>

&nbsp;

Прочитать:
1. [Подробное объяснение](https://ru.reactjs.org/docs/hooks-effect.html#detailed-explanation)
2. [useEffect(fn, []) is not the new componentDidMount()](https://reacttraining.com/blog/useEffect-is-not-the-new-componentDidMount/)

&nbsp;

</details>

<details><summary>Как реализовать однократное выполнение операции при начальном рендеринге?</summary>

&nbsp;

Прочитать:
1. [useEffect](https://ru.reactjs.org/docs/hooks-reference.html#useeffect)

&nbsp;

</details>

<details><summary>В чём разница между useEffect и useLayoutEffect?</summary>

&nbsp;

Прочитать:
1. [useEffect vs useLayoutEffect](https://kentcdodds.com/blog/useeffect-vs-uselayouteffect)

&nbsp;

</details>

<details><summary>Зачем в setState() нужно передавать функцию?</summary>

&nbsp;

Прочитать:
1. [Функциональные обновления](https://ru.reactjs.org/docs/hooks-reference.html#functional-updates)

&nbsp;

</details>

<details><summary>Зачем нам нужен менеджер состояния?</summary>

&nbsp;

Прочитать:
1. [How to Manage State in Your React Apps](https://www.freecodecamp.org/news/how-to-manage-state-in-your-react-apps/)
2. [Application State Management with React](https://kentcdodds.com/blog/application-state-management-with-react)

&nbsp;

</details>

<details><summary>Как определить что состояние является глобальным?</summary>

&nbsp;

Прочитать:
1. [Global vs Local State in React](https://dev.to/fkrasnowski/global-vs-local-state-in-react-lp5)
2. [How to Manage State in Your React Apps](https://www.freecodecamp.org/news/how-to-manage-state-in-your-react-apps/)

&nbsp;

</details>

<details><summary>Почему нельзя использовать контекст в качестве хранилища состояния?</summary>

&nbsp;

Прочитать:
1. [How to use React Context effectively](https://kentcdodds.com/blog/how-to-use-react-context-effectively)

&nbsp;

</details>

<details><summary>Что такое серверный рендеринг (SSR)?</summary>

&nbsp;

Прочитать:
1. [Rendering on the Web](https://web.dev/rendering-on-the-web/)
2. [Server Side Rendering (SSR) vs. Client Side Rendering (CSR) vs. Pre-Rendering using Static Site Generators (SSG) and client-side hydration](https://medium.com/@prashantramnyc/server-side-rendering-ssr-vs-client-side-rendering-csr-vs-pre-rendering-using-static-site-89f2d05182ef)

&nbsp;

</details>

<details><summary>В чем заключаются недостатки SSR?</summary>

&nbsp;

Прочитать:
1. [Server Side Rendering (SSR) vs. Client Side Rendering (CSR) vs. Pre-Rendering using Static Site Generators (SSG) and client-side hydration](https://medium.com/@prashantramnyc/server-side-rendering-ssr-vs-client-side-rendering-csr-vs-pre-rendering-using-static-site-89f2d05182ef)

&nbsp;

</details>

<details><summary>Какие есть альтернативы SSR?</summary>

&nbsp;

Прочитать:
1. [Rendering Patterns](https://www.patterns.dev/posts/#rendering-patterns)

&nbsp;

</details>

<details><summary>Что такое двустороннее связывание?</summary>

&nbsp;

Прочитать:
1. [Однонаправленный поток данных](https://ru.reactjs.org/docs/state-and-lifecycle.html#the-data-flows-down)
2. [Data binding in React](https://stackoverflow.com/questions/42217579/data-binding-in-react)
3. [ReactJS Data Binding](https://www.geeksforgeeks.org/reactjs-data-binding/)
4. [Difference between One-way Binding and Two-way Binding](https://www.geeksforgeeks.org/difference-between-one-way-binding-and-two-way-binding/)

&nbsp;

</details>

<details><summary>Зачем нам нужен механизм двустороннего связывания?</summary>

&nbsp;

Прочитать:
1. [Однонаправленный поток данных](https://ru.reactjs.org/docs/state-and-lifecycle.html#the-data-flows-down)
2. [Data binding in React](https://stackoverflow.com/questions/42217579/data-binding-in-react)
3. [ReactJS Data Binding](https://www.geeksforgeeks.org/reactjs-data-binding/)
4. [Difference between One-way Binding and Two-way Binding](https://www.geeksforgeeks.org/difference-between-one-way-binding-and-two-way-binding/)

&nbsp;

</details>

<details><summary>Рассажи кратко как сделать бесконечный скролл</summary>

&nbsp;

Прочитать:
1. [React: How to implement an infinite scroll](https://medium.com/suyeonme/react-how-to-implement-an-infinite-scroll-749003e9896a)
2. [React Hooks for infinite scroll: An advanced tutorial](https://blog.logrocket.com/react-hooks-infinite-scroll-advanced-tutorial/)

&nbsp;

</details>

<details><summary>что такое virtual scroll</summary>

&nbsp;

Прочитать:
1. [Virtual scrolling: Core principles and basic implementation in React](https://blog.logrocket.com/virtual-scrolling-core-principles-and-basic-implementation-in-react/)
2. [React Virtuoso](https://virtuoso.dev/)
3. [react-virtualized](https://github.com/bvaughn/react-virtualized)
4. [react-window](https://github.com/bvaughn/react-window)

&nbsp;

</details>

<details><summary>какой атрибут нужно дополнительно указывать и зачем, когда рендеришь список в реакте</summary>

&nbsp;

Прочитать:
1. [Списки и ключи](https://ru.reactjs.org/docs/lists-and-keys.html)
2. [React key attribute: best practices for performant lists](https://www.developerway.com/posts/react-key-attribute)

&nbsp;

</details>

<details><summary>какой единственный классовый компонент до сих активно используется</summary>

&nbsp;

Прочитать:
1. [Предохранители](https://ru.reactjs.org/docs/error-boundaries.html)

&nbsp;

</details>

<details><summary>что такое Props drilling</summary>

&nbsp;

Прочитать:
1. [Prop Drilling](https://kentcdodds.com/blog/prop-drilling)

&nbsp;

</details>

<details><summary>в каких случаях использовать рефы</summary>

&nbsp;

Прочитать:
1. [Рефы и DOM](https://ru.reactjs.org/docs/refs-and-the-dom.html)
2. [A complete guide to React refs](https://blog.logrocket.com/complete-guide-react-refs/)

&nbsp;

</details>

<details><summary>Что такое flushSync в Реакте</summary>

&nbsp;

Прочитать:
1. [flushSync](https://ru.reactjs.org/docs/react-dom.html#flushsync)
2. [What does flushSync() do in React?](https://stackoverflow.com/questions/62725935/what-does-flushsync-do-in-react)

&nbsp;

</details>

<details><summary>Что такое lazy loading?</summary>

&nbsp;

Прочитать:
1. [Разделение кода](https://ru.reactjs.org/docs/code-splitting.html)

&nbsp;

</details>

<details><summary>Вто такое инверсия наследования (Inheritance Inversion)?</summary>

&nbsp;

Прочитать:
1. [How to develop your React superpowers with the HOC Pattern](https://www.freecodecamp.org/news/how-to-develop-your-react-superpowers-with-the-hoc-pattern-61293651d59/)
2. [Higher-Order Component in React](https://blog.devgenius.io/higher-order-component-in-react-2bed7b6053f0)

&nbsp;

</details>

<details><summary>Для чего предназначен метод registerServiceWorker() в React?</summary>

&nbsp;

Прочитать:
1. [What does registerServiceWorker do in React JS?](https://stackoverflow.com/questions/47953732/what-does-registerserviceworker-do-in-react-js)

&nbsp;

</details>

## Web API

<details><summary>Что такое HTTP?</summary>
      
&nbsp;
    
Прочитать:
1. [Протокол HTTP](https://doka.guide/tools/http-protocol/)
2. [Простым языком об HTTP](https://habr.com/ru/post/215117/)
3. [Hypertext Transfer Protocol](https://en.wikipedia.org/wiki/Hypertext_Transfer_Protocol)
      
&nbsp;
     
 
</details>
    
<details><summary>Структура HTTP запроса?</summary>
    
&nbsp;
  
Прочитать:
1. [Структура HTTP-сообщения](https://ru.wikipedia.org/wiki/HTTP#%D0%A1%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B0_HTTP-%D1%81%D0%BE%D0%BE%D0%B1%D1%89%D0%B5%D0%BD%D0%B8%D1%8F)
    
&nbsp;
   
</details>
    
<details><summary>Какие методы может иметь HTTP-запрос?</summary>
    
&nbsp;
  
Прочитать:
1. [Методы HTTP](https://ru.wikipedia.org/wiki/HTTP#%D0%9C%D0%B5%D1%82%D0%BE%D0%B4%D1%8B)
    
&nbsp;
   
</details>
    
<details><summary>В чем принципиальная разница между POST и GET?</summary>
    
&nbsp;
  
Прочитать:
1. [Чем отличаются HTTP-методы GET и POST](https://htmlacademy.ru/blog/php/get-vs-post)
2. [GET vs. POST](https://www.diffen.com/difference/GET-vs-POST-HTTP-Requests)
    
&nbsp;
   
</details>
    
<details><summary>Можем ли мы закешировать POST запрос?</summary>
    
&nbsp;
  
Прочитать:
1. [Is it possible to cache POST methods in HTTP?](https://stackoverflow.com/questions/626057/is-it-possible-to-cache-post-methods-in-http)
    
&nbsp;
   
</details>
    
<details><summary>Что такое коды ответа сервера и чем они отличаются друг от друга?</summary>
    
&nbsp;
  
Прочитать:
1. [Список кодов состояния HTTP](https://ru.wikipedia.org/wiki/%D0%A1%D0%BF%D0%B8%D1%81%D0%BE%D0%BA_%D0%BA%D0%BE%D0%B4%D0%BE%D0%B2_%D1%81%D0%BE%D1%81%D1%82%D0%BE%D1%8F%D0%BD%D0%B8%D1%8F_HTTP)
    
&nbsp;
   
</details>
    
<details><summary>Чем отличается http от https?</summary>
    
&nbsp;
  
Прочитать:
1. [Как HTTPS обеспечивает безопасность соединения: что должен знать каждый Web-разработчик](https://habr.com/ru/post/188042/)
2. [HTTPS](https://en.wikipedia.org/wiki/HTTPS)
3. [HTTP vs HTTPS – What's the Difference?](https://www.freecodecamp.org/news/http-vs-https/)
    
&nbsp;
   
</details>
    
<details><summary>Можем ли мы запустить http2 без https?</summary>
    
&nbsp;
  
Прочитать:
1. [HTTP/2](https://en.wikipedia.org/wiki/HTTP/2#Encryption)
    
&nbsp;
   
</details>
    
<details><summary>Почему повсеместно нужен https?</summary>
    
&nbsp;
  
Прочитать:
1. [Как HTTPS обеспечивает безопасность соединения: что должен знать каждый Web-разработчик](https://habr.com/ru/post/188042/)
2. [HTTPS](https://en.wikipedia.org/wiki/HTTPS)
    
&nbsp;
   
</details>
    
<details><summary>Что дает https помимо шифрования?</summary>
    
&nbsp;
  
Прочитать:
1. [Google HTTPS Ranking: Why SSL is Good for SEO](Google HTTPS Ranking: Why SSL is Good for SEO)
    
&nbsp;
   
</details>
    
<details><summary>Можем ли мы получить картинку по HTTP?</summary>
    
&nbsp;
  
Прочитать:
1. [MIME types](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)
    
&nbsp;
   
</details>
    
<details><summary>Как мы можем подсказать браузеру подготовиться к загрузке ресурсов?</summary>
    
&nbsp;
  
Прочитать:
1. [Preload, prefetch и другие теги](https://habr.com/ru/post/445264/)
    
&nbsp;
   
</details>
    
<details><summary>Влияет ли скорость ответа сервера на скорость загрузки сайта?</summary>
    
&nbsp;
  
Прочитать:
1. [Время до первого байта: что это такое и почему это важно](https://habr.com/ru/company/ruvds/blog/470868/)
    
&nbsp;
   
</details>
    
<details><summary>Как браузер понимает что ресурс нужно закешировать?</summary>
    
&nbsp;
  
Прочитать:
1. [HTTP caching](https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching)
2. [A Web Developer’s Guide to Browser Caching](https://medium.com/@codebyamir/a-web-developers-guide-to-browser-caching-cc41f3b73e7c)
    
&nbsp;
   
</details>
    
<details><summary>Зачем нужен хеш в названиях файлов?</summary>
    
&nbsp;
  
Прочитать:
1. [Why is including a hash in a filename better for caching than appending a timestamp as a query parameter?](https://stackoverflow.com/questions/25557631/why-is-including-a-hash-in-a-filename-better-for-caching-than-appending-a-timest)
    
&nbsp;
   
</details>
    
<details><summary>Как браузер понимает что картинка является картинкой?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Какими способами мы можем получить картинку с сервера?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Каким образом браузер понимает тип содержимого в ответе от API(картинка, текст, etc)?</summary>
  
&nbsp;

Прочитать:
  
&nbsp;
  
</details>
  
<details><summary>Как браузер понимает что нужно загрузить картинку?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Как браузер понимает что нужно отображать именно картинку а не текст?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое CORS?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Какие способы авторизации ты знаешь?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>что будет если авторизацию сделать через GET</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>почему форму с паролем нельзя отправить GET запросом</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Какой будет запрос для подтверждения регистрации пользователя?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое JWT?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое refresh токен?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Как защититься от парсинга?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>почему картинки загружаются через GET, а не через POST</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Отличия http2 от http1</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Протоколы взаимодействия с беком</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>расскажи зачем заголовок Referrer</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое и чем опасен XSS?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое CSRF?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>что такое csrf токен</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Как обезопасить себя от потенциально опасного клиентского ввода?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Есть ли уязвимость связанная с \_target =blank?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое прогрессивная отрисовка?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Разница между Progressive Enhancement и Graceful Degradation?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Разница между feature detection, feature inference и анализом строки user-agent?</summary>
  
&nbsp;

Прочитать:
  
&nbsp;
  
</details>
  
<details><summary>Что такое Веб-компоненты и какие технологии в них используются?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Способы уменьшения времени загрузки веб-страницы?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое Progressive Web Application?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>что такое сервис воркеры</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое Web Workers?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>расскажи про repaint и reflow</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>расскажи про restyle и relayout</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>что такое Layout trashing</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое Flash Of Unstyled Content?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>можно ли вставить счётчик в виде картинки</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>как сделать так, чтобы картинка, которая кэшируется обновлялась</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>какие есть способы хранения данных в браузере</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>в чём отличие localStorage от sessionStorage</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое IndexedDB в браузере?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что мы можем делать с помощью devtools браузера?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое HTTP cookie? Для чего они используются?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Разница между cookie, sessionStorage и localStorage?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Как защитить cookie?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое WebSocket? В чем принцип его работы?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое безопасные (Secure) и HttpOnly cookies?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое Content Security Policy (CSP)?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Как работает JSONP?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое History API в браузере?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое BOM?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>назвать способы оптимизации загрузки страниц сайта</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>рассказать об инструментах, которые можно использовать для анализа оптимизаций</summary>
  
&nbsp;

Прочитать:
  
&nbsp;
  
</details>
  
<details><summary>Как мы можем оптимизировать отрисовку?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое force layout и почему это плохо?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Как работает hot reload?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
<details><summary>Что такое Веб-компоненты и какие технологии в них используются?</summary>
    
&nbsp;
  
Прочитать:
    
&nbsp;
   
</details>
    
## Git

<details><summary>Зачем нужна система контроля версий?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Что такое gitflow?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Что такое merge и rebase, в чем отличие друг от друга?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Как наши изменения попадают в ветку?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Как можно заставить git что-то забыть?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Как можно переименовать коммит?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>В чем отличие amend от squash?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Что такое cherry-pick?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Что такое семантические коммиты?</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

<details><summary>Что ты знаешь про semantic version</summary>

&nbsp;
  
Прочитать:
  
&nbsp;
 
</details>

