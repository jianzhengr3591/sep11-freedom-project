# Entry 4
##### 03/14/2022
### Content
 In the last blog [entry](entry03.md), I was coding up to the camera entity of the project, because I have already finished putting the shapes and geometric shapes together and have the image of what my thought is presented to me on the screen with the following codes. So after I crossed out those due dates on the google doc, I have now begun the second part of my plan which is modified and also makes these shapes selectable or responsive in another way of saying this. But as I was researching and adding on now code functions, I realized one big issue with my use of a-frame, and the tough question that hit me internally is that " DO i want to make it more towards the gaming side of a-frame or just the regular version of the selectable a-frame use with ul being displaced on the screen." I did a lot of research and I will illustrate why I choose to stay away from the gaming style of a-frame.
 
 ```js
          HTML 
    <a-scene id = "shapes">
      <a-cylinder position="-1.82 0.75 -2.2" radius="0.1" height="1.5" color="#FFC65D" value = "cylinder1"></a-cylinder>
      <a-cylinder position="1.60 0.75 -2.2" radius="0.1" height="1.5" color="#FFC65D" value = "cylinder2"></a-cylinder>
      <a-cylinder position="1.60 0.75 -5.8" radius="0.1" height="1.5" color="#FFC65D" value = "cylinder3"></a-cylinder>
      <a-cylinder position="-1.82 0.75 -5.8" radius="0.1" height="1.5" color="#FFC65D" value = "cylinder4"></a-cylinder>
      <a-cylinder position="0.3 2 -2" color="black" radius="0.1" value = "cylinder5"></a-cylinder>
      <a-cone position="-0.10 2 -3" color="tomato" radius-bottom="2" radius-top="0" value = "cone1"></a-cone>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4" value = "plane1"></a-plane>
    </a-scene>        
        
 ```
Here is the first adjustment I made after I crossed off the first timeline, although it looks identical to the codes I had in [Previous](entry03.md), but is slightly different, and that little adjustment will make my life so much easier when I begin to put all my codes together. The reason why I choose to add `value` to each shape is because I don't want my final product to be overwhelmed with many steps being repeated over and over again. However, what my simplified Plan was to select this entire section with the `id` of `shapes` and then use a `forEach()` loop to run through each of the shapes.

```js
      document.querySelector("#shapes").addEventListener("click",function(event){
         if (event.target.value == "cylinder 1"){
          alert("hey")
         }
      })   

```

The code above is the idea I have come across when working through it in class time after my second unit was taught. I thought that using the `addEventListener()` could possibly allow the our mouse to make a responsive respond. As stated in the line of code. `if` that statement is true, than  `alert()` the user on the page. But when I went to preview it, not only were there no errors in the console but there were also no errors in the `idecs50`. So i went back to the [Aframe](https://aframe.io/) home website and looked at why my shapes in the preview page is not responding like how I saw the examples on the homepage will do. which caused me to be super confused, but i saw one of the examples in the Aframe website and the title is " Aframe-gallery", immediately to my head, I was like " oh yeah, JZ you better go in this glitch example see what important takeaways you can get from this."  And these couple lines of codes caught my attentions.

```js
        <a-cursor
          id="cursor"
          animation__click="property: scale; startEvents: click; from: 0.1 0.1 0.1; to: 1 1 1; dur: 150"
          animation__fusing="property: fusing; startEvents: fusing; from: 1 1 1; to: 0.1 0.1 0.1; dur: 1500"
          event-set__mouseenter="_event: mouseenter; color: springgreen"
          event-set__mouseleave="_event: mouseleave; color: black"
          raycaster="objects: .link"></a-cursor>
```

This is that chunk of code that caught all my attention, and this is the main part of the project I needed to focus on the most. The A-frame language is only slightly similar from what we've been learning in class. Like `events`, `mouse`, these are the things we covered when we were learning the doms lesson, and not only that, in that glitch example it looks like the expect didn't even use the loops, all three images being displaced have an `id` and he just selected and used throughout the entire coding. which shock me, because at first i thought each shapes should have its own corresponding `evenListener()`. 
After looking at this, I was more aware and clear that coding in A Frame is very different from javascript and the things we are learning in class. With that in mind, I was looking more into the codes A-frame website provided and did some research on youtube as well.

Besides looking at the examples and through the [glitch sources](https://glitch.com/~aframe-gallery), I also used [Youtube](https://www.youtube.com/watch?v=cS8uGfd_oG8), a great way to experience the codes more visually and also have a better understanding of what is really going on. And here are some of the things I learned from it. And I was being introduced to this great system that's being applied in A-frame called `asset management system`, what this system does for us and the aframe program is that it makes it easier for the browser to cache assets (images, videos, models) and A-Frame will make sure all of the assets are fetched before rendering. So when we using the same entity more than  once we don't have to get it's `src`. 
* we can specify the environment of a entity using the `environment="preset: forest; dressingAmount: 500"`.
* `asset system`
* Add <a-assets> to the scene.
* Define the texture as an <img> under <a-assets>.
* Give the <img> an HTML ID (e.g., id="boxTexture").
* Reference the asset using the ID in DOM selector format (src="#boxTexture").
 
 After learning about all these within Aframe, the next step for me is to slowly apply to the area where it is necessary so the program will function.
 
 ### Engineering process
 As of right now, I am still on the "Brainstorm possible solutions" step of the engineering process, because as presented before, this Aframe language is huge. If you ever want to learn everything, let me guarantee you, you will need more than just a school year to do that. As I research about the different questions in the Aframe home site, more codes are being presented to me and I have been gathering useful information I found into my unit notes, so once in awhile I will test them out to see which ones are suitable and which are the ones i can take off the notes. And this is the reason why I am still brainstorming the possible solution, because every monday i find new stuff and new ideas come in mind as i work on it, so i can't just focus on one method of drawing my "dream house" using Aframe. On top of that I am also somewhat on the "communicate the result" , although i am working by myself, but i always ask myself that, if I apply something i learned from the a frame home site, would it affect my codes, or would it have the same outcome as what I hope it will come out as, just constantly asking these kinds of question will allow me to make sure each step of my project was being done the right way.
 
 ### Skills
The skill I used for this section of my freedom project is mainly " How to research" and being "organized". This part of the freedom project I did not focus a lot on the physical coding  part but more on the research. I realized that I have a lot of questions about the things I am working on when I placed the shapes into the plane. And also that sometimes when i research about a topic, i am not being specific enough which will not show me what i needed. NOt only that because i was doing a lot of researching, my notes were a little unorganized. So every once in a while, I will look at my freedom project notes and put them in the order that will guide me through the coding part. 





[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
