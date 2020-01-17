# Xnor.ai acquisition by Apple

## Interesting news of the day

Apple have reportedly acquired [xnor.ai] (https://xnor.ai) for $200M

Xnor are well known for having advocated the use of binary neural networks rather than low-precision floating point, int8 or other numerical formats.

The advantage of (Binary Neural Networks) BNNs is that the chip area and propagation delays for circuits implementing BNNs are much less costly in dynamic and leakage power than NN accelerators using other formats.  

The reason for this is down to Boolean algebra

The cost of a Binary multiplication is one AND gate

| A | B |A.B|
| - | - | - |
| 0 | 0 | 0 |
| 0 | 1 | 0 |
| 1 | 0 | 0 |
| 1 | 1 | 1 |

Also the memory required to store a binary weight/coefficient for a BNN multiplier is one bit

And the wiring required to transmit the weight from a register or memory to the multiplier is one bit wide

In a nanometer world where wiring is now the most costly element of a System on Chip (SoC) this is a big deal

## Why this is a big deal

Binary networks are not a new idea and in some ways are almost as old as computing itself

Alan Turing proposed the use evolution to “train” a particular type of neural network he called a “B-type unorganised machine” in 1948 

The challenge until now has that while BNNs are very attractive from a power/area/cost/frequency perspective this big challenge was the degradation in network accuracy

As we all know network accuracy is key to being able to deploy a product or service based upon it as 50% accuracy means you might as well flip a coin as pay heed to the output of your deep network

The jury has been out on whether it is possible to trade off an increase in the complexity of BNN networks against higher accuracy

By that I mean recover the accuracy lost in simply quantising all the weights to 1-bit by making much wider and potentially much deeper networks

This has been the focus of a lot of academic effort and a few startups over the past 3-4 years

Clearly this must have yielded fruit for Apple to have paid $200M

## Why

I decided to try this after reading [Jeremy Howard's blog post]  (https://www.fast.ai/2020/01/16/fast_template/)

[My blog is now accessible on] (https://moloned.github.io/cto_maverick/)

The only issue not codered in Jeremy's blog entry was that you need to set the Github Pages section of the settings menu for your blog repo to Master otherwise the blog isn't accessible and you get a 404 error

## How

For those (like me) who are new to markdown here's a useful [cheatsheet] (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) I found it while Googling how to format a table in markdown
