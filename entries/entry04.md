# Entry 4
##### 3/20/23

### Context

After creating the bulk button we wanted to implement the `next day` button. When this button is clicked, we want to make a fade out animation which transitions the game to the next day. The current day will be displayed on the top right of the screen.

### Coding

The first thing I did was create a `next day` button. I first imported the pixel art of the button I made and then created a `button`. The `nextday` button is extremely important since this button will change all the stats of the user. Here is how the button looks :

![image](https://user-images.githubusercontent.com/73479590/226502392-bd16874d-843f-4476-bed4-0ea0ac492f77.png)

I then created a new script called `transitionThing` that will act as the function for the button. The goal of the button is to make it so when it's clicked, a text displaying the current day will increase by 1. Here is the code for it:

![image](https://user-images.githubusercontent.com/73479590/226502428-d3ce59b7-8e56-4ae4-b5ef-b335d3c502f2.png)

![image](https://user-images.githubusercontent.com/73479590/226502444-bd539959-0446-45b4-8be4-aebb23047fc9.png)

I first made two variables, One to hold the text while the other will be the counter for the days. In the second image, since the game starts on day 1, we set the counter to 1. we then set `dayNum` to `"Day " + counter`. This will basically display `Day #` in the game, # denoting the current day number. The `buttonClick()` function then makes it so when the `next day` button is pressed, the counter increases by 1 and the dayNum text is updated to the current day.

The next thing I did was display the stats in the journal page. This part was pretty easy as all I had to do was create accessor methods and display them. I first created multiple accessor methods which got all the stats of the user. Here is the code for that:

![image](https://user-images.githubusercontent.com/73479590/226502317-b4553641-0452-414f-9d8a-790912c970ea.png)

I then went into the journal script and set `statText` to whatever format I wanted the stats to be displayed as.

![image](https://user-images.githubusercontent.com/73479590/226502337-f7189c62-ee20-412e-b086-bd2df1d578e5.png)





### Engineering Design Process
I am currently at EDP stage 5 where I am creating the prototype. Me and my group are currently working on the core functions of the game. We already have planned what we want to add to the game and split up who will do what. In order to move on to the next stage we have to finish a few more functions of the game. My goal by the next week is to create a mood system which will affect the users stats.

### Skills

The skills that I have learned while coding this part are `debugging` and `problem decomposition`. While coding, there were many errors in the code whether it'd be mines or my partners. We would message each other about how to solve these errors and try to break the code down into smaller pieces so we could find out what was the problem. We eventually did solve all the errors but I'm sure that there will be more errors to come.





[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)


