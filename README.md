# Components and Services of tr_script

## 1. **Components**

### 1.1 **UI**:
  - `Switch`: Switch(или toggle) кнопка
  - `Button`: кастомный ```tsx <button/>``` компонент
  - `View`: врапер для страницы
  - `Typography`: кастомный компонент, заменяющий текстовые теги  (`<h1/>`,`<h2/>` и т.д.)
  - `Input`: кастомный `<input/>` компонент
    
### 1.2 **Widgets**:
  - `TokenTracker` - список всех доступных токенов, состоит из:
    - `Filters`: фильтры для списка токенов 
    - `Item`: итем каждого из доступных токенов 
  - `NotificationHistory` - список уведомлений, состоит из
    - `Item`: итем уведомления, приходящих юзеру
  - `CardLink` - линк на различные страницы приложения, выглядит как карточка
  - `TokenModal` - модальное окно, которое показывает информацию по каждому достпуному токену в `TokenTracker`, состоит из:
    - `Field`: поле, отображающее определенный поинт(цена, ликвидность и т.д.) по токену
  - `BlackListToken` - черный список токенов, состоит из:
    - `Item` - итем, показывающий каждый токен, добавленный в черный список

## 2. Services
  - `GetToken`: получает все данные по токенам, которая хранится на сервере(для дальнейшего парсинга данных в `TokenTracker` итемы)
  - `SetFavoriteToken`: ставит флаг, для сохранения выбранного токена в список избранных (?)
  - `ClearFavoriteToken`: удаляет флаг и соответственно выбранный токен из списка избранного (?)
  - `NofifyNewToken`: ставит флаг, для рассылки уведомлений о появлении нового токена
  - `GetNotification`: ставит флаг, для получения уведомлений по изменениям статуса различных токенов(цена и т.п.) (?)
  - `ClearNotification`: чистит список уведомлений (?)
  
