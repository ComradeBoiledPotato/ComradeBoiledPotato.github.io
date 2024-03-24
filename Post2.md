## The neuronchip: how to teach neurons to play video games.

**In this article, I will discuss how I designed a chip that's able to train live neurons to play pong.**


One time I had a German customer that asked me if I could come up with a chip that could train neurons to play pong. 
I thought he was joking, but he was dead serious. So I told him I'd think about his offer and get back to him later. 
In the meantime I did some research and it turned out that training neurons to use computers had already be done before and in theory 
it wasn't too hard. My customer had only asked me if I could design the chip, so the diffuclt part of assembeling it was left to him. 
I reached out to the customer, told him I'd do it and then we started discussing the price.

After we'd agreed on the terms I got to work and first tried to think about how I was actually gonna pull this off. 
I eventually decided to treat at first as if I was designing an analog chip, except instead of resistors and capacitors the neurons were 
this time actual neurons. The problem with live neurons is that you can't arrange them into a neat network and you sort of have to hope that
they will form a proper network themselves eventually. But before spending too much time trying to solve that problem, I first had to design
a chip that the neurons could be put into without them dying. 
The first thing that we needed to solve were the electrical connections: copper or tin would easily poison the neurons, so I only made the 
outer electrical connections out of copper, and the connections to which the neurons would be connected would be made out of gold, because 
gold is a good enough conducter and is biocompatible so the neurons can grow onto them without getting poisend. 
Now that the electrical connections won't kill the neurons, we still need a medium for them to live in.
I looked online and consulted a few local microbiologists, and eventually settled on a recipe that basically contained a bunch of glucose, 
some proteins to help with neural connections and some antibodies to kill any pathogens. 
You'd just need to add that recipe to distilled water and you'd have a medium for the neurons to live in.

Now that we more or less have our chip, how do we train our neurons? Because we were dealing with living things, we couldn't implement any 
fancy training methods. So I went for the simplest training method that'd work with neurons: reinforcement learning. 
It turns out that neurons preffer organised, predictable electrical signals over choatic ones. So if we want to punish our neurons, we'd 
transmit some electrical noise to them, and if we wanted to reward them we just transmit a steady signal.

But we still have one problem: when we add the neurons to our chip and they start growing and moving around, 
they're just making connections with each other at random. This can start to be problematic if it causes the density of neurons to increase
a lot, because a high denisty of neurons means a lot of unnecesary connections that can mess with the output. 
We can try to control this by adding our neurons gradually in a "spread-out" way (not too spread out because that'll result in too few connections)
and transmit choatic electrical signals to regions with bad density. 
These measures won't immediatley result in a good density, but will defenitly help.

So now I only had to program a simple script that would communicate with the neuron chip 
(which only involves sending input and listening for output) and I was done! I send the design to the customer, and they send the payment.

*I hope that this article has suceeded with introducing you to the world of neuronchips.*






