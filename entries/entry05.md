# Entry 5
##### 4/23/23


### Context

After creating the button `transitionThing`, we made it so every function of the game relies on that button. The moment it is clicked, all the user's stats will change depending on various factors of the game. One factor that I had to make was a function called `mood`. This `mood` function will randomly give the player a mood every week which will affect the user's stats.

### Coding

The first thing I did was make it so the `mood` was viewable in the journal. This was done by going into the `journal` script and simply appending the mood text at the end.

![image](https://user-images.githubusercontent.com/73479590/233855163-d200dcd9-39df-4afb-a419-f0b9b3ce57b7.png)

This is what it looked like.

![image](https://user-images.githubusercontent.com/73479590/233855129-f9ee6f49-9e3b-4e35-a583-716e54e43117.png)


The first thing I did was go into the `initStat` script to add `mood` variable. This allows us to get the `mood` of the player.

![image](https://user-images.githubusercontent.com/73479590/233855181-bfa9cf00-a5df-433e-99b3-9bb3b37abfdb.png)


I then created a `moodChanger` script that will run everytime the `next week` button is pressed. I first created the variables I needed. A `string mood` variable to hold the current mood, a `player` variable so I can change the stats of the player, and an `array` of `moods` so I can randomize the moods each week.

The constructor `moodChanger` will first randomly select a mood from the array with a random number generator and then set the `string mood` to whatever the mood chose was. We then created a `changeMood()` method to actually change the stats of the `player`. In this method, we make it so if the `string mood` is equal to any of the words listed, it will change the `players` stats depending on its determination. Before changing the determination, I made it so the determination can not go beyond `100` or go under `0`. This is because determination should be a stat out of `100` that will decide whether or not the player will do it's exercises. 

![image](https://user-images.githubusercontent.com/73479590/233855226-782e4709-4655-4040-b271-cce38127019e.png)

After all this, I just run the code every time the `next week` button is pressed:

![image](https://user-images.githubusercontent.com/73479590/233855210-533808f7-b579-4aea-aa73-7b2b91c29b54.png)

### Engineering Design Process

Right now, We have finished our MVP (Minimal Viable Product) which leaves us at EDP stage 6 or 7. We are currently making sure that everything in the game works and functions as intended. We then plan to add more functions in the game and fix/improve the code to make it more efficient.

### Skills

The skills I learned from this process are communication and creativity. I felt like communication was a big part of this process because we had to make sure everyone was doing the work they needed to do. This is because the MVP was due soon and we needed to fix all the mistakes in the code. I also learned creativity because I had to figure out what to add to the game and how I was going to implement it.





[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)


