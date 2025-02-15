# Components and Services of tr_script

## 1. **Components**

### 1.1 **UI**:
  - `Switch`: Switch(aka toggle) button
  - `Button`: custom ```tsx <button/>``` component
  - `View`: mobile page wrapper component
  - `Typography`: text html tags replacement (`<h1/>`,`<h2/>` etc.)
  - `Input`: custom `<input/>` component
    
### 1.2 **Widgets**:
  - `TokenTracker` - list of all public tokens, consists of:
    - `Filters`: appliable filters for the list
    - `Item`: item of each public token
  - `NotificationHistory` - list of notifications, consists of:
    - `Item`: item of each notification
  - `CardLink` - link to a several different pages, apparently looks like card
  - `TokenModal` - modal window, which shows information for every accessible token in a `TokenTracker`, consists of:
    - `Field`: a field of some information for a token(not a `<fieldset/>` component though)

## 2. Services
  - `GetToken`: takes all the data for all the components, that stores on the server (for a )
  - `SetFavoriteToken`: sets a token into a favorite list (?)
  - `ClearFavoriteToken`: deletes a token from a favorite list (?)
  - `NofifyNewToken`: sets a condition for user to take notifications for a new token
  - `GetNotification`: takes data for a new notifications, considering price change of a tokens (?)
  - `ClearNotification`: deletes all items from a notification list (?)
  
