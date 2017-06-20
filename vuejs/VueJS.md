## Installation
 To add VueJS I can insert **"<script src = "https://unpkg.com/vue"></script>"** into html file.
 
## Basic Application
 ```javascript
 new Vue({
  el: '#app',
  data:{
      title: 'Title Message'
    }
 });
 ```
 * "new Vue()" creates new Vue object, use it always you need vue generated data
 * "el:" is an reserved property, shows which part Vue takes under control
 * "data:{}" is an reserved property.
 ***
v-on:<name_of_event>="<method_name>" is a directive; instruction/command which will be recognised by vue. It says: Listen to an event

Put <methods:{}> after **<data:{}>** to list all the used methods.
***
Instead of **~data.title~** use **this.title**. This is because VueJS is making it accesable from the Vue object.


## Templates
{{}} - Interpolation
The process: Raw HTML -> Vue Object -> Real HTML
{{ functionName() }} - must return a string

**NO CURLY BRACES INSIDE ANY HTML ATTRIBUTE**: <a href="{{ link }}">Link</a> - **is invalid**
			Instead use: <a v-bind:href="link">Link</a> - that will work
			
Directive - instruction

## Directives
 * v-on   - takes event and updates when the event is happening
 * v-bind - bind an **attribute** to vue
 * v-once - content won't be overwritten and will stick to the initial value
 * v-html - renders HTML code, won't escape. (Be careful, csrf is an issue)