## Analog chips in machine learning: a simple introduction.


Hello there! In this post I will talk about what analog chips are and how they can be used with machine learning. This is an simple introduction to the concept, and should at most be used to introduce someone to the topic or as an inspiration for a hobby project.

    **Analog versus Digital**
In order to understand what analog chips are and why they could be prefferred over digital chips in ML, we first need to get a basic understanding of digital chips. Digital computer chips are basically a ton of logic gates that channel electricty in such a way that you can perfectly controll your output with the input. Digital chips are not dependant of the electrical signal itself: If there's any amount of electricity it represents a **1** and if there's not electricty it represents a **0**. Obviously, we would like to compute numbers bigger than this, so we came up with the binary counting system. Based on which logic gate is giving a **1** or **0**, we can represent a bigger number. So for example (read right to left) **00000011** is three and **00001011** is eleven. This allows us to compute precisly up to very high numbers.

Analog chips do not work with 1's and 0's. Instead, the electrical signal itself represents a number. So for example a current of 36mA = 36. Because of this, we do not need to wire up logic gates in a very complex way so that we get our desired result. Instead, all the calculations can be represented physically. Adding two number together becoms adding two wires together: I + I = 30mA + 30mA = 30 + 30 = 60. And in order to do some more complex calculations like multiplication, we just have to take a look at some physics formula's: U = I*R = 200mA * 20Ohm = 200 * 20 = 4000. Here our inputs are the current and resistance (which you can control with an variable resistor) and our output is the voltage we measure.

    **Why is digital used more than analog?**






