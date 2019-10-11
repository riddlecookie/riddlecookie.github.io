---
layout: post
title: Can we think about programs as vectors? [Things, that fuck up my brain pt. 1 - Mine]
image: /img/posts/2019-08-24-first-post/mr_freeman_avatar.jpg
---

![some cool image]()

I wanted to start this blog with something completely different, but screw this - this is my blog and I can do whatever I want! :D So, fasten your seatbelts and let's begin.

*Sidenote: Those of you with some background can skip to the [Functions as vectors](#functions_as_vectors) section.*

# Algorithm as a function

What is the purpose of an algorithm (like, in general)? It takes some input (eg. some number, image, filled out form, etc.) and produces desired output. Now, we can consider all possible inputs, for which a particular algorithm was designed to take as an input. For example, this can be a set of all natural numbers, or a set of dates sooner than 11-10-2019. Let's denote this input-set as $X$ and each element belonging to it as $x$ (so, eg. a mentioned set of all natural numbers is marked as $X$ and number 4 is marked as $x$). Finally, let's say that for any input our algorithm produces exactly one output.

Now, we can think of the set of all possible outcomes of our algorithm in a simmilar fassion as we did in the case of inputs. Then, let's just denote the output-set for a given function by $Y$, and elements belonging to it by $y$.

To wrap everything up, we also need some name for our algorithm. Let's call it $f$. Having all of the above, we can describe an action of our algorithm, as some transition between elements from the set $X$ to the $Y$ set. It can be written down as follows:

$$ X \xrightarrow{f} Y, $$

or in another way:

$$ y = f(x), $$

where:
- $x$ belongs to $X$,
- $y$ belongs to $Y$.

And this looks exactly like a function!

Summing up, you can think about any program/algorithm (Skype, reddit webpage, whatever you want) as a function. Well, this conclusion isn't yet anything really astounding...

# Turing machines and Lambda calculus

Now, so that it isn't too nice, let's introduce a little bit of history. There was once a genius man called [Alan Turing](https://en.wikipedia.org/wiki/Alan_Turing). (I really recommend reading his story, this can be really informative...). He came up with a lot of incredible ideas, but today I'm going to mention only one of those - the **[Turing machine](https://en.wikipedia.org/wiki/Turing_machine)**. It's a teorethical model, which can represent any algorithm. It actually initiated the creation of computer science. From Wikipedia we can learn, that:

*A Turing machine is a mathematical model of computation that defines an abstract machine, which manipulates symbols on a strip of tape according to a table of rules. Despite the model's simplicity, given any computer algorithm, a Turing machine capable of simulating that algorithm's logic can be constructed.*

Fantastic! Now, we have to mention the other main player in this field - the [Lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus). In this formalism any algorithm/program can be representad as a specific **function**. Moreover, it has been proved that these two mentioned models are equivalent ways of describing any (computable) algorithm's logic.

I won't go into any more detail about these concepts (those of you, who are interested in learning more I highly encourage to go through at least the provided links), but this is another way of arriving at the same conclusions, as we did earlier.

# <a name="functions_as_vectors"></a> Functions as vectors



# Ok, but why do I need this?

- Kąt między programami.
- Rzut jednego programu na drugi.
- superpozycja programów.

# References
