# Entry 3
##### 2/12/23


### Context 

After learning a bit about Unity, we decided that it was time to start on our project. My partner Wei Jie created the github repository for the game and created the foundation for the game already. As such, I was tasked with creating the `bulk` option for the game. The button is supposed to increase or decrease your `determination` depending if you want to bulk or not. `Determination` is a stat that will affect whether or not you will skip or do your exercises. 

### Coding

In order to create the `bulk` option, I had to add two buttons onto my canvas. One button will indicate `bulk` being on, while the other will it being off. I then designed how the buttons will look will pixel art so I can better differentiate which button should do what. Here is how it looks:

![image](https://user-images.githubusercontent.com/73479590/218335339-9d110e0d-5e17-4207-9edb-11c855c64798.png)
![image](https://user-images.githubusercontent.com/73479590/218335348-d0a8f2cc-8f41-43f7-8524-58cde2852f40.png)

* Green indicates `bulk` being on
* Red indicates `bulk` being off

I then had to write the code to make the button interactable. Here is how I planned for the button to work: When the `bulk` button is in its red state, you want to make it so when you click it, it lowers the determination of the user. When you `bulk` you want to do less exercises so you can gain more weight and lowering the `determination` increases the chance of skipping exercises. As such, on the other hand when the button is green, you want to make it so when it's clicked, you increase the `determination`. Here is how the code looks:

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

In order to use the variables that was written in our script, we had to attach the buttons we made onto the script through the `inspector`.

![image](https://user-images.githubusercontent.com/73479590/218335926-ceacf75f-7222-4151-9a74-9d38eaa267d9.png)

Writing the script wasn't that difficult. When the button is clicked in the red state, lines 1 to 3 run. `.SetActive()` basically either hides or reveal the object by using a boolean (`true` reveals it while `false` hides it). We set the `bulkOn` button to `true` because we are turning it on, while we set the `bulkOff` button to false. We then increase the determination since the user wants to do less exercises when bulking. This is then done in the reverse when turing bulk off (lines 4 to 6).





Text

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
