# Jquery
1. To get a CDN that you can incoorporate in your project go to: https://developers.google.com/speed/libraries#jquery.There you will copy the 3.x snippet - the latest version of jQuery.
2. To add the CDN in your project, just simply add the the <script></script> you just copied, just above/before the javascript file you have created.
3. So how to use jQuery:
    3.1: $() == jQuery() == document.querySelector();
         $() works for document.querySelector() and querySelectorAll();
    3.2: addClass() build in method for jQuery 
         addClass() == classList.add();
         same thing goes for removeClass() == classList.remove();
         same thing goes for checking if an element has somekind of class: hasClass() == classList();
    3.3: text = innerHTML;
         so for example:
          before: document.querySelector().innerHTML=something == $().text();
    3.4: html is a better version of text so html >= text;
         it's so because with html we can add opening and closing tags with changing our text. So for example: $().html(<em>something</em>) and so on.
    3.5: attr(source attribute, 'source') : is a method to set up source for example src , href... . attr work for classes as well.
    3.6: click(function) and keydown(function) : add Event listener. Even when we have classes with the same name, thanks to jQuery, click and keydown will search for all the classes with the same name. So there is no need for for loops.
    3.7: on(event, function) is a better method to search for event. Of course we need to specify the event in the first input of the metod.
    3.8: before() is a method that can create a new html element BEFORE the specified element. So for example, if we wanted to create a new element before something we write: $(h1).before(<button></button>) and this will create a button before our specified h1 in this case.
         same goes for after(), but this time it will create the element, AFTER the specified element
         There is also prepend() and append(), where prepend() will add a new element just write after the opening tag of the element we created, and append() will create the element just before the closing tag of the element we specified.
         remove() will remove ALL the specified element.
   3.9: hide() will hide an element. show() will show the element. It's important to understand that these methods are constand, meaning that once hide() and show() are executed it will stay like that. We can use hide() and show() to simulate an animation or simply use: toggle() which works like hide() and show() in the same time. Usually these methods are within functions after we specifed an even that occur.
        fadeOut() is a more animatic hide() and same goes for fadeIn() for show() and fadeToggle.
        There are also slideOut(), slideIn(), slideToggle().
  3.10: animate() is a more free way to stylies our animation, but not that free: We can't change color for example. Only numeric value can be changed, like opacity, margin, etc.
4. All methods in 3. can be used in one call of $().
