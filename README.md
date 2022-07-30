# Вопросы для собеседования на позицию фронтенд разработчик

## Секция 1. Вопросы по HTML

  <details><summary>Что такое и зачем нужен HTML?</summary>
  &nbsp;

  HTML (от англ. *HyperText Markup Language* — «язык гипертекстовой разметки») - это код, который используется для структурирования веб-страницы и её контента. HTML предоставляет средства для создания заголовков, абзацев, списков, ссылок, цитат и других элементов. Элементы HTML выделяются тегами, записанными с использованием угловых скобок. Например, ```<img />```, ```<input />``` или ```<p>```.
  
  Почитать:
  1. [Основы HTML](https://developer.mozilla.org/ru/docs/Learn/Getting_started_with_the_web/HTML_basics)
  2. [Основы HTML](https://html5book.ru/osnovy-html/)
  3. [Learn HTML Basics for Beginners in Just 15 Minutes](https://www.freecodecamp.org/news/html-basics-for-beginners/)
  
  &nbsp;
</details>
  <details><summary>Что такое doctype и зачем он нужен?</summary>
  
  &nbsp;
  
  Тег DOCTYPE сообщает браузеру какую версию HTML вы используете. DOCTYPE должен находиться на первой строке каждого HTML документа. В HTML5 декларация типа документа выглядит очень просто: ```<!DOCTYPE html>```
  
  Почитать:
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
    
  Почитать:
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
  
  Почитать:
  1. [Атрибуты и свойства](https://learn.javascript.ru/dom-attributes-and-properties)
  2. [Атрибуты и свойства элементов документа ](https://flagman.top/css/atributy-i-svojstva)
  3. [Element](https://doka.guide/js/element/)
  
  &nbsp;
  
</details>
  <details><summary>Что такое мета-теги?</summary>

  &nbsp;
  
  Мета-теги позволяют передавать поисковым системам дополнительную информацию о страницах, на которых они размещены.
  
  Почитать:
  1. [Meta Tags for SEO: A Simple Guide for Beginners](https://ahrefs.com/blog/seo-meta-tags/)
  2. [Meta Tags: The Definitive Guide to Meta-Data for SEO (2021)](https://seosherpa.com/meta-tags/)
  3. [meta](https://doka.guide/html/meta/)
  
  &nbsp;

</details>
  <details><summary>Что описывается в теге head?</summary>
  
  &nbsp;
  
  Тег ```head``` предназначен для хранения служебной информации о странице. Он располагается перед ```body```. Внутри ```head``` обычно содержится заголовок и описание страницы, подключаются внешние ресурсы, например, стили. Содержимое этого тега не отображается на странице напрямую.
  
  Почитать:
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
  
  1. [Метатег viewport: почему он важен и как его правильно использовать](https://timeweb.com/ru/community/articles/metateg-viewport-pochemu-on-vazhen-i-kak-ego-pravilno-ispolzovat)
  2. [Viewport meta tag](https://developer.mozilla.org/en-US/docs/Web/HTML/Viewport_meta_tag)
  
  &nbsp;
 
  </details>
  <details><summary>Что такое html entities?</summary>
    
  &nbsp;
  
  HTML-сущности — это части текста ("строки"), которые начинаются с символа амперсанда (&) и заканчиваются точкой с запятой (;). Некоторые специальные символы, если они появляются в документе HTML, могут вызвать недопонимание в синтаксическом анализаторе исходного кода HTML, например, символ "меньше" ( < ), при встрече с данным символом анализатор HTML может ошибочно принять этот символ за тег. Чтобы избежать данное недопонимание, можно использовать специальный объект (entity) &lt; чтобы заменить символ ( < ).
  
  Почитать:
  1. [Мнемоники в HTML](https://ru.wikipedia.org/wiki/%D0%9C%D0%BD%D0%B5%D0%BC%D0%BE%D0%BD%D0%B8%D0%BA%D0%B8_%D0%B2_HTML)
  
  &nbsp;
 
  </details>
  <details><summary>Где можно найти списки с html entities? </summary>
  
  
    Списки html сущностей можно найти [в спецификации](https://html.spec.whatwg.org/multipage/named-characters.html) или [в Википедии](https://ru.wikipedia.org/wiki/%D0%9C%D0%BD%D0%B5%D0%BC%D0%BE%D0%BD%D0%B8%D0%BA%D0%B8_%D0%B2_HTML).
    
  
  </details>
  <details><summary>Что такое data атрибуты?</summary>

  &nbsp;
  
  data-* атрибуты позволяют хранить дополнительную информацию в стандартных элементах HTML без визуального представления. 
  
  Почитать:
  1. [Полное руководство по HTML-атрибутам data-*](https://habr.com/ru/company/ruvds/blog/490626/)
  2. [.dataset](https://doka.guide/js/element-dataset/)
  
  &nbsp;

</details>
  <details><summary>Откуда берутся пробелы в HTML?</summary>

  &nbsp;
  
  Элемент со значением ```display: inline-block``` ведет себя, как обычная буква и простой текст — имеет пробелы между словами. Браузер создаёт пустой текстовый узел, который, по сути, может являться переводом строки, пробелом или табом. Все и эти перечисленные вещи превращаются в один единственный пробел и описывается следующей сущностью: &#x0020. Удалить пробелы можно удалив пробелы между HTML элементами.
  
  Прочитать:
  1. [«Загадочные отступы» между инлайн-элементами (+прочитать обсуждение под статьей)](https://habr.com/ru/post/137582/)
  1. [Fighting the Space Between Inline Block Elements](https://css-tricks.com/fighting-the-space-between-inline-block-elements/)
  2. [How whitespace is handled by HTML, CSS, and in the DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Whitespace)
  
  &nbsp;
  
</details>
  <details><summary>Типы input элементов в HTML?</summary>
  
  &nbsp;
  
  ```input``` — это контейнер для интерактивных элементов, с помощью которых пользователь может ввести данные, что-то выбрать, поставить галочку или нажать кнопку.
  Атрибут type указывает на его тип. Тип элемента определяет его отображение и функционал. Например, type="text" - текстовое поле, type="submit" - кнопка отправки, type="radio" - переключатель, type="checkbox" - чек-бокс, type="hidden" - скрытое поле, type="password" - пароль и т.д.
  
  Почитать:
  1. [Многогранный тег input](https://doka.guide/html/input/)
  2. [<input> MDN](https://developer.mozilla.org/ru/docs/Web/HTML/Element/Input)
  
  &nbsp;
  
  </details>
  <details><summary>Какие глобальные атрибуты есть в HTML?</summary>
    
  &nbsp;
  
  Глобальные атрибуты - атрибуты, которые могут быть использованы со всеми HTML элементами.
  
  Почитать:
  1. [Глобальные атрибуты](https://developer.mozilla.org/ru/docs/Web/HTML/Global_attributes)
  2. [HTML-атрибуты](https://html5book.ru/html-attributes/)
  
  &nbsp;
  
  </details>
  
  
  <details><summary>Почему у разных тегов есть одни и теже свойства?</summary>
  
  &nbsp;
  
  Интерфейс Element представляет собой один из объектов в Document. Этот интерфейс описывает методы и свойства, общие для всех видов элементов. Конкретные модели поведения описаны в интерфейсах, которые наследуют от Element, и добавляют дополнительную функциональность.
Например, интерфейс HTMLElement является базовым интерфейсом для HTML-элементов, SVGElement (en-US) является основой для всех SVG-элементов.
  
  Почитать:
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
  
  Почитать:
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

Почитать:
  1. [Что такое доступность?](https://developer.mozilla.org/ru/docs/Learn/Accessibility/What_is_accessibility)
  2. [Web Almanac - Accessibility](https://almanac.httparchive.org/en/2019/accessibility)
  3. [Semantic HTML: the foundation of web accessibility](https://uxdesign.cc/semantic-html-the-foundation-of-web-accessibility-e5bbecad7c17)
  &nbsp;
  
  
  </details>
  <details><summary>Как мы можем семантически разделять контент на странице?</summary>
    
  &nbsp;
  
  HTML5 предлагает набор секционных (структурных) элементов, используя которые вы добавляете смысловую или семантическую нагрузку своим страницам, тем самым позволяя компьютерным программам лучше понимать их содержание.
  
  1. [Как использовать секционные элементы HTML5](https://habr.com/ru/post/214407/)
  2. [How to Section Your HTML](https://css-tricks.com/how-to-section-your-html/)
  
  &nbsp;
  
  </details>
  <details><summary> Почему это не очень правильно вместо тегов section и header использовать обычный div?</summary>
    
  &nbsp;
  
  Такие теги, как: header, footer, aside, h1, nav, ul и другие, помогают людям с ограниченными возможностями воспринимать сайт полностью без проблем. Так же используя семантические теги вы показываете поисковому роботу структуру сайта, где у вас шапка сайта, где подвал, а где основной контент страницы.
  
  Почитать:
  1. [Что такое доступность?](https://developer.mozilla.org/ru/docs/Learn/Accessibility/What_is_accessibility)
  2. [How to Section Your HTML](https://css-tricks.com/how-to-section-your-html/)
  
  &nbsp;
  
  </details>
  <details><summary>в чём отличие article от section</summary>
    
  &nbsp;
  
  1. [Структура HTML5 — div, section и article](https://noteskeeper.ru/heritage/54/)
  2. [Difference between article tag and section tag](https://www.geeksforgeeks.org/difference-between-article-tag-and-section-tag/)
  2. [Why You Should Choose HTML5 article Over section](https://www.smashingmagazine.com/2020/01/html5-article-section/)
  
  &nbsp;
  
  </details>
  <details><summary>Как семантически правильно сверстать картинку с подписью?</summary>

  &nbsp;
  
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
    2. [Alt-texts: The Ultimate Guide](https://axesslab.com/alt-texts/)
  
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
  
  1. [Learn Forms](https://web.dev/learn/forms/)
  2. [Best Practices for Form Design: Structure, Inputs, Labels and Actions](https://xd.adobe.com/ideas/principles/web-design/best-practices-form-design/)
  3. [Creating Accessible Forms](https://webaim.org/techniques/forms/)
  4. [Best Practices For Mobile Form Design](https://www.smashingmagazine.com/2018/08/best-practices-for-mobile-form-design/)
  
  &nbsp;
  
  </details>
  <details><summary>С помощью каких тегов ты будешь делать html форму?</summary>
    
  &nbsp;
  
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
  
  >
  
  </details>
  <details><summary>Что такое HTML валидация? И какие типы проверок HTML документа вы знаете?</summary>
    
  &nbsp;
  
  
  
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
  
  Почитать:
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
  
  
  
  &nbsp;
  
  </details>
  


## Секция 2. Вопросы по CSS
- Как расшифровывается аббревиатура CSS?
- Как ты понимаешь что такое каскад?
- что такое блочная модель
- значения box-sizing и чем они отличаются
- Как работает наследование в CSS?
- Способы изоляции стилей в CSS?
- Какие знаешь подходы по написанию CSS?
- Почему плохо писать все стили в одном файле или теге style?
- В чем отличия разных подходов подключения стилей?
- рассказать о достоинствах и недостатках подхода CSS-in-JS
- рассказать о критическом css
- Специфичность в CSS
- зачем иногда селектора перечисляют через запятую?
- Как в CSS работают разные приоритеты стилей?
- Рассказать про схлопывание марджинов
- Что такое адаптивная верстка?
- Как ты знаешь подходы по созданию адаптивных сайтов?
- рассказать о подходах mobile-first и desktop-first
- Использовал ли ты media запросы?
- Какими параметрами нужно манипулировать чтобы адаптировать сайт?
- В чем отличие адаптивного дизайна от отзывчивого?
- Проблема адаптации таблицы?
- Что ты знаешь о БЭМ?
- Какие способы выровнить элемент по горизонтали и вертикали ты знаешь?
- способы, чтобы задать расстояние между несколькими колонками
- Как растянуть элемент на 100%?
- Что такое псевдоэлементы?
- Что такое псевдоклассы?
- Как сбросить фон у элемента?
- Ключевое отличие гридов от флексов
- Объясни для каких задач подойдут флексы, а для каких гриды
- Рассказажи какие бывают значения у свойства display?
- Чем отличается блочный от инлайнового элемента?
- Рассказажи какие бывают значения у свойства position?
- Что такое position: sticky?
- Как бы ты эмулировал поведение position: sticky?
- Расскажи про поведение top,left,bottom,right при различных значениях position
- что будет когда position absolute внутри position absolute?
- Какие есть способы подключения шрифтов?
- С какими проблемами ты сталкивался при подключении кастомных шрифтов?
- в чём отличие вариативных шрифтов от обычных
- Назови способы оптимизации шрифтов
- Назови способы оптимизации иконок
- Расскажи какие форматы графических изображений ты знаешь
- Какой популярный браузер только недавно начал поддерживать webp?
- Зачем нужно указывать ширину и высоту для картинок?
- Как мы можем сделать webp с фолбеком?
- Что ты знаешь про концепцию optimistic ui?
- Можно ли с помощью JS поменять значение псевдоэлемента?
- Как можно скрыть элемент не используя display: none?
- как скрыть элемент, но чтобы поисковики его видели?
- Какие еще есть свойства для скрытия элемента? 
- Как найти все скрытые элементы на странице?
- Как ты стилизуешь чекбоксы, инпуты etc? 
- Что такое User agent стили
- Импорты и модульность в CSS
- Какие препроцессоры ты используешь или знаешь?
- Для чего ты используешь SASS?
- Минус использование амперсанда в препроцессорах?
- Как мы можем заставить элемент быть поверх другого?
- Что такое и когда создаётся новый контекс наложения?
- Как бороться с переполнением контентом?
- Какие есть единицы измерения в CSS?
- Когда брать абсолютные величины а когда относительные?
- Какие есть варианты указания цвета и зачем нам столько?
- Какие есть способы модификации цвета?
- Особенности свойства color?
- Какое количество цветов поддерживает GIF?
- Доступность цвета
- Что такое вендорные префиксы? И для чего они используются?
- Зачем нам нужен autoprefixer?
- Как автопрефиксер понимает где поставить префиксы?
- Как выбирать свойство основываясь на поддержке браузерами?
- что за свойство isolation в css
- какие в CSS есть ключевые слова (initial, inherit, unset, revert)
- что такое функция attr
- Разница между Reset.css и Normalize.css?
- Разница между margin и padding?
- Что такое CSS спрайт и для чего он используется
- Что такое #shadow-root в инспекторе HTML-страницы?


## Секция 3. Вопросы по JavaScript
  - Какие типы данных есть в JS?
  - Разница между null и undefined?
  - Мутабельные и имутабельные типы данных
  - Какие есть типы переменных?
  - в каких случаях можно изменить значение в const
  - Что такое поднятие (Hoisting)?
  - Чему равен и какой тип у NaN?
  - почему typeof NaN - число?
  - Зачем нужна блочная область видимости если уже есть функциональная?
  - Какие есть операторы в JS?
  - Чем отличаются друг от друга унарные, бинарные и тернарные операторы?
  - Какие есть операторы сравнения?
  - Разница между == и === (нестрогое/строгое равенство)?
  - Чем отличается null и undefined?
  - В чем есть особенность у логических операторы?
  - В чем особенность выполнения логического "И"
  - Какие есть falsy значения?
  - Особенности оператора &&
  - Зачем нужен use strict?
  - Что такое Map и Set?
  - Какие есть и как работают циклы в JS?
  - В чем разница циклов for .. in и for .. of?
  - Что за метод hasOwnProperty?
  - Можем ли мы создать объект который будет себя иначе вести в for of?
  - Отличие цикла for от while? 
  - Разница между forEach и map?
  - как работают методы reduce и filter
  - как проверить что массив это массив
  - Как можно добавить элемент в начало и в конец массива?
  - Какие ты знаешь способы клонирования объектов?
  - Для чего используется оператор !! (двойного отрицания)?
  - Разница между Rest и Spread операторами?
  - Как можно работать с датами в JS?
  - Можем ли мы замерить скорость работы участка кода с Date.now?
  - Что такое function expression и function declaration?
  - Что такое чистая функция?
  - Что такое функция первого порядка?
  - Что такое псевдомассив arguments?
  - Что такое рекурсия?
  - Что такое замыкание? 
  - Что такое контекст у функции?
  - Какой контекст у стрелочных функций?
  - Как мы можем изменить контекст у функции? 
  - В чём разница между bind, call, apply?
  - Что будет если забиндить два контекста подряд?
  - Чем область видимости отличается от контекста?
  - Как передаются параметры в функцию: по ссылке или по значению?
  - что такое каррирование?
  - что такое частичное применение?
  - Что такое eval и почему его следует избегать?
  - Что такое регулярное выражение (Regular Expression)?
  - Что такое цепочка вызовов функций (chaining)?
  - Что такое генераторы? Когда стоит использовать генераторы?
  - Разница между host-объектами и нативными объектами?
  - Что такое объектная обертка (Wrapper Objects)?
  - Как работает boxing/unboxing в JavaScript?
  - Что такое прототипы и прототипное наследование?
  - что такое __proto__
  - Что происходит когда мы пишем ключевое слово new? 
  - Откуда у примитива появляются методы? (.toSting(), etc...)
  - Как бы ты добавлял статический метод в prototype?
  - Почему патчинг прототипа это плохо?
  - Откуда берется свойство length у массива?
  - Как сделать какое либо свойство объекта неизменяемым?
  - Как можно запретить изменение объекта?
  - Разниц между Object.freeze() и Object.seal()?
  - Разница между typeof и instanceof?
  - Как работает метод Object.create()?
  - Как объекты преобразовываются в примитивы?
  - Знаешь ли что такое event loop?
  - Что такое и как работоают ES модули?
  - В чем разница между ES и commonjs модулями?
  - Можем ли мы поменять переменную в модуле извне?
  - Как мы можем эмулировать модули не используя ES modules/require?
  - что такое iife?
  - В чем смысл оборачивания всего содержимого JavaScript-файла в функцию?
  - Что такое и как работает Promise?
  - как увидеть какой статус у промиса
  - какие методы есть у промисов?
  - что будет, если в промисе вызвать несколько резолвов подряд?
  - В чём разница между макро- и микро- тасками
  - что такое async/await
  - Что такое Callback Hell?
  - В чём отличия между setTimeOut и setInterval
  - Что такое сборщик мусора?
  - Можем ли мы повлиять на сборку мусора?
  - Как мы будем через JS анимировать что либо?
  - Расскажи про реквест анимашн фрейм
  - Зачем нужны сборщики во фронтенде?
  - Как ты понимаешь что код написан хорошо?
  - Зачем нужен REST?
  - Что такое ООП?
  - Чем ООП в JS отличается от ООП в других языках?
  - В чем заключается отличие классов в JS от классов в других языках?
  - Какие еще знаешь парадигмы программирования?
  - Чем описание класса отличается от экземпляра класса?
  - Что такое SOLID?
  - Что такое CQRS? 
  - Что такое GRASP?
  - Что такое DRY, KISS? 
  - Пишешь ли тесты и что о них знаешь?
  - Что такое полифил (polyfill)?
  - Что такое временная мёртвая зона (temporal dead zone)?
  - Плюсы и минусы BFF (Backend for Frontend)
  - Что такое Babel и для чего он используется?

## JavaScript в браузере
  - Что такое DOM?
  - Пропадет ли DOM если мы отключим JS?
  - Что такое всплытие событий и какие у него есть фазы?
  - Что такое делегирование событий?
  - В чем отличие .getElementsByClassName от .querySelectrorAll?
  - Как понять что DOM загружен?
  - Что за событие DOM Content Loaded? 
  - Чем отличается событие DOM Content Loaded от load?
  - Сталкивался ли ты c shadow dom?
  - Разница между event.target и event.currentTarget?
  - Разница между HTMLCollection и NodeList?
  - Как динамически добавить элемент на HTML-страницу?
  - Какие есть способы добавить обработчик события на DOM-элемент?
  - Сколько аргументов принимает addEventListener?
  - Как удалить обработчик события с DOM-элемента?
  - Почему нам нужно отписываться от обработчиков?
  - Утечки памяти, что это такое и почему плохо?
  - Как происходит процесс утечки?
  - Как исправить утечку памяти?
  - Способы фокусировки на элементе?
  - Как закрыть модалку по клику вне нее?
  - Как выполнить действие когда произошел скролл до нужного места? 
  - Как определить что элемент во вьюпорте?
  - Как оптимизировать частый вызов обработчиков?
  - Методы оптимизации скролла 
  - что такое и зачем throttling
  - что такое и зачем debouncing
  - Что такое и зачем нужен Ajax?
  - Приватные поля в браузере
  - Разница между JSON и XML?
  - В чем опасность работы с innerHTML? 
  
  
## React
  - Что такое React?
  - Чем SPA отличается от классического сайта?
  - Что такое и зачем нужен virtual DOM?
  - недостатки виртуального dom
  - почему операции над дом деревом дорогие
  - перерисуются ли дочерние компоненты, если перерисовался родительский и почему
  - при перерисовке ветки в виртуальном доме что будет с этой веткой в браузерном доме
  - расскажи про фазу согласования
  - Что Такое JSX?
  - Что такое React Fiber?
  - Что такое строгий режим в React? Его преимущества?
  - Что такое синтетические события в React?
  - Что такое условный рендеринг (Conditional Rendering)? Как его выполнить?
  - Что такое компонент?
  - Разница между элементом и компонентом?
  - Зачем мы разбиваем код на компоненты?
  - Какие есть способы общения между компонентами?
  - В чем разница между управляемыми (controlled) и не управляемыми (uncontrolled) компонентами?
  - Какие методы жизненного цикла компонента существуют в React?
  - Стадии жизненного цикла компонента в React?
  - Что такое PureComponent?
  - Что такое Компонент высшего порядка (Higher-Order Component, HOC)?
  - Что такое компонент-переключатель (Switching Component)?
  - Разница между компонентом и контейнером?
  - в чём разница между пропсами и стейтом
  - Двустороннее и однонаправленное связывание данных?
  - Что такое поднятие состояния вверх (Lifting State Up)?
  - Как работает проп children?
  - Что такое порталы в React?
  - назови основные хуки в реакте
  - назови 3 правила написания хуков
  - почему нельзя использовать хуки в условных выражениях
  - Разница между useEffect() и componentDidMount()?
  - Как реализовать однократное выполнение операции при начальном рендеринге?
  - В чём разница между useEffect и useLayoutEffect?
  - Зачем в setState() нужно передавать функцию?
  - Зачем нам нужен менеджер состояния?
  - Как определить что состояние является глобальным?
  - Почему нельзя использовать контекст в качестве хранилища состояния?
  - Что такое серверный рендеринг (SSR)?
  - В чем заключаются недостатки SSR?
  - Какие есть альтернативы SSR?
  - Что такое двустороннее связывание?
  - Зачем нам нужен механизм двустороннего связывания?
  - Рассажи кратко как сделать бесконечный скролл
  - что такое virtual scroll
  - какой атрибут нужно дополнительно указывать и зачем, когда рендеришь список в реакте
  - какой единственный классовый компонент до сих активно используется
  - что такое Props drilling
  - в каких случаях использовать рефы
  - Что такое flushSync в Реакте
  - Что такое lazy loading?
  - Что такое инверсия наследования (Inheritance Inversion)?
  - Разница между useEffect() и componentDidMount()?
  - Для чего предназначен метод registerServiceWorker() в React?

## Web API
  - Что такое HTTP?
  - Как работает HTTP?
  - Структура HTTP запроса?
  - Какие методы может иметь HTTP-запрос?
  - В чем принципиальная разница между POST и GET?
  - Можем ли мы закешировать POST запрос?
  - Что такое коды ответа серверы и чем они отличаются друг от друга?
  - Чем отличается http от https?
  - Можем ли мы запустить http2 без https?
  - Почему повсеместно нужен https?
  - Что дает https помимо шифрования?
  - Можем ли мы получить картинку по HTTP?
  - Как мы можем подсказать браузеру подготовиться к загрузке ресурсов?
  - Влияет ли скорость ответа сервера на скорость загрузки сайта?
  - Как браузер понимает что ресурс нужно закешировать?
  - Зачем нужен хеш в названиях файлов?
  - Как браузер понимает что картинка является картинкой? 
  - Какими способами мы можем получить картинку с сервера?
  - Каким образом браузер понимает тип содержимого в ответе от API(картинка, текст, etc)?
  - Как браузер понимает что нужно загрузить картинку?
  - Как браузер понимает что нужно отображать именно картинку а не текст?
  - Что такое CORS?
  - Какие способы авторизации ты знаешь?
  - что будет если авторизацию сделать через GET
  - почему форму с паролем нельзя отправить GET запросом
  - Какой будет запрос для подтверждения регистрации пользователя?
  - Что такое JWT?
  - Что такое refresh токен?
  - Как защититься от парсинга?
  - почему картинки загружаются через GET, а не через POST
  - Отличия http2 от http1
  - Протоколы взаимодействия с беком
  - расскажи зачем заголовок Referrer
  - Что такое и чем опасен XSS?
  - Что такое CSRF?
  - что такое csrf токен
  - Как обезопасить себя от потенциально опасного клиентского ввода? 
  - Есть ли уязвимость связанная с _target =blank?
  - Что такое прогрессивная отрисовка?
  - Разница между Progressive Enhancement и Graceful Degradation?
  - Разница между feature detection, feature inference и анализом строки user-agent?
  - Что такое Веб-компоненты и какие технологии в них используются?
  - Способы уменьшения времени загрузки веб-страницы?
  - Что такое Progressive Web Application?
  - что такое сервис воркеры
  - Что такое Web Workers?
  - расскажи про repaint и reflow
  - расскажи про restyle и relayout
  - что такое Layout trashing
  - Что такое Flash Of Unstyled Content?
  - можно ли вставить счётчик в виде картинки
  - как сделать так, чтобы картинка, которая кэшируется обновлялась
  - какие есть способы хранения данных в браузере
  - в чём отличие localStorage от sessionStorage
  - Что такое IndexedDB в браузере?
  - Что мы можем делать с помощью devtools браузера?
  - Что такое HTTP cookie? Для чего они используются?
  - Разница между cookie, sessionStorage и localStorage?
  - Как защитить cookie?
  - Что такое WebSocket? В чем принцип его работы?
  - Что такое безопасные (Secure) и HttpOnly cookies?
  - Что такое Content Security Policy (CSP)?
  - Как работает JSONP?
  - Что такое History API в браузере?
  - Что такое BOM?
  - назвать способы оптимизации загрузки страниц сайта
  - рассказать об инструментах, которые можно использовать для анализа оптимизаций
  - Как мы можем оптимизировать отрисовку?
  - Что такое force layout и почему это плохо? 
  - Как работает hot reload?
  - Что такое Веб-компоненты и какие технологии в них используются?


## Git
  - Зачем нужна система контроля версий?
  - Что такое gitflow?
  - Что такое merge и rebase, в чем отличие друг от друга?
  - Как наши изменения попадают в ветку?
  - Как можно заставить git что-то забыть?
  - Как можно переименовать коммит?
  - В чем отличие amend от squash?
  - Что такое cherry-pick?
  - Что такое семантические коммиты?
  - Что ты знаешь про semantic version




вопросы https://github.com/likezninjaz/react-ru-interview-questions


задачи про промисы:
https://youtu.be/AY9Ta6cKcP0?t=4560

задачи про контекст:
https://habr.com/ru/company/ruvds/blog/422089/

https://habr.com/ru/post/578370/
https://github.com/likezninjaz/react-ru-interview-questions
