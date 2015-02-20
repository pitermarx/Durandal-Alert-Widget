### _Durandal + Bootstrap alert widget_

_Assuming there is a durandal project with bootstrap loaded..._

#### Example
Add a widget to the html
```html
<div data-bind="alert: {id:'alert1'}"></div>
```
Include the alert widget in the config
```js
app.configurePlugins({
    widget: {
        kinds: ['alert']
    }
});
```
Use the durandal's app events
```js
app.trigger('alert1:info', "All good!");
app.trigger('alert1:danger', "Not all good!");
```
