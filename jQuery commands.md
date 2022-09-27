# Jquery
1. To get a CDN that you can incoorporate in your project go to: https://developers.google.com/speed/libraries#jquery.There you will copy the 3.x snippet - the latest version of jQuery.<br/>
2. To add the CDN in your project, just simply add the the <script></script> you just copied, just above/before the javascript file you have created.<br/>
3. So how to use jQuery:<br/>
    3.1: $() == jQuery() == document.querySelector();<br/>
         $() works for document.querySelector() and querySelectorAll();<br/>
    3.2: addClass() build in method for jQuery <br/>
         addClass() == classList.add();<br/>
         same thing goes for removeClass() == classList.remove();<br/>
         same thing goes for checking if an element has somekind of class: hasClass() == classList();<br/>
    3.3: text = innerHTML;<br/>
         so for example:<br/>
          before: document.querySelector().innerHTML=something == $().text();<br/>
    3.4: html is a better version of text so html >= text;<br/>
         it's so because with html we can add opening and closing tags with changing our text. So for example: $().html(<em>something</em>) and so on.
    3.5: attr(source attribute, 'source') : is a method to set up source for example src , href... . attr work for classes as well.<br/>
    3.6: click(function) and keydown(function) : add Event listener. Even when we have classes with the same name, thanks to jQuery, click and keydown will search for all the classes with the same name. So there is no need for for loops.<br/>
    3.7: on(event, function) is a better method to search for event. Of course we need to specify the event in the first input of the metod.<br/>
    3.8: before() is a method that can create a new html element BEFORE the specified element. So for example, if we wanted to create a new element before something we write: $(h1).before(<button></button>) and this will create a button before our specified h1 in this case.<br/>
         same goes for after(), but this time it will create the element, AFTER the specified element<br/>
         There is also prepend() and append(), where prepend() will add a new element just write after the opening tag of the element we created, and append() will create the element just before the closing tag of the element we specified.<br/>
         remove() will remove ALL the specified element.<br/>
   3.9: hide() will hide an element. show() will show the element. It's important to understand that these methods are constand, meaning that once hide() and show() are executed it will stay like that. We can use hide() and show() to simulate an animation or simply use: toggle() which works like hide() and show() in the same time. Usually these methods are within functions after we specifed an even that occur.<br/>
        fadeOut() is a more animatic hide() and same goes for fadeIn() for show() and fadeToggle.<br/>
        There are also slideOut(), slideIn(), slideToggle().<br/>
  3.10: animate() is a more free way to stylies our animation, but not that free: We can't change color for example. Only numeric value can be changed, like opacity, margin, etc.<br/>
4. All methods in 3. can be used in one call of $().
