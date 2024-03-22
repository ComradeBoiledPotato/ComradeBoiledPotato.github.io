## Analog chips in machine learning: a simple introduction.


Hello there! In this post I will talk about what analog chips are and how they can be used with machine learning. 
This is an simple introduction to the concept, and should at most be used to introduce someone to the topic or as an inspiration for a hobby project.

    **Analog versus Digital**

In order to understand what analog chips are and why they could be prefferred over digital chips in ML, we first need to get a basic understanding of digital chips. 
Digital computer chips are basically a ton of logic gates that channel electricty in such a way that you can perfectly controll your output with the input. 
Digital chips are not dependant of the electrical signal itself: If there's any amount of electricity it represents a **1** and if there's no electricty it represents a **0**. 
Obviously, we would like to compute numbers bigger than this, so we came up with the binary counting system. Based on which logic gate is giving a **1** or **0**, we can represent a bigger number.
So for example (read right to left) **00000011** is three and **00001011** is eleven. This allows us to compute precisely up to very high numbers.

Analog chips do not work with 1's and 0's. Instead, the electrical signal itself represents a number. So for example a current of 36mA = 36. 
Because of this, we do not need to wire up logic gates in a very complex way so that we get our desired result. Instead, all the calculations can be represented physically. 
Adding two numbers together becomes adding two wires together: I + I = 30mA + 30mA = 30 + 30 = 60. 
And in order to do some more complex calculations like multiplication, we just have to take a look at some physics formula's: U = I*R = 200mA * 20Ohm = 200 * 20 = 4000. 
Here our inputs are the current and resistance (which you can control with an variable resistor) and our output is the voltage we measure.

    **Why is digital used more than analog?**

Even though analog chips consume a lot less electricty, these days mostly digital chips are used. That is because digital chips are 
very precise, because they work with absolute values like 1's and 0's. Analog chips work with the electrical signal itself, which is
never exactly the same and can de influenced by the smallest of factors like the resistance of the wires. Because of this, analog chips
are only used in for example very precise voltage meters. 

    **Why analog chips could be preferred over their digital counterparts in ML**

When running a neural network, a digital chips needs to peform a lot of multiplications, each of which requiring thousands of bits,
and on top of that it also needs to keep fetching the locations of the data of a cell in the neural network (like weight, bias, etc.)
so that it can peform the calculation. This is very energy intensive and is the reason why you hear all sorts of horror stories of AI's like
ChatGPT using 2L of water to cool down the computers it runs on everytime you send it a prompt. This is a problem that analog chips could solve.
A Neural Network can be physically represented by using normal wires as the connections between neurons and the neurons themselves being
variable resistors set to specific values. By controlling the electrical signal going into this analog chip, we control the inputs of the AI.
And by measuring the electrical signal at the end we can determine the AI action. In training mode, we can adjust the neural network
by adjusting the values on our variable resistors. In the end the AI would end up using a lot less power and would be a lot faster.


*I hope that this has explained the basics of analog chips and how they can be used with ML.*





