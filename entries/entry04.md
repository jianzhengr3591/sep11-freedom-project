# Entry 4
##### 03/14/2022
### content
 In the last blog [entry](entry03.md), I were coding up to the camera entity of the project, because I have already finished putting the shapes anmd geometric shapes together and have the image of what my thought is presented to me on the screen with the following codes. So after i crossed out those due dates on the google doc, I have now began the second part of my plan which is modtifiy and also make these shapes selectable or responsive in another way of saying this. But as I was researching and adding on now code funtions, I realized one big issue with my use of aframe, and the tough question that hit me internally is that " DO i want to make it more towards the gaming side of aframe or just the regular version of the selectable aframe use with ul being displaced on the screen." I did a lot of research and I will illustrate why i choose to stay away from the gaming style of aframe.
 
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
Here is the first adjustment I made after I cross off the frist time line, althought it look identical as the codes I had in [Previous](entry03.md), but is slightly different, and thqat little adjustment will make my life so much easier when i begin to put all my codes together. The reason why I choose to value and `id` to each shape is because i don't want my final product to be overwhelmed with many steps being repeated over and over again. However what my simplied Plan was to selected this entire section with the `id` of `shapes` and then use a `forEach()` loop to run throught each of the shapes.

```js
      document.querySelector("#shapes").addEventListener("click",function(event){
         if (event.target.value == "cylinder 1"){
          alert("hey")
         }
      })   

```

THese codes above is the idea I have came across when working throught it in class time after my second unit was taught. I thought that using the `addEventListener()` could possibly allow the our mouse to make a responsive respond. As stated in the line of code. `if` that statement is true, than  `alert()` the user on the page. But when i went to pre-view it, not only there's no erros in the console but there is also no erros in the `idecs50`. So i went back to the [Aframe](https://aframe.io/) home website and looked at why my shapes in the pre-view page is not responding like how I saw the examples on the home page will do. which caused me to be super confused, but i saw one of the examples in the Aframe webite and the title is " Aframe-galery", immediatluy to my head, I was like " oh yeah, JZ you better go in this glitch example see what important take ways you can get from this."  And these couple lines of codes caught my attentions.

```js
        <a-cursor
          id="cursor"
          animation__click="property: scale; startEvents: click; from: 0.1 0.1 0.1; to: 1 1 1; dur: 150"
          animation__fusing="property: fusing; startEvents: fusing; from: 1 1 1; to: 0.1 0.1 0.1; dur: 1500"
          event-set__mouseenter="_event: mouseenter; color: springgreen"
          event-set__mouseleave="_event: mouseleave; color: black"
          raycaster="objects: .link"></a-cursor>
```

This is that chunk of codes that caught all my attentions, and this is the main part of the project i needed foucs on the most. Aframe language is only slightly similair from what we been learning in class. Like `eventts`, `mouse`, these are the things we covered when we were learning the doms lesson, and not only that, in that glicth example it looks like the expect didn't even use the loops, all three images being displaced have an `id` and he just selected and used throught out the entire coding. whichg shock me, because at first i thought each shapes should have its own corresponding `evenListener()`. 
After looking at this, I was more aware and clear that, coding in Aframe is very different with javascript and the things we learning in class, with that in mind, i was looking more into the codes Aframe website provided and done some research on youtube as well.

Besides looking at the examples and throught the [glitch sources](https://glitch.com/~aframe-gallery), I also used Youtube, a great way to experience the codes more vitually and also have a better understanding of what is really going on. And here is some of the things I learned from it. And I was being introduced to this great system that's being applied in Aframe called `asset mangement sytem`, what this system does for us and the aframe program is that it makes it easier for the browser to cache assets (images, videos, models) and A-Frame will make sure all of the assets are fetched before rendering. So when we using the same entity more than  once we don't have to get it's `src`. 
* we can specify the enviornmnet of a entity using the `environment="preset: forest; dressingAmount: 500"`.
* `asset system`
* Add <a-assets> to the scene.
* Define the texture as an <img> under <a-assets>.
* Give the <img> an HTML ID (e.g., id="boxTexture").
* Reference the asset using the ID in DOM selector format (src="#boxTexture").
 
 After learning about all these within Aframe, the next step for me is to slowly apply to the area where is necessay so the program will function.
 
 ### 







[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
