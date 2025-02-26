## Исследование  пользователей сервиса GoFast сервис аренды самокатов)
## Описание данных. 

**Пользователи — users_go.csv**
+ user_id - уникальный идентификатор пользователя
+ name - 	имя пользователя
+ age -	возраст
+ city -	город
+ subscription_type -	тип подписки (free, ultra)
**Поездки — rides_go.csv**
+ user_id	- уникальный идентификатор пользователя
+ distance -	расстояние, которое пользователь проехал в текущей сессии (в метрах)
+ duration -	продолжительность сессии (в минутах) — время с того момента, как пользователь нажал кнопку «Начать поездку» до момента, как он нажал кнопку «Завершить поездку»
+ date -	дата совершения поездки
**Подписки — subscriptions_go.csv**
+ subscription_type -	тип подписки
+ minute_price -	стоимость одной минуты поездки по данной подписке
+ start_ride_price -	стоимость начала поездки
+ subscription_fee -	стоимость ежемесячного платежа
Чтобы совершать поездки по городу, пользователи сервиса GoFast пользуются мобильным приложением. Сервисом можно пользоваться:
1. без подписки
+ абонентская плата отсутствует;
+ стоимость одной минуты поездки — 8 рублей;
+ стоимость старта (начала поездки) — 50 рублей;
2. с подпиской Ultra
+ абонентская плата — 199 рублей в месяц;
+ стоимость одной минуты поездки — 6 рублей;
+ стоимость старта — бесплатно.
**Цель иследования:**
    
   1. Определить вырочку с подпиской и без подписки; 
   2. Проверить: тратять ли пользователи с подпиской больше, чем пользователи без подниски;
   3. Среднее расстояние, которое проезжают пользователи с подпиской за одну поездку, не превышает 3130 метров;
   4. Помесячная выручка от пользователей с подпиской по месяцам выше, чем выручка от пользователей без подписки.

  **Ход иследования:**
Данные о поездах, пользователях и подписках я получу из файлов : `users_go.csv`, `rides_go.csv`, `subscriptions_go.csv`. 
О качестве данных ничего не известно. Перед тем как приступить к анализу данных, следует предобработать датасеты, а именно проверить на пропуски, дубликаты, неверные значения и другое.
