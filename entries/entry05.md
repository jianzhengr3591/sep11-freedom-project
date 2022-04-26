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
### How I work and tackle my problems towards the finish line !
This is the idea that had in mind, I was hoping that when I run this line of code I will be able to see myself walking upfront in the canvas or the aframe scene. When i went to preview the codes, there was nothing popping up, not only that it completely crashed my codes. One what I was trying to select did not work at all because Aframe and some of JS codes don't really match together. Secondly, `upArrow` was not defined because I did not use the `key()` so whenever I click on the keyboard, although the computer realize there is a click but it didn't know what key was pressed.

I begin to question myself, " why did the example provided in the [Aframe](https://aframe.io/) wedsite did not use any `eventlistener()` to move there camera move when they wanted to see other stuff or objects in the Aframe scene. When I look into the codes from the example I did not see any `Eventlistener()` but just a scene and then one line of link that will back up or already have the code function ready for us. So I went on our helpful friend `[YOUTUBE](../README.md)`, I was shoock by the thinsg I didscovered. Maybe is because that I never search up the right topic or I am confused on what I need to insert into my code.

The one thing that caught most of my attention is where I saw this title `beginner tutorial` , the light pole in my head immeditely went up because that beginner is me.  Something I learn and take away from the video is that, in JS we can customize our background of a scene, but in Aframe we can have an environment in our scene, and all these environment is already made as a function in the back end all we have to do is to call it out and make it pop up. 
```js
    <a-scene id = "shapes" environment="preset:forest">
    
As we can see, in order if want a certain environment all we need to add is to call the `environment` and set it equal to the environment that you want your building environment to be in.
```

This is just one of the most exciting thing I found, the coolest thing that I discover is that, you don't acutally need to import any `camera()` entity all you got to do is insert the aframe backend tool set, and that link will insert a " Aframe tool belt" into your program.
```
 <script src="https://unpkg.com/aframe-environment-component@1.3.1/dist/aframe-environment-component.min.js"></script>
 
This one single line of code with the `Src` is what how we get the full control and abloe to aviod the complex route of writting every line of code letter by letter.
```

Lastly I had to close out my roof top, and the main compoent I used for this part of my project is the `rotation=""`. The rotation component defines the orientation of an entity in degrees. It takes the pitch (x), yaw (y), and roll (z) as three space-delimited numbers indicating degrees of rotation. And for now I just want a simple roof top since is MVP, but when I have time which is beyoung MVP I can customize a theme roof or something more fancy.
```js
    <a-box position= "-1 5 -4"  rotation= "0 0 45"color="#20B2AA" depth="8" height="0.1" width="7"></a-box>
   
    <a-box position= "1 5 -4"  rotation= "0 0 -45"color="#20B2AA" depth="8" height="0.1" width="7"></a-box>
    
  I just simpliy did a box and change the depth, height and width and then rotate it 45 degrees so it will form a triangle top
```

### Engineering process

I am proud to say this is a great journy for me to both learn and experience from. I am currently in stage 6 and 8 which is Test and evaluate the prototype also Communicate the results. I have reached a point where I have inputted all the informations I need to achieve my MVP, with that being said I am now testing out the codes and the functionality of my program and see where are the areas that I can improve and delvelope upon during my beyoung MYP. And also with the outcome of testing and taking notes on the areas I can improve on then I can let myself learn and educate myself on the glows and thr grows of this porject. Which can help me to aviod the same obsctales the next time I encouter the same type of project.


### Skills

The two main skills I will be foucsing on as of where I am at right now are embracing failure and also consideration. Since I am basically at the end of my project, I just now need to understand the mistake and digest them to better understand why those mistakes occurs and also what other ways I could've done to aviod this mistake. Also to consider how my next trail of working on this kind of project will be like, Use the things i analzed after a whole school year and learn from my own mistakes. Sometimes is better to learn off your own mistakes then teaching it brand new by others because yourself have already experienced.



[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
