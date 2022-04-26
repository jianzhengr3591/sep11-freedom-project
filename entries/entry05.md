# Entry 5
##### 4/25/22

### Content
Previously, I tried to add eventlistener() so whenever I pressed a key the computer was able to run those lines of codes and move the camera() entity up and walk like a human being viewing a house. The reason why I chose to go through that complex route is because I couldn't find anything that or what we call the backend program. This was the hardest part of Aframe because everything else you can pretty much do using some simple highschool math and geometry.
```js
    document.querySelector("#scene").addEventListener("click",function(event){
         if (event.target.value == "upArrow"){
          cameraFront += 5
         }
      })  
```
### How I work and tackle my problems towards the finish line !
This is the idea that I had in mind, I was hoping that when I run this line of code I will be able to see myself walking upfront in the canvas or the aframe scene. When i went to preview the codes, there was nothing popping up, not only that it completely crashed my codes. One thing I was trying to select did not work at all because Aframe and some of the JS codes don't really match together. Secondly, upArrow was not defined because I did not use the key() so whenever I click on the keyboard, although the computer realizes there is a click but it doesn't know what key was pressed.
I begin to question myself, " why did the example provided in the Aframe website not use any eventlistener() to move their camera when they wanted to see other stuff or objects in the Aframe scene. When I look into the code from the example I did not see any Eventlistener() but just a scene and then one line of link that will backup or already have the code function ready for us. So I went on our helpful friend [YOUTUBE](../README.md), I was shocked by the things I discovered. Maybe is because that I never search up the right topic or I am confused on what I need to insert into my code.
The one thing that caught most of my attention is when I saw this title beginner tutorial , the light pole in my head immediately went up because that beginner is me. Something I learn and take away from the video is that, in JS we can customize our background of a scene, but in Aframe we can have an environment in our scene, and all these environment is already made as a function in the back end all we have to do is to call it out and make it pop up.
```js
   <a-scene id = "shapes" environment="preset:forest">
```    
As we can see, in order if you want a certain environment all we need to add is to call the `environment` and set it equal to the environment that you want your building environment to be in.
This is just one of the most exciting thing I found, the coolest thing that I discover is that, you don't actually need to import any camera() entity all you got to do is insert the Aframe backend tool set, and that link will insert a " Aframe tool belt" into your program.
```js
<script src="https://unpkg.com/aframe-environment-component@1.3.1/dist/aframe-environment-component.min.js"></script>

This one single line of code with the `Src` is how we get full control and are able to avoid the complex route of writing every line of code letter by letter.
```
 
Lastly I had to close out my rooftop, and the main component I used for this part of my project is the rotation="". The rotation component defines the orientation of an entity in degrees. It takes the pitch (x), yaw (y), and roll (z) as three space-delimited numbers indicating degrees of rotation. And for now I just want a simple roof top since it is MVP, but when I have time which is beyoung MVP I can customize a theme roof or something more fancy.
```js
   <a-box position= "-1 5 -4"  rotation= "0 0 45"color="#20B2AA" depth="8" height="0.1" width="7"></a-box>
    <a-box position= "1 5 -4"  rotation= "0 0 -45"color="#20B2AA" depth="8" height="0.1" width="7"></a-box>
    
  I just simply did a box and change the depth, height and width and then rotate it 45 degrees so it will form a triangle top
```
### Engineering process
I am proud to say this is a great journey for me to both learn and experience from. I am currently in stage 6 and 8 which is Test and evaluate the prototype also Communicate the results. I have reached a point where I have inputted all the informations I need to achieve my MVP, with that being said I am now testing out the codes and the functionality of my program and see where are the areas that I can improve and develop upon during my beyoung MYP. And also with the outcome of testing and taking notes on the areas I can improve on then I can let myself learn and educate myself on the glows and the growth of this project. Which can help me to avoid the same obstacles the next time I encounter the same type of project.
### Skills
The two main skills I will be focusing on as of where I am at right now are embracing failure and also consideration. Since I am basically at the end of my project, I just now need to understand the mistakes and digest them to better understand why those mistakes occur and also what other ways I could've done to avoid this mistake. Also to consider how my next trail of working on this kind of project will be like, Use the things I analyzed after a whole school year and learn from my own mistakes. Sometimes is better to learn off your own mistakes then teaching it brand new by others because yourself have already experienced.



[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
