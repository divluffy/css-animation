# hi





### The animation property is a shorthand property for:

- animation-name
- animation-duration
- animation-timing-function
- animation-delay
- animation-iteration-count
- animation-direction
- animation-fill-mode
- animation-play-state

#### whats mean this property?


animation-name	Specifies the name of the keyframe you want to bind to the selector
animation-duration	Specifies how many seconds or milliseconds an animation takes to complete
animation-timing-function	Specifies the speed curve of the animation
animation-delay	Specifies a delay before the animation will start
animation-iteration-count	Specifies how many times an animation should be played
animation-direction	Specifies whether or not the animation should play in reverse on alternate cycles
animation-fill-mode	Specifies what values are applied by the animation outside the time it is executing
animation-play-state	Specifies whether the animation is running or paused

#### then we can write this in one line, how?
 
animation: name duration timing-function delay iteration-count direction fill-mode;

Example: 
animation: nameAnimation 0.5s ease-in-out;


#### And when we use animation then we use keyframes with it
#### what keyframes?

The @keyframes controls the intermediate steps in a CSS animation sequence by defining styles for keyframes (or waypoints) along the animation sequence. This gives more control over the intermediate steps of the animation sequence than transitions.

Example: 
If use from and to.
```
@keyframes nameAnimation {
  from {
    transform: translateX(0%);
  }

  to {
    transform: translateX(100%);
  }
}
```

If you use percentages from 0% to 100%
```
@keyframes nameAnimation {
  0% { top: 0; }
  50% { top: 30px; left: 20px; }
  50% { top: 10px; }
  100% { top: 0; }
}
```

Specify when the style change will happen in percent, or with the keywords "from" and "to", which is the same as 0% and 100%. 0% is the beginning of the animation, 100% is when the animation is complete.

#### Also we can use from and to with percentage like

```
@keyframes myexample {
  from {top: 0px;}
  50%  {top: 100px !important;} /* ignored */
  to   {top: 200px;}
}
```

>> The !important rule is ignored in a keyframe
> The !important rule is ignored in a keyframe




