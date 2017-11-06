# S-R Latch

## About

**A bistable device having two states *Set* & *Reset* and therefore, is known as *Set-Reset*, or *S-R* Latch.**                                                                                                                                                                                       
----------------------------------

### Sequential Circuits

Unlike Combinational Logic circuits that change state depending upon the actual signals being applied to their inputs at that time, Sequential Logic circuits have some form of inherent “Memory” built in.

![](http://www.electronics-tutorials.ws/wp-content/uploads/2013/08/seq4.gif)

The word “**Sequential**” means that things happen in a “**sequence**”, one after another and in Sequential Logic circuits, the actual clock signal determines when things will happen next. Simple sequential logic circuits can be constructed from standard Bistable circuits such as: *Flip-flops, Latches and Counters* and which themselves can be made by simply connecting together universal **NAND Gates** and/or **NOR Gates** in a particular combinational way to produce the required sequential circuit.

----------------------------------

### S-R Latch

#### Procedure
We can wire two NOR gates in such a way that the output of one feeds back to the input of another, and vice versa, like this:

![](https://www.electrical4u.com/images/february16/1458318341.gif)

By definition condition of Q=1 and not-Q=0 is **set** and Q=0 and not-Q=1 is **reset**.

**In the above logic circuit if S = 0 and R = 1, Q becomes 1. Let's explain how.**

* NAND gate always gives output 1 when at least one of the inputs is 0.
  So, when S is applied as 0 the output of gate G1 i.e. Q is 1 irrespective of the condition of second input  to the gate.

 
* Now, Q is input of gate G2 so both the inputs of G2 become 1 as R is already 1. So output of G2 is now  or 0.
  So whatever may be the previous condition of Q, it always becomes Q = 1 and  = 0 when S = 0 and R = 1. This is called SET     condition of the latch.


**In the above logic circuit if S = 1 and R = 0, Q becomes 0. Let's explain how.**

* As we already said, a NAND gate always gives output 1 when at least one of the inputs is 0.
* So when R is applied as 0, the output of gate G2 i.e.  is 1 irrespective of the condition of second input Q to the gate.
* So whatever may be the previous condition of , it always becomes 1 this 1 is then fed back to input of gate G1. As here S     is already 1, both inputs of G1 are 1. Hence output of G1 i.e. Q will be 0. So Q = 0 and  = 1 when, S = 1 and R = 0. This     is called RESET condition of the latch.


**In the above logic circuit if S = 1 and also R = 1, Q remains same as it was. Let's explain how.**

* First suppose Q is previously 1.
* Now both inputs of G2 are 1 as R = 1 and Q = 1. So output of G2 i.e.  is  or 0.
* Now the inputs of G1 are 1 and 0 as R = 1 and  = 0. So output of G1 i.e. Q is  or 1.
* Now suppose Q is previously 0.
* Now the inputs of G2 are 1 and 0 as R = 1 and Q = 0. So output of G2 i.e.  is  or 1.
* Now both inputs of G1 are 1 as S = 1 and  = 1. So output of G1 i.e. Q is  or 0.
* So it is proved that Q remains same as it is when, S = 1 and also R = 1.

**In the above logic circuit if S = 0 and also R = 0, the condition of Q is totally unpredictable. Let's explain how.**


* First suppose Q is previously 0.
* Now both inputs of G2 are 0 as R = 0 and Q = 0. So output of G2 i.e.  is  or 1.
* Now the inputs of G1 are 0 and 1 as S=0 and  = 1. So output of G1 i.e. Q is  or 1. That means Q is changed.
* Now Q is 1. So inputs of G2 are 0 and 1 as R = 0 and Q = 1. So output of G2 i.e.  is  or 1. That means  is unchanged.
* Now the inputs of G1 are 0 and 1 as S=0 and  = 1. So output of G1 i.e. Q is  or 1. That means Q is unchanged.
* So, when both S and R are 0, it becomes unpredictable whether the value of output Q will be changed or unchanged. This       condition of S R latch normally avoided.

![](https://www.electrical4u.com/images/february16/1458318549.png)

--------------------------------------

## Contributors :octocat:

To see a list of all contributors see [here](https://github.com/indrarahul2013/Alisa---An-8-bit-Computer/blob/master/contributors.md)

