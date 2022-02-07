# Entry 3
##### 2/7/2022

### Content
Previously in [blog entry 2](entry02.md), I talked about what are some starting codes I begin to place into my coding session of this freedom project, which are like the legs of the building. The reasonw why I choose that as my first step is because I believe having a visual of what I will coding about is important. I don't want to come to an end and see a struture that I don't even like or the completly the opposite of what I predicted. 

```js
    <a-scene>
      <a-cylinder position="-1.52 0.75 -2.53" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-cylinder position="1.60 0.75 -2.53" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-cylinder position="1.60 0.75 -2.53" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-cylinder position="-1.52 -1.50 -2.53" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      <a-plane position="0 0 -4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
    </a-scene>
```
This is what I bascially put into my coding template, the reason why the opening and closing <a-scene> tag is outside of all my shapes is because is a scene of a struture, without the <a-scene> tag there won't be a displace bascially. After I wrote these codes then I went to preview it, but I hit an obsctales which is I can't rotate the screen around the struture, I was only able to see the front view of what I code in but not all around. So I went to the [A-frame](https://aframe.io/) website and went into the camera inside the compoent section. And this was one of the most helpful line of code I will need for my project. 
  ```js
  <a-entity camera look-controls position="0 1.6 0"></a-entity>
  ```

  This line of code is basically a camera that serve for us at a human eye level, which means that when we preview the struture we can see it at a comfort level and up at a werid angle where it will make us feel dizzy. This is what I am working on currently, but [A-frame](https://aframe.io/) is not the only resoures I get my code tools from. From github, Mr.mueller also provided me and the people who work on the same tool a website called [A-frame School](https://aframe.io/aframe-school/#/). This webiste is also pretty much like the regular A-frame webiste but is more like the key idea of the tool A-frame, so if there was a speiclfy code I need to know I have to go back to the mother page of it.
```js   
    1, document.createElement()
    
    2, .setAttribute()
    
    3, .appendChild()        
```
    
    
  Here are the three take away I got from the A-frame school website, and the reason why I think this will suit me perfectly is because this is javascript based, which means that all the 100 steps of repeating the same element but at a different positon, I can just simpily use Javascipt codes and make them into reusable codes. Which makes my life a whole lot easier, not only that this will also allow me to edit my codes a lot cleaier when I have a bug someone in these codes I wrote.
    
```js
    <a-entity camera look-controls position="0 1.6 0"></a-entity>
```
  
    
For example something like this, although I know this line of codes will create a camera view for me when I press preview, but I won't know how will it affect me if I were to rotate my view to the left of the house, will it still be at the same position or it will not even show up. That's why digging deep into these codes are important than just grabbing it and using it.
 
   What is next ? Next up I really hope I can finsih learning about the camera section of this building project using codes. Adding layers onto the based of my struture that's easy, I just have to figure out the position of where I want my shape to be placed at, like the x y z coordinate. My main aim for the next step is learn about the look-control, layers and visible in the A-frame website. Like I said before, my main goal of doing this project is because i am passiante about construtions and how things are being add on to build a safe house for myself, but on the process of building I can't just foucs on the front of it because what if the back of the house is unstable and god forbid a storm hit then the house will turned into a flat piece of land.
    
### EDP
    
    
    
    
    
### Skills
    
    
    
    
  
[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
