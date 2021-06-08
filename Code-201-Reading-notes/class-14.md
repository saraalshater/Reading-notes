
# New research reveals surprising truths about why some work groups thrive and others falter.



- software engineers are encouraged to work together, in part because studies show that groups tend to innovate faster, see mistakes more quickly and find better solutions to problems. Studies also show that people working in teams tend to achieve better results and report higher job satisfaction. In a 2015 study, executives said that profitability increases when workers are persuaded to collaborate more. Within companies and conglomerates, as well as in government agencies and schools, teams are now the fundamental unit of organization. If a company wants to outstrip its competitors, it needs to influence not only how people work but also how they work together.


- The researchers eventually concluded that what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. The right norms, in other words, could raise a group’s collective intelligence, whereas the wrong norms could hobble a team, even if, individually, all the members were exceptionally bright.


- As the researchers studied the groups, however, they noticed two behaviors that all the good teams generally shared. First, on the good teams, members spoke in roughly the same proportion, a phenomenon the researchers referred to as ‘‘equality in distribution of conversational turn-taking.’’ On some teams, everyone spoke during each task; on others, leadership shifted among teammates from assignment to assignment. But in each case, by the end of the day, everyone had spoken roughly the same amount. ‘‘As long as everyone got a chance to talk, the team did well,’’ Woolley said. ‘‘But if only one person or a small group spoke all the time, the collective intelligence declined.’’


- the good teams all had high ‘‘average social sensitivity’’ — a fancy way of saying they were skilled at intuiting how others felt based on their tone of voice, their expressions and other nonverbal cues. One of the easiest ways to gauge social sensitivity is to show someone photos of people’s eyes and ask him or her to describe what the people are thinking or feeling — an exam known as the Reading the Mind in the Eyes test. People on the more successful teams in Woolley’s experiment scored above average on the Reading the Mind in the Eyes test. They seemed to know when someone was feeling upset or left out. People on the ineffective teams, in contrast, scored below average. They seemed, as a group, to have less sensitivity toward their colleagues.



- researchers sometimes colloquially refer to traits like **‘‘conversational turn-taking’’** and **‘‘average social sensitivity’’** as aspects of what’s known as **psychological safety** — a group culture that the Harvard Business School professor Amy Edmondson defines as a **‘‘shared belief held by members of a team that the team is safe for interpersonal risk-taking.’’** **Psychological safety is ‘‘a sense of confidence that the team will not embarrass, reject or punish someone for speaking up,’’** Edmondson wrote in a study published in 1999. **‘‘It describes a team climate characterized by interpersonal trust and mutual respect in which people are comfortable being themselves.’’**


`‘We had lots of data, but there was nothing showing that a mix of specific personality types or skills or backgrounds made any difference. The ‘‘who’’ part of the equation didn’t seem to matter.’`


<br>
<br>

# [Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.


## Transform Syntax

```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```



## 2D Transforms

- Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.


- Three-dimensional transforms work on both the x and y axes, as well as the z axis.*** These three-dimensional transforms help define not only the length and width of an element, but also the depth.*** 


## 2D Rotate 

The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a **positive** value will rotate an element **clockwise**, and using a **negative** value will rotate the element **counterclockwise**. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.


## 2D Scale

scale allows you to change the appeared size of an element.

The default scale value is 1, **therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.**


The `scaleX` value will scale the width of an element while the `scaleY `value will scale the height of an element. 


## 2D Translate

The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.


## Perspective

The perspective of an element can be set in two different ways. One way includes using the perspective value within the transform property on individual elements, while the other includes using the perspective property on the parent element residing over child elements being transformed.


<br>
<br>

# [Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)


# Transitions
for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including **transition-property, transition-duration, transition-timing-function, and transition-delay**. Not all of these are required to build a transition, with the first three are the most popular.



## Transitional Property
The `transition-property` property determines exactly what properties will be altered in conjunction with the other transitional properties.
By default, all of the properties within an element’s different states will be altered upon change. However, only the properties identified within the `transition-property` value will be affected by any transitions.



If multiple properties need to be transitioned they may be **comma separated** within the transition-property value. Additionally, the keyword value all may be used to transition all properties of an element.


-  **not all properties may be transitioned**, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another.

## Transition Duration
The duration in which a transition takes place is set using the `transition-duration` property. The value of this property can be set using general timing values, **including seconds (s) and milliseconds (ms)**. These timing values may also come in fractional measurements, .2s for example.

- When transitioning multiple properties you can set multiple durations, one for each property. As with the transition-property property value, multiple durations can be declared using comma separated values. The order of these values when identifying individual properties and durations does matter. For example, the first property identified within the transition-property property will match up with the first time identified within the transition-duration property, and so forth.


<br>


# Animations


## Animations Keyframes

To set **multiple** points at which an element should undergo a transition, use the @keyframes rule. The `@keyframes` rule includes the animation name, any animation breakpoints, and the properties intended to be animated.


```
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```
<br>
<br>

# [8 SIMPLE CSS3 TRANSITIONS THAT WILL WOW YOUR USERS](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

<br>
<br>

# [Button animated](https://codepen.io/retyui/pen/ByoaXV)

<br>
<br>

# [CSS3 Animations: Keyframes](https://codepen.io/akshaychauhan/pen/oAfae)

<br>
<br>

# [404](https://codepen.io/kieranfivestars/pen/MYdQxX)


<br>
<br>

# [Pure CSS Bounce Animation](https://codepen.io/dp_lewis/pen/gCfBv)



[link to my reading]()