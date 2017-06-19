## Installation:
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
