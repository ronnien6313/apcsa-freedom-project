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
        bulkOn.SetActive(true);
        bulkOff.SetActive(false);
        InitStat.determination = (int)(InitStat.determination * 1.1);
    }
    // Turn bulk off
    public void buttonClick(){
        bulkOff.SetActive(true);
        bulkOn.SetActive(false);
        InitStat.determination = (int)(InitStat.determination * 0.9);
    }
    
    
```



Text

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
