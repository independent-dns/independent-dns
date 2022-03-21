## Сетевая гигиена

### Все системы
- Установите Tor Browser и забудьте про слежку и цензуру: https://www.torproject.org/ru/download/. Правда, за это придётся заплатить снижением скорости и некоторой нестабильностью связи.
- Ещё один универсальный способ — установить приложение с сайта https://1.1.1.1/ (для владельцев телефонов с Android-ом может оказаться проще так: https://play.google.com/store/apps/details?id=com.cloudflare.onedotonedotonedotone). Это мир Cloudflare со всеми его достоинствами и недостатками.
- Если Вы не любите или не можете устанавливать программы, то существуют некоторые менее радикальные решения. Первое из них — использование независимых DNS-серверов; о нём и поговорим.

### Windows
1. Нажмите на клавиатуре одновременно клавиши `⊞Win` и `R`:

   ![1-alt-r](https://user-images.githubusercontent.com/102029879/159248644-be7b6b23-2ac5-4278-a846-c4f751197ffb.jpg)

2. В появившемся окошке наберите `ncpa.cpl` и нажмите `Enter`:

   ![2-ncpa-cpl](https://user-images.githubusercontent.com/102029879/159248647-00ed528a-cf96-4d32-9177-0233dfe369b6.png)

3. Теперь Ваша задача — найти в списке действующее сетевое подключение. Скорее всего, Вы его сами легко узнаете: оно не отмечено красным крестиком, и рядом нет слов *Unplugged*, *Disconnected*, *Отключено* и т.д.

   ![3-network-connections](https://user-images.githubusercontent.com/102029879/159248648-a9084036-ad4d-4799-8d24-0bc6e853bfbf.png)

   Но если не получится, смело можете проделать дальнейшие шаги со всеми подключениями.
4. На выбранном подключении щёлкните **правой** кнопкой мыши, а потом выберите пункт *Properties*, или *Свойства*:

   ![4-properties](https://user-images.githubusercontent.com/102029879/159248654-8e28efdb-020b-4e4d-b58a-879575d2e636.png)

5. В интернет мы почти все заходим по протоколу TCP/IPv4. Этот пункт Вам и нужен, выбирайте его и щёлкайте на *Properties*/*Свойства*:

   ![5-tcp-ipv4](https://user-images.githubusercontent.com/102029879/159248655-7dac9279-8d9d-450f-abf8-1b0cbaaba98c.png)

6. Вот Вы и добрались до того места, где начинается свобода — по крайней мере, от примитивной DNS-блокировки. По умолчанию Ваш компьютер использует адресацию от Вашего интернет-провайдера, который, увы, подконтролен местным спецслужбам. Чтобы не зависеть от чужих прихотей хотя бы в этом, настройте адреса DNS-серверов вручную:

   ![6-dns](https://user-images.githubusercontent.com/102029879/159248657-54bb5116-e59e-440f-ad0c-be3ca8962712.png)

   Тут можете выбрать два любых на свой вкус:
   
   `1.1.1.1` — это сервер уже упоминавшейся Cloudflare;
   
   `8.8.8.8` — сервер Google;
   
   `77.88.8.8` — сервер Яндекса, если угодно: уж там-то никакой Russia Today не заблокируют!
   
   Если что, есть и куча других.

### Ссылки
У Вас другая версия Windows и Вы запутались в настройках? Здесь всё расскажут лучше и подробнее: https://www.comss.ru/page.php?id=754

Не хватает грамотно изложенных технических деталей? Вам сюда: https://habr.com/ru/post/352654/
