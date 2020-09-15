---
layout: post
title: Can we think about programs as vectors?
subtitle: [Mind twisters pt. 1]
image: /img/posts/2019-10-12-algorithms-as-vectors/avatar.jpg
---

![header](/img/posts/2019-10-12-algorithms-as-vectors/header.jpg)

You're sitting in subway responding to a message you got from a friend on the Messenger. Suddenly, a pop-up informs you, that someone liked a photo from your last vacation, that you posted on Facebook. With a smile on your face you open the reddit app to check the \"Popular\" page, but it's your station. You grab your things, get out from the car and go to work. There, you sit at your desk, turn on the computer, open Outlook and Chrome and a normal day at the office is just beginning.

In our day to day life, we often don't have time to sit for a moment and think about the surrounding world (or, we rather tell ourselves, that we don't have time for that), not to mention moving to higher levels of abstraction of looking at normal things. But today I'm going to take you on a journey. We will start very simple, by looking at the things, that all of us use every single day - programs. Apps, browsers, games, webpages... All of these are in general just programs. As the path in front of us unfolds, I will take you to higher and higher levels of abstraction. At the end, I will try to convince you for example, that we can imagine such a thing as an angle between the Facebook and reddit pages.

So, without any further ado, let's just dive into the subject.

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

*"A Turing machine is a mathematical model of computation that defines an abstract machine, which manipulates symbols on a strip of tape according to a table of rules. Despite the model's simplicity, given any computer algorithm, a Turing machine capable of simulating that algorithm's logic can be constructed."*

Fantastic! Now, we have to mention the other main player in this field - the [Lambda calculus](https://en.wikipedia.org/wiki/Lambda_calculus). In this formalism any algorithm/program can be representad as a specific **function**. Moreover, it has been proved that these two mentioned models are equivalent ways of describing any (computable) algorithm's logic.

I won't go into any more detail about these concepts (those of you, who are interested in learning more I highly encourage to go through at least the provided links), but this is another way of arriving at the same conclusions, as we did earlier.

# <a name="functions_as_vectors"></a> Functions as vectors<sup>[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)</sup>

Let's switch for a moment from functions to the concept of a **vector**. A vector $\bar{v}$ is usually ilustraded as an arrow in some given space/plane. The properties characterizing vector are: its anchor point, its length (magnitude) and the direction in which it is pointing. The classical picture of a vector in two dimensions is given below<sup>[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)</sup>:

{% include image.html url="/img/posts/2019-10-12-algorithms-as-vectors/vector_1.gif" description="An example vector in two dimesnions." %}

The above vector can be represented in some other fassion called a $spike\ diagram$. By plotting the value of the components versus the component index we get<sup>[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)</sup>:

{% include image.html url="/img/posts/2019-10-12-algorithms-as-vectors/vector_2.gif" description="The first vector presented using the $spike\ diagram$." %}

(Note, that the $i$ symbol in the above picture doesn't stand for an imaginary number $i$, but is just some index.)

Now, we can move from two dimensions three and more<sup>[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)</sup>:

{% include image.html url="/img/posts/2019-10-12-algorithms-as-vectors/vector_3.gif" description="$Spika\ diagram$ of a vector in three dimensions (left) and some larger number of dimensions (right)." %}

Let's do one step further. What happens, if we move to an infinite number of dimensions? We would ilustrate a vector belonging to such a space like this<sup>[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)</sup>:

{% include image.html url="/img/posts/2019-10-12-algorithms-as-vectors/vector_4.gif" description="A vector with infinitely many components." %}

But hey, if we lead a curve through all upper vertices of our spikes, we get something that look's just like a plot of some function! (Actually, that's why it's denoted as $f(x)$ in the above picture.) So, if we get rid of the spikes themselve, we are left with only the plot of our function<sup>[1](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)</sup>:

{% include image.html url="/img/posts/2019-10-12-algorithms-as-vectors/vector_5.gif" description="Thr plot of a function corresponding to a vector with infinitely many components." %}

Summarizing: using the above logic, we can think of functions as vectors with infinitely many components! But be careful, because it doesn't always work the other way around.

Finally, we've already shown, that an algorithm is nothing more than just a function. An additionally, a function can be seen as a vector. Thanks to that, we can easily come to the conclusion, that **algorithms themselve can be viewed as vectors**!

# Yeah, yeah, yeah, but who really cares about that?

Honestly, in a day to day life probably nobody. But for me it's fucking awesome! I think, that it's good to sometimes think about seemingly trivial things in a more abstract way, or view something from a different angle. But if this doesn't convince you, let me wreck your brain a little bit more. Below are two conclusions, that came to my mind.

Firstly, if two algorithms/programs can be seen as a vectors, it's theoretically possible to calculate an angle between them (don't aks me how, I just guess that it's possible). Can you imagine an angle between YouTube and Facebook pages? (This is a slight exaggeration, but you know what I'm talking about.) Moreover, maybe it's possible to project one program onto the other?

Secondly, have you ever heard about the [Schrödinger's cat](https://en.wikipedia.org/wiki/Schr%C3%B6dinger%27s_cat)? It is described shortly below<sup>[2]</sup>:

*"A cat, a flask of poison, and a radioactive source are placed in a sealed box. If an internal monitor (e.g. Geiger counter) detects radioactivity (i.e. a single atom decaying), the flask is shattered, releasing the poison, which kills the cat. The Copenhagen interpretation of quantum mechanics implies that after a while, the cat is simultaneously alive and dead. Yet, when one looks in the box, one sees the cat either alive or dead, not both alive and dead."*

{% include image.html url="/img/posts/2019-10-12-algorithms-as-vectors/schrodingers_cat.svg" description="The artist's representation of a Schrödinger's cat thought experiment. [ii]" %}

So, as long as the box is closed, the cat is at the same time alive and dead. Put it another way, a cat is in a **superpositon** of being alive and dead. The concept of superposition is a fascinating topic in itself, but I won't describe it in here. You just need to know, that **if we have two vectors written down in some common basis, we can superpose them**. So, you can imagine a quantum Firefox browser, which until you look at the screen shows at the same time the BBC and The Guardian pages, but when you finally want to check what's going on around the world, it collapses to only one of those pages (with some probability).

There is a field of science on the intersection of computer science and quantum physics, which examines [quantum information](https://en.wikipedia.org/wiki/Quantum_information) and [quantum computation](https://en.wikipedia.org/wiki/Quantum_computing), where this could be actually aplicable! Moreover, when (or if) a reasonably big quantum computer will be finally built, and by big I mean one with a large number of [quibts](https://en.wikipedia.org/wiki/Qubit), this idea would not seem so abstract anymore.


Wow, it came longer than I expected, but I hope you enjoyed it. For those of you, who are still interested in the topic, can read a discussion under my post on reddit concering exactly the same things, as I described above:

<https://www.reddit.com/r/compsci/comments/cwyk3a/thinking_of_programs_as_vectors/>

Thanks for reading!

<div style="text-align: right"> - Cookie monster </div>


### References

- [1] [Functions as vectors](http://eng.fsu.edu/~dommelen/quantum/style_a/funcvec.html)

- [2] [Schrödinger's cat](https://en.wikipedia.org/wiki/Schr%C3%B6dinger%27s_cat)

### Images

- [i] [Header image](https://blog.algorithmia.com/algorithm-development-is-broken)

- [ii] [Schrödinger's cat image](https://upload.wikimedia.org/wikipedia/commons/thumb/9/91/Schrodingers_cat.svg/330px-Schrodingers_cat.svg.png)
