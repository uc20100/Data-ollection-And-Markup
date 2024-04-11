# ДЗ по "Сбор и разметка данных (семинары)"

## Семинар 1. Основы клиент-серверного взаимодействия. Парсинг API
* Домашнее задание:
1.	Ознакомиться с некоторые интересными API. 
https://docs.ozon.ru/api/seller/ https://developers.google.com/youtube/v3/getting-started https://spoonacular.com/food-api
2.	Потренируйтесь делать запросы к API. Выберите публичный API, который вас интересует, и потренируйтесь делать 
API-запросы с помощью Postman. Поэкспериментируйте с различными типами запросов и попробуйте получить различные 
типы данных.
3.	Сценарий Foursquare
4.	Напишите сценарий на языке Python, который предложит пользователю ввести интересующую его категорию (например, 
кофейни, музеи, парки и т.д.).
5.	Используйте API Foursquare для поиска заведений в указанной категории.
6.	Получите название заведения, его адрес и рейтинг для каждого из них.
7.	Скрипт должен вывести название и адрес и рейтинг каждого заведения в консоль.

## Семинар 2. Парсинг HTML. BeautifulSoup
* Домашнее задание:  
Выполнить скрейпинг данных в веб-сайта http://books.toscrape.com/ и извлечь информацию о всех книгах на сайте во 
всех категориях: название, цену, количество товара в наличии (In stock (19 available)) в формате integer, описание.
Затем сохранить эту информацию в JSON-файле

## Семинар 3. Системы управления базами данных MongoDB и Кликхаус в Python
* Домашнее задание:
1.	Установите MongoDB на локальной машине, а также зарегистрируйтесь в онлайн-сервисе. https://www.mongodb.com/ https://www.mongodb.com/products/compass
2.	Загрузите данные который вы получили на предыдущем уроке путем скрейпинга сайта с помощью Buautiful Soup в MongoDB и создайте базу данных и коллекции для их хранения.
3.	Поэкспериментируйте с различными методами запросов.
4.	Зарегистрируйтесь в ClickHouse.
5.	Загрузите данные в ClickHouse и создайте таблицу для их хранения.

## Семинар 4. Парсинг HTML. XPathПарсинг HTML. XPath
* Домашнее задание:  
- Выберите веб-сайт с табличными данными, который вас интересует.
Напишите код Python, использующий библиотеку requests для отправки HTTP GET-запроса на сайт и получения 
HTML-содержимого страницы.
Выполните парсинг содержимого HTML с помощью библиотеки lxml, чтобы извлечь данные из таблицы.
Сохраните извлеченные данные в CSV-файл с помощью модуля csv.  

- Ваш код должен включать следующее:  
Строку агента пользователя в заголовке HTTP-запроса, чтобы имитировать веб-браузер и избежать блокировки сервером.
Выражения XPath для выбора элементов данных таблицы и извлечения их содержимого.
Обработка ошибок для случаев, когда данные не имеют ожидаемого формата.
Комментарии для объяснения цели и логики кода.  
  
- Примечание: Пожалуйста, не забывайте соблюдать этические и юридические нормы при веб-скреппинге.

## Семинар 5. Scrapy
* Домашнее задание:  
1.	Найдите сайт, содержащий интересующий вас список или каталог. Это может быть список книг, фильмов, спортивных 
команд или что-то еще, что вас заинтересовало.
2.	Создайте новый проект Scrapy и определите нового паука. С помощью атрибута start_urls укажите URL выбранной вами 
веб-страницы.
3.	Определите метод парсинга для извлечения интересующих вас данных. Используйте селекторы XPath или CSS для навигации 
по HTML и извлечения данных. Возможно, потребуется извлечь данные с нескольких страниц или перейти по ссылкам на 
другие страницы.
4.	Сохраните извлеченные данные в структурированном формате. Вы можете использовать оператор yield для возврата 
данных из паука, которые Scrapy может записать в файл в выбранном вами формате (например, JSON или CSV).
5.	Конечным результатом работы должен быть код Scrapy Spider, а также пример выходных данных. Не забывайте соблюдать 
правила robots.txt и условия обслуживания веб-сайта, а также ответственно подходите к использованию веб-скрейпинга.

## Семинар 6. Scrapy. Парсинг фото и файлов
* Домашнее задание: 
1.	Создайте новый проект Scrapy. Дайте ему подходящее имя и убедитесь, что ваше окружение правильно настроено для 
работы с проектом.
2.	Создайте нового паука, способного перемещаться по сайту www.unsplash.com. Ваш паук должен уметь перемещаться 
по категориям фотографий и получать доступ к страницам отдельных фотографий.
3.	Определите элемент (Item) в Scrapy, который будет представлять изображение. Ваш элемент должен включать такие 
детали, как URL изображения, название изображения и категорию, к которой оно принадлежит.
4.	Используйте Scrapy ImagesPipeline для загрузки изображений. Обязательно установите параметр IMAGES_STORE в файле 
settings.py. Убедитесь, что ваш паук правильно выдает элементы изображений, которые может обработать ImagesPipeline.
5.	Сохраните дополнительные сведения об изображениях (название, категория) в CSV-файле. Каждая строка должна 
соответствовать одному изображению и содержать URL изображения, локальный путь к файлу (после загрузки), 
название и категорию.

## Семинар 7. Selenium в Python
* Домашнее задание: 
1.	Выберите веб-сайт, который содержит информацию, представляющую интерес для извлечения данных. Это может быть 
новостной сайт, платформа для электронной коммерции или любой другой сайт, который позволяет осуществлять скрейпинг 
(убедитесь в соблюдении условий обслуживания сайта).
2.	Используя Selenium, напишите сценарий для автоматизации процесса перехода на нужную страницу сайта.
3.	Определите элементы HTML, содержащие информацию, которую вы хотите извлечь (например, заголовки статей, названия 
продуктов, цены и т.д.).
4.	Используйте BeautifulSoup для парсинга содержимого HTML и извлечения нужной информации из идентифицированных элементов.
5.	Обработайте любые ошибки или исключения, которые могут возникнуть в процессе скрейпинга.
6.	Протестируйте свой скрипт на различных сценариях, чтобы убедиться, что он точно извлекает нужные данные.
7.	Предоставьте ваш Python-скрипт вместе с кратким отчетом (не более 1 страницы), который включает следующее: 
URL сайта. Укажите URL сайта, который вы выбрали для анализа. Описание. Предоставьте краткое описание информации, 
которую вы хотели извлечь из сайта. Подход. Объясните подход, который вы использовали для навигации по сайту, 
определения соответствующих элементов и извлечения нужных данных. Трудности. Опишите все проблемы и препятствия, с 
которыми вы столкнулись в ходе реализации проекта, и как вы их преодолели. Результаты. Включите образец извлеченных 
данных в выбранном вами структурированном формате (например, CSV или JSON).  
*Примечание: Обязательно соблюдайте условия 
обслуживания сайта и избегайте чрезмерного скрейпинга, который может нарушить нормальную работу сайта.*

## Семинар 8. Работа с данными
* Домашнее задание:  
- Скачайте датасет House Prices Kaggle со страницы конкурса ([ссылка на Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data)) и сохраните его в том же каталоге, что и ваш скрипт или блокнот Python.  
- Загрузите датасет в pandas DataFrame под названием df.  
- Выполните предварительную обработку данных, выполнив следующие шаги: 
   - Определите и обработайте отсутствующие значения в датасете. Определите, в каких столбцах есть отсутствующие значения, и решите, как их обработать (например, заполнить средним, медианой или модой, или отбросить столбцы/строки с существенными отсутствующими значениями). 
   - Проверьте и обработайте любые дублирующиеся строки в датасете. 
   - Проанализируйте типы данных в каждом столбце и при необходимости преобразуйте их (например, из объектных в числовые типы).  
- Проведите разведочный анализ данных (EDA), ответив на следующие вопросы: 
  - Каково распределение целевой переменной 'SalePrice'? Есть ли какие-либо выбросы?   
  - Исследуйте взаимосвязи между целевой переменной и другими характеристиками. Есть ли сильные корреляции? 
  - Исследуйте распределение и взаимосвязи других важных характеристик, таких как 'OverallQual', 'GrLivArea', 'GarageCars' и т.д. 
  - Визуализируйте данные, используя соответствующие графики (например, гистограммы, диаграммы рассеяния, квадратные диаграммы), чтобы получить представление о датасете.
- Выполните проектирование признаков путем реализации следующих преобразований: 
  - Работайте с категориальными переменными, применяя one-hot encoding или label encoding, в зависимости от характера переменной. 
  - При необходимости создайте новые характеристики, такие как общая площадь или возраст объекта недвижимости, путем объединения существующих характеристик.
- Сохраните очищенный и преобразованный набор данных в новый CSV-файл под названием 'cleaned_house_prices.csv'

## Семинар 9. Инструменты разметки наборов данных
* Домашнее задание:  

- Задача 1.
Выберите датасет, который имеет отношение к вашей области интересов или исследований. Датасет должен содержать неструктурированные данные, требующие разметки для решения конкретной задачи, например, анализа настроений или распознавания именованных сущностей.

- Задача 2.
Выполните разметку на основе правил (rule-based labeling) на подмножестве выбранного датасета. Разработайте и реализуйте набор правил или условий, которые позволят автоматически присваивать метки данным на основе определенных шаблонов или критериев.

- Задача 3.
Выполните разметку вручную отдельного подмножества выбранного датасета с помощью выбранного вами инструмента разметки.

- Задача 4.
Объедините данные, размеченные вручную, с данными, размеченными на основе правил. Объедините два подмножества размеченных данных в один набор данных, сохранив при этом соответствующую структуру и целостность.

- Задача 5.
Обучите модель машинного обучения, используя объединенный набор размеченных данных. Разделите датасет на обучающий и тестовый наборы и используйте обучающий набор для обучения модели.

- Задача 6.
Оценить эффективность обученной модели на тестовом датасете. Используйте подходящие метрики оценки. Интерпретируйте результаты и проанализируйте эффективность модели в решении задачи разметки.



