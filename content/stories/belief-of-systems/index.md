# The Belief of a Search System

… and doing the best despite uncertainties

*So as it is our last day, I thought to share some thoughts/aids/ideas that helped me understand some of the concepts like fundamental to so many things that we've been studying. I don't doubt that there would be plenty of mistakes (and dimness in labels) for a first draft, and will be glad to receive any and all corrections and feedback :)*

____

So you're a Search System. Everything you know is comprised in a Library of Knowledge full of scrolls and docs

![The World.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20World.png)

and your job is to find and give Seekers what they need based on what they tell you.

![The Truth.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Truth.png)

You have a knack for finding things, and for doing what you're told, so you imagine that for any *need of knowledge* that they might have, If your docs-world has the truth, in these docs, you'll find and guide them to the Truth and nothing else.

![The Truth Retrieved.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Truth%20Retrieved.png)

In an ideal, rainbows-and-unicorns world.

Unfortunately for you, there is an interface the user's need has to pass through before reaches you: which is *how well they can express their thoughts*.

All you can get is a ***query***, an rough idea, of what their need is. With that, you have to guess your best to divide your docs world into what you *think* is correct and not. 

And given how far off the query was from the need, your guess might be ... well, a bit patchy.

![The Guess.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Guess.png)

![The Guess Retrieved.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Guess%20Retrieved.png)

You decide to find at least know just how far off you really are, rather than leaving everything upto chance, so you can maybe find tricks to do better. 

## The Elusive Truth

But just *how* far your guess is from the real deal? You notice three main areas

- **The Extra Part**: in the guess, it has things added that <u>should not</u> have

![The Extra Part.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Extra%20Part.png)

- **The Missed Part**: in the truth, which are things removed/not selected that <u>should</u> have

![The Missed Part.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Missed%20Part.png)

And then of course,

- **The Correct Part**: the one Both have, things that should have been added and are added, the correct/good part, where both are same --> the green part.

![The Correct Part.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Correct%20Part.png)

## The Dilemma

There seem to be two ways to correct the error then. You don't have control on the real part, just on the guess. So, you can,

- grow the guess: absorb more of the Missed

- reduce the guess: reduce some of the Extra

But this can't be done without a Seeker's help.

So the next seeker that comes up to you and states his need, you give the docs and ask,

You: "Hey, so any thoughts about the results?"

Seeker: "Yeah they're nice, though there are some wrong docs in here too."

You: "I can think of a way to imporve them maybe. Could you try to be more specific, and maybe remove some words?"

![The  Guess No Extra (no text).png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20%20Guess%20No%20Extra%20(no%20text).png)

Seeker: "Yeah now *all* of these seem fine, there's no wrong ones, and looks like there are quite a few missing"

![The Guess No Extra.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Guess%20No%20Extra.png)

You: "Well, what if you added more words and were more general?"

![The  Guess Catching everything (no text).png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20%20Guess%20Catching%20everything%20(no%20text).png)

"Yeah now there's everything I wanted, what are all these other things?"

![The  Guess Catching Everything.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20%20Guess%20Catching%20Everything.png)

Hmm.

It seems there are two very different ways of *doing well*, each of which is good in one way, but bad in another.

And, you realize, unless the **initial offset** between query and need is cured, or you're *very* lucky, you're never going to do well on both.

## The Types of Goodnesses

So it seems you need to track both these cases of your searches. 

Two points strike you that might be good pointers:

**Quantity**: How well you were able to catch everything. It shows you *correct* things *removed* mistakenly.

That would basically be *your catch* vs *everything correct*.

That is, **your correct guess ÷ truth**

![Quantity.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Quantity.png)

The other one is **Quality**: How well did you avoid being wrong. It shows *wrong* things *added* mistakenly.

Which would be *your catch* vs *everything you got* 

That is, **your correct guess ÷ guess** 

![Quality.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Quality.png)

Not bad. The only trouble now is that you're having some difficulty measuring all those areas.

## "Finding things" is everywhere

To fix the squiggly shape area problem, you dumb it down removing unnecessary details, that makes it easier.

![To Boxes.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/To%20Boxes.png)

Hang on. This looks familiar.

It look just like something your friend, who is an **Object Detection System**, does.

![Object Detection.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Object%20Detection.png)

You're quite excited and show it to her. She's very interested, but then points out that it's actually not surprising, and in fact your measures are real and actually have names:

- Measuring Quality is usually called ***Precision***: So for her, how well her guess catches *only* the object.

- Measuring Quantity is on the other hand called ***Recall***: How well her guess gets *all* of the object

![New Names.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/New%20Names.png)

What's more, there are even more names. The extra part, for example is called a *False Postive*. The missed part on the other hand is called a *False Negative*. And the correctly guessed part is called a *True Positive*.

<img title="" src="file:///Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/FN%20TP%20FP.png" alt="FN TP FP.png" width="710">

Woah, that's neat.

You start to ask her how does *she* measure them, but them remember that she really just has all the box widths and pixel values which are pretty convenient.

But your corpus and guesses do not have any apparent shape ...

... which actually might be a good thing. Maybe you don't even have to stop at this box shape.

## The Proportions

You keep trying things out, and then something hits you.

Maybe there's no real reason for the guess and real blobs to be in the middle. (And let's just increase the sizes so they're easier to work with)

![The Transformation.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/The%20Transformation.png)

Ah, now everything is proportional to the big Docs Box. That should make measuring things a bit easier.

So Precision and Recall would now look like,

![Equivalence.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Equivalence.png)

Working with proportions seems pretty convenient.

Say if there are 10% true docs, then we don't have to know the actual number of docs.

![Prior 10 percent.png](Prior%2010%20percent.png)

Also, you had heard somewhere that percents can be thought of as measuring the chance, or "probability".

So if you just got 1 doc from the entire store, it would have a 10% chance of being correct.

To put in an another way, **P(was true) = 10%**

You decide to go even further. To see what happens when you guess.

Say the Seeker gives you a query, and 70% of correct docs satify it, along with 5% of the incorrect ones.

![Percents After Guess.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Percents%20After%20Guess.png)

This means you know you got 70% of correct ones. 

It sounds very familiar ... wait isn't that just Recall? 

Also, 70% of correct ones is also just another way to say *the chance that a doc was guessed, given it was true (limiting ourself to just true docs), is 70%.*

That is, **P(doc_was_got | doc_was_true) = 70%**

Which means, all of these are equivalent:

![Recall Calculation.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Recall%20Calculation.png)

So we have had our Recall with just proportions or rather, probabilities.

Can we do precision too in a similar way?

## The Bayes Case

![Precision Box diag.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Precision%20Box%20diag.png)

Precision looks like it is very similar. The correct docs (green part) are still in the focus, but here you compare it with respect to the ***guess*** (yellow) part rather than the true part.

So looks like here Precision would also be a probability, but a flipped one; it would say: "Given you got a doc, what is the chance it was true?",

Which is **P(doc_was_true | doc_was got)**

But for that you need the areas of the green and yellow. Not a problem, you can find them with the percents you know.

![Precision Components Areas.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Precision%20Components%20Areas.png)

This means Precision is,

![Precision Calculation.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Precision%20Calculation.png)

Oh, but wait.

We already know that the 

- 10% is **P(doc_was true_)**

- 70% is **P(doc_was_got | doc_was true)**

In the same way, 

- 90% is **P(doc_was_not_true)**

- 2% is **P(doc_was_got | doc_was_not_true)**

Also, that denominator is just the entire guess, which is **P(doc_was_got)**

And so, you find Precision to be, 

![Precision Probabilities.png](/Users/prateekshasingh/Dropbox/stories/the-belief-of-systems/Precision%20Probabilities.png)

Woo! Can't wait to show this interpretation your friend, bet she hasn't seen this one before.

--

You slowly begin to realize that whatever are any of those docs, even if you don't know their exact count, just a rough ratio, or a chance how many they might be, you *still* have a way to know how good we'll be.

Of course, everything still much upto chance. But something hits different.

It's like you now know exactly just how much that chance is :)

## Credits

**Concepts**: CSE 535 by Prof. Srihari, Information Retrieval by Chris Manning, Bayes Theorem by 3Blue1Brown

**Style**: Lauren Ipsum, Wait But Why, Vihart, Advent of Code, HPMoR

**Based on**: Precision and Recall, Bayes Theorem, and the probablistic approach to IR

**Illustrations** made in figma, a wonderful tool. 

In the works: "Spinoff: So you're a Medical Test"

*It has been awesome studying with you all. Thanks to the entire 535 team for making this a wonderful experience. See you around, and have an amazing holiday :)*

____

## Scraps

Link to workboard: [Figma](https://www.figma.com/file/l2NG6ikWz8l9scFb50ffgQ/Belief?node-id=0%3A1)

So labelling all of them, putting in some example numbers just to get an idea:

Say there are total 10k docs (1), and 1k of those are right.

The Seeker gives you a query, and you are able to guess 700 correct and 180 incorrect docs.

[labelled world]

The measures would be:

P = 700 / 700 + 180 = ____

R = 700 / 1000 = 0.7

[diag fractions from earlier = number fraction colored = answer in bold]

Just for the record, you rewite the earlier example

[diag fractions from earlier = number fraction colored = answer in bold]

Meaning, if 10% out of 100% docs are correct, then

**10%** is chance the ANY given doc from entire World is Correct : **P(it_was_Correct)**

which is this. **[just Prior box]**

[BIG chart]

you ponder ...

- Then this must be the chance any doc is guessed.

- And of course, this then

--

It looks as if she could use this system as well, on checking how much extra image she added with Precision, and how much she missed with Recall.

And it seems in this case, Precision seems to be the c**hance that a fetched document was correct**

You look up on some way to write it, looks like it is written as

**P(it_was_Correct | doc_was_got)**

But then can the other percents be called chances as well? you look excitedly

**10%** is chance the ANY given doc from entire World is Correct : **P(it_was_Correct)**

**70%** is chance that Correct document was fetched, or doc was fetched given it was correct: **P(doc_was_got | it_was_Correct)**

**15%** is chance that InCorrect document was fetched

But isn't all this just **P(doc_was_got)**

--

Your precision is: green / green + yellow = **P(it_was_Correct | doc_was_got)**

= 70% * 10% [of the total area] / (70% * 10% + 15% * 19%) of the total area

if the initial box was 100% and if 10% initial docs were correct (blue),

[pic: prior, labelled with percents]

and you got 70% of those correct ones (green), and 15% of incorrect ones (yellow)

[pic: both correct incorrect, labelled with percents ]

Your precision is: green / green + yellow

= 70% * 10% [of the total area] / (70% * 10% + 15% * 19%) of the total area

--

[Again, the guess is correct for all you know, to your best *beliefs*. But by starting from shaky ground (the approximate query), you have no way of knowing the real need]

### Dividing the World

PoV

Flesh out, independently first, only then you'll know the relations

### Probability IR as well (NOPE: the Bayes diagram, but hard to explain)

Something about this initial offset really irks you. It seems things are always going to be uncertain.

You want to be able to say "given your initial query,If I gave you a doc, this is the chance if is correct"

my_given_doc = doc_given

P(C | my, q)

It seems P(C | doc_I_gave, q) is really

and that seems equal to this, which is really P( doc_I_gave | )

You had heard about Baye's theorem, but never knew it would be similar to precision.

When you give these "I think these are relevant" docs, you unknowingly divide your docs world into retrieved and not retrieved docs.

This is your approximation of relevant docs.

- makes it to 

2 ways to correct then:

Trial 1:

- absorb more of the green part :

- reduce some of the blue part

No ...

Trial 2:

- grow the approximate part

- reduce the real part

No ... that doesn't seem right either, you don't have control on the real part

Trial 3:

- grow the approximate part

- reduce the approximate part

Ah, that seems to be it. It is actually the same as Trial 1

Trial 4:

- grow the approximate part: absorb more of the green part

- reduce the approximate part: reduce some of the blue part

You try and think how the user can help, and how phrasing their query can help in catching more of that green missed "real" part. Maybe if the user added some more words it would help?

But that would make the approimate part grow, which means even the extra added things could also grow.

On the other hand, if

And you're given a query like "Apple".

For you, at any time, this world will be divided into relevant and non relevant document

## Aside: Your CV friend

You tell about this to your CV, who it turns out, was using the similar concept for measuring her errors.

You kind of see similar measure being used for a friend of yours that detects objects in images

[pic: side by side square case of IR and IP,

(there too there is the correct part (the ground truth object) and the]
