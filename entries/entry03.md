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

  This line of code is basically a camera that serve for us at a human eye level, which means that when we preview the struture we can see it at a comfort level and up at a werid angle where it will make us feel dizzy.
  
  
[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
