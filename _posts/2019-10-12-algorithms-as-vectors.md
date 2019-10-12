---
layout: post
title: Can we think about programs as vectors? [Things, that fuck up my brain pt. 1 - Mine]
image: /img/posts/2019-08-24-first-post/mr_freeman_avatar.jpg
---

![some cool image]()

I wanted to start this blog with something completely different, but screw this - this is my blog and I can do whatever I want! :D So, fasten your seatbelts and let's begin.

*Sidenote: Those of you with some background can skip to the [Functions as vectors](#functions_as_vectors) section.*

# Algorithm as a function

What is the purpose of an algorithm (like, in general)? It takes some input (eg. some number, image, filled out form, etc.) and produces desired output. Now, we can consider all possible inputs, for which a particular algorithm was designed to take as an input. For example, this can be a set of all natural numbers, or a set of dates sooner than 12-10-2019. Let's denote this input-set as $X$ and each element belonging to it as $x$ (so, eg. the already mentioned set of all natural numbers is marked as $X$ and the number 4 is marked as $x$). Finally, let's say that for any input our algorithm produces exactly one output.

Now, we can think of the set of all possible outcomes of our algorithm in a simmilar fassion as we did in the case of inputs. Then, let's just denote the output-set for a given function by $Y$, and elements belonging to it by $y$.

To wrap everything up, we also need some name for our algorithm. Let's call it $f$. Having all of the above, we can describe an action of our algorithm, as some transition between elements from the set $X$ to the $Y$ set. It can be written down as follows:

$$ X \xrightarrow{f} Y, $$

or in another way:

$$ y = f(x), $$

where:
- $x$ belongs to $X$,
- $y$ belongs to $Y$.

And this looks exactly like a **function**!

Summing up, you can think about any program/algorithm (Skype, reddit webpage, whatever you want) as a function. Well, this conclusion isn't yet anything really astounding...

# Turing machines and Lambda calculus

Now, so that it isn't too nice, let's introduce a little bit of history. There was once a genius man called [Alan Turing](https://en.wikipedia.org/wiki/Alan_Turing). (I really recommend reading his story, this can be really informative...). He came up with a lot of incredible ideas, but today I'm going to mention only one of those - the **[Turing machine](https://en.wikipedia.org/wiki/Turing_machine)**. It's a teorethical model, which can represent any algorithm. It actually initiated the creation of computer science. From Wikipedia we can learn, that:

*A Turing machine is a mathematical model of computation that defines an abstract machine, which manipulates symbols on a strip of tape according to a table of rules. Despite the model's simplicity, given any computer algorithm, a Turing machine capable of simulating that algorithm's logic can be constructed.*

Fantastic! Now, we have to mention the other main player in this field - the [Lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus). In this formalism any algorithm/program can be representad as a specific **function**. Moreover, it has been proved that these two mentioned models are equivalent ways of describing any (computable) algorithm's logic.

I won't go into any more detail about these concepts (those of you, who are interested in learning more I highly encourage to go through at least the provided links), but this is another way of arriving at the same conclusions, as we did earlier.

# <a name="functions_as_vectors"></a> Functions as vectors[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)

Let's switch for a moment from functions to the concept of a **vector**. A vector $\bar{v}$ is usually ilustraded as an arrow in some given space/plane. The properties characterizing vector are: its anchor point, its length (magnitude) and the direction in which it is pointing. The classical picture of a vector is given below[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html):

![vector_1](/img/posts/2019-10-12-algorithms-as-vectors/vector_1.gif)

The above vector can be represented in some other fassion called a $spike diagram$. By plotting the value of the components versus the component index we get[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html):

![vector_2](/img/posts/2019-10-12-algorithms-as-vectors/vector_2.gif)

Note, that the $i$ symbol in the above picture doesn't stand for an imaginary number $i$, but is just some index.

Ok, so ...

![vector_3](/img/posts/2019-10-12-algorithms-as-vectors/vector_3.gif)

![vector_4](/img/posts/2019-10-12-algorithms-as-vectors/vector_4.gif)

![vector_5](/img/posts/2019-10-12-algorithms-as-vectors/vector_5.gif)


# Yeah, yeah, yeah, but who really needs that?

- Kąt między programami.
- Rzut jednego programu na drugi.
- superpozycja programów.

# References

- [1] http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html
