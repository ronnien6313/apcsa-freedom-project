# Entry 2
##### 12/12/22



### Context

In APCSA, after deciding the tool and application I wanted to create, It was time for me to start tinkering with my tool. The first thing I wanted to do was to create a pop-up screen. The goal was to create an object that allowed a small panel to be opened when clicked. While doing this, I learned that there were many functions that was needed in order to make this work. The first function I learned was `onMouseDown()`. This allowed me to perform an action after the button is clicked. The second function I learned was `getComponent()` because I wanted to be able to alter the properties of the object. When combining these two functions, It allowed to me to create panel that could be opened and closed.

### Learning

#### onMouseDown() and getComponent<>()

The first thing I made using `onMouseDown()` and `getComponent()` was not a button and panel. I did something relatively simple, which was changing the color of an object. I first create a square object and attached a script to it, this script was named `colorChanger` which had the class `colorChanger`. In this class I created the method `onMouseDown()`. This is a built in method which requires a `collider` on the object to work. In order to have a `collider` on the object, I can manually go into the sqaures project and add a component called `2d Collider`. In this `onMouseDown()` method, it listens for a click from the user and then changes the color of the square to red. Here is the code I wrote:


The code I wrote also utilizes `getComponent<>()`. Without `getComponent()` I wouldn't have been able to change the properties of the square. What `getComponent<>()` does is whatever you put in to the `<>`, I am able to access the properties of it if I store it in a variable. By getting the `color` component of the square, I can set it to whatever I want.


#### Opening a Panel

Opening a panel was definitely much more complex compared to changing the color of a square. I first had to create both a `button` and a `panel`. The `button` already had a built-in `onClick` function, this meant that I didn't need `onMouseDown()` at all. After creating the button and panel, I set the panel to be turned off at first.

![image](https://user-images.githubusercontent.com/73479590/208309715-ccfc947b-a269-44af-83fd-a08fb70509a4.png)

The little box to the left of the word `Panel` is normally checked, but I turned it off so you can't see it in the beginning. My next step was to write the code to open the panel.

![image](https://user-images.githubusercontent.com/73479590/208310033-4b18728e-92c3-4793-a8bf-25453112d8fb.png)
![image](https://user-images.githubusercontent.com/73479590/208309997-68a86fa0-0a1c-4bf5-ad9e-384acc5f9eae.png)

What this code does it basically checks if there is a panel object and if there is, make the panel visible again.



### Engineering Design Process

I think I am at either EDP stage 2 or 3. I am trying to learn my tool, `Unity` so I can better understand the platform. Right now I only know how to code in Unity and create objects, But I haven't really started on creating the project yet. This leads to what I am planning to do next, which is actually starting the project. 


### Skills

The skills I learned was `How to Google` and `How to Learn`. This is because in order to learn `Unity`, I had to go to google and find out which tutorials or documentations could work for me. Some tutorials were kind of outdated and hard to follow, while others were more confusing than others. In the end, I mostly learned from the latest Unity Documentation and youtube videos that are recently uploaded, I say latest because some of their documentations are also outdated.




[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
