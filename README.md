# 10.01. Зачем и что нужно мониторить

## 1 задание

загрузка ЦПУ и оперативной памяти, т.к. производятся вычисления;

мониторинг кодов http, т.к. сервис работает по этому протоколу;

количество клиентских соединений;

мониторинг скорости записи/чтения на диск и свободного места на нем, т.к. производится запись и вывод файлов.

## 2 задание

Если менеджер не понимает, на помощь придут метрики SLO/SLA/SLI. Обязанности перед клиентом надо изложить в SLA, на основании SLA выбрать SLO - метрики и границы, за которые они не должны выходить. SLI - это фактические метрики работы сервиса, они ответят на вопрос насколько мы выполняем свои обязанности перед клиентами и какое качество обслуживания.

## 3 задание

Можно настроить бесплатный ELK, для рассылки алертов использовать elasticalert.

## 4 задание

Не учтены 100-е и 300-е коды, они не являются ошибками, надо их добавить в формулу: (summ_1xx_requests+summ_2xx_requests+summ_3xx_requests)/summ_all_requests.
