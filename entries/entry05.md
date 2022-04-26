# Entry 5
##### 4/25/22

### Content 

Previously, I tried to add `evenlistener()` so whenever I press a key the computer is able to run those line of codes and move the `camera()` entity  move up and walk like a huamn being viewing a house. The reason why I choose to go throught that complex route is because I couldn't find anything that or what we call the call the backend program. This was the hardest part aframe because everything else you can pretty much do it using some simple highschool math and geometry. 
```js
     document.querySelector("#scene").addEventListener("click",function(event){
         if (event.target.value == "upArrow"){
          cameraFront += 5
         }
      })   
```
This is the idea that had in mind, I was hoping that when I run this line of code I will be able to see myself walking upfront in the canvas or the aframe scene. When i went to preview the codes, there was nothing popping up, not only that it completely crashed my codes. One what I was trying to select did not work at all because Aframe and some of JS codes don't really match together. Secondly, `upArrow` was not defined because I did not use the `key()` so whenever I click on the keyboard, although the computer realize there is a click but it didn't know what key was pressed.

I begin to question myself, " why did the example provided in the [Afrmae](https://aframe.io/) wedsite did not use any `eventlistener()` to move there camera move when they wanted to see other stuff or objects in the Aframe scene. When I look into the codes from the example I did not see any `Eventlistener()` but just a scene and then one line of link that will back up or already have the code function ready for us. So I went on our helpful friend `YOUTUBE`, I was shoock by the thinsg I didscovered. Maybe is because that I never search up the right topic or I am confused on what I need to insert into my code.


[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
