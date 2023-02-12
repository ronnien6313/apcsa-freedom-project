# Entry 3
##### 2/12/23


### Context 

After learning a bit about Unity, we decided that it was time to start on our project. My partner Wei Jie created the GitHub repository for the game and created the foundation for the game already. As such, I was tasked with creating the `bulk` option for the game. The button is supposed to increase or decrease your `determination` depending if you want to bulk or not. `Determination` is a stat that will affect whether or not you will skip or do your exercises. 

### Coding

In order to create the `bulk` option, I had to add two buttons to my canvas. One button will indicate `bulk` is on, while the other will indicate it being off. I then designed how the buttons will look will pixel art so I can better differentiate which button should do what. Here is how it looks:

![image](https://user-images.githubusercontent.com/73479590/218335339-9d110e0d-5e17-4207-9edb-11c855c64798.png)
![image](https://user-images.githubusercontent.com/73479590/218335348-d0a8f2cc-8f41-43f7-8524-58cde2852f40.png)

* Green indicates `bulk` being on
* Red indicates `bulk` being off

I then had to write the code to make the button interactable. Here is how I planned for the button to work: When the `bulk` button is in its red state, you want to make it so that when you click it, it lowers the determination of the user. When you `bulk` you want to do fewer exercises so you can gain more weight and lowering the `determination` increases the chance of skipping exercises. As such, on the other hand, when the button is green, you want to make it so that when it's clicked, you increase the `determination`. Here is how the code looks:

```C#
    // Variables both scripts had
        public GameObject bulkOn;

        public GameObject bulkOff

    // Turn bulk on
        public void buttonClick (){
        bulkOn.SetActive(true); // line 1
        bulkOff.SetActive(false); // line 2
        InitStat.determination = (int)(InitStat.determination * 0.9); // line 3
    }
    // Turn bulk off
    public void buttonClick(){
        bulkOff.SetActive(true); // line 4
        bulkOn.SetActive(false); // line 5
        InitStat.determination = (int)(InitStat.determination * 1.1); // line 6
    }
 
```

In order to use the variables that were written in our script, we had to attach the buttons we made onto the script through the `inspector`.

![image](https://user-images.githubusercontent.com/73479590/218335926-ceacf75f-7222-4151-9a74-9d38eaa267d9.png)

Writing the script wasn't that difficult. When the button is clicked in the red state, lines 1 to 3 run. `.SetActive()` basically either hides or reveals the object by using a boolean (`true` reveals it while `false` hides it). We set the `bulkOn` button to `true` because we are turning it on, while we set the `bulkOff` button to false when the user doesn't want to bulk. We then increase the determination since the user wants to do less exercises when bulking. This is then done in the reverse when turning bulk off (lines 4 to 6).

### Engineering Design Process

I think that I am currently in EDP stage 3 or 4. I and my group are both planning and creating the game right now. While creating the game, we still are incorporating new ideas and see how we can create certain game mechanics. In order to move on to the next stage, we would need to first complete the prototype of the game. We believe that this will come after more weeks of work as we just started creating the game recently.


### Skills

The skills I learned while creating the `bulk` button were `time management` and `how to read`. I managed my time better because I was slacking a bit before doing this part of the project because of the workload I had from other classes. However, now that I have kind of sorted out how my work was distributed throughout my day, I definitely got more work done effectively. The next skill I learned was `how to read`. I didn't really watch youtube videos and tutorials but instead looked through documentation on how I can import images and how to utilize buttons fully.




[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)


