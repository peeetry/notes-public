# Diátaxis documentation framework

*"The grand unified theory of documentation", David Laing*

[This guide](https://diataxis.fr/_/downloads/en/latest/pdf/) "aims to solve the problem of structure in technical documentation", separating all documentation in four "modes", (types/categories):

* Tutorials;
* How-to guides;
* Technical reference;
* Explanation.

"Technical documentation should be structured explicitly around these four types, and should keep them all separate and distinct from each other."

> Remember: documentation is based on the user's needs.

## Tutorials

*Learning-oriented.*

Tutorials are practical step-by-step guides that help the user to get started with the learning. They should "take the reader by the hand thought a series of steps to complete a project". Learning how and not learning what. However, tutorials can be hard to make, time demanding and usually is "the weakest part of documentation". 

The focus is to work the user's confidence, by practicing, through repetition. 

Tutorials must be:

* Meaningful;
* Successful;
* Logical;
* Usefully complete.

Good tutorials "allows the users to form an idea of what they will achieve from the start". You must show clearly what the pupil will be able to do after following the tutorial. 

Create a sense of progression. "The effect of every action should be clear to them as soon as possible. The relation of cause and effect should be evident. Each result should be something that the user can see as meaningful. Every step the learner follows should produce a comprehensible result, however small".

"Resist the temptation to introduce abstraction [...] Tutorials are composed of concrete steps, not abstract discussion [...] The user doesn't need explanations in order to complete the tutorial [...] We are asking a user to do things. The learner is focused on following your directions and getting a result".

Offer only one way to complete the task. "There may be many interesting diversions along the way – ignore them". 

Tutorial language examples:

```
* In this tutorial, you will (describe what the learner will accomplish [not "you will learn"]);
* First, do x. Now, do y. Now that you have done y, do z. (No room for ambiguity or doubt);
* We must always do x before we do y be because... (see explanation fore more details);
* The output should look something like this;
* Notice that... Remember that;
* You have built a secure, three-layer hylomorphic stasis engine. (Describe and admire, in a mild way, what your learner has accomplished [not "you have learned"]).
``` 

## How-to guides

*Task/goal-oriented*

Different from tutorials, how-to guides are just like cooking recipes. "A professional chef who made exactly the same thing multiple times before may still follow a recipe, even if they created the recipe themselves, to ensure that they do it correctly".

It requires a basic level of knowledge and competence.

How-to characteristics:

* Focused on tasks or problems;
* Assume the user knows what they want to achieve;
* Action and only action;
* No digression, explanation, teaching.

Just like tutorials, keep your explanations to the explanation section.

However, "a how-to guide needs to be adaptable to real-world use-cases. A how-to guide that is useless for any purpose except exactly the narrow one you have addressed is rarely valuable.

A how-to guide H1 starts with exactly the "how" word.

```
Good: "How to integrate application performance monitoring".
Bad: "Integrating application performance monitoring".
Very bad: "Application performance monitoring".
```

How-to language examples: 

```
* This guide shows how to (describe clearly the problem or task that the guide shows the user how to resolve);
* If you want, do y. To achieve w, do z. (Use conditional imperatives).
* Refer to the x reference guide for a full list of options. (Don't pollute your practical how-to guide with every possible thing the user might do related to x).
```

## Reference

*Information-oriented*

Technical reference has one job: to describe. It should not explain, discuss, instruct and speculate.

Reference guides describe the product you are talking about. "Describe, as succinctly as possible, and in an ordered way".

References are not to be read. They are consulted.

"Reference material is like a map. A map tells you what you need to know about the territory, without having to go out and check the territory for yourself. A reference guide serves the same purpose for the product and its internal machinery".

Just like and usual Wikipedia page.

`JavaScript is a programming language...`

Accurate, up-to-date, comprehensive information.

"The structure of the documentation should mirror the structure of the product, so that the user can work their way through them at the same time".

Style and form:

* Austere and uncompromising;
* Neutrality, objectivity, factuality;
* Structured according to the structure of the machinery itself.

Provide examples (always use rich, real-world examples). 

Reference language examples: 

```
* X is an example of y. W needs to be initialized using z. This option does that.
* Sub-commands are: a, b, c, d, e, f.
* You must use a. You must not apply b unless c. Never d.
```

## Explanation

*Understanding-oriented*

Explanation docs are explanatory materials. It should clarify, deepens and broadens the understanding of a subject.

It allows the documentation to become discussion. It must make sense if you are reading while away from the product.

"Explanation documentation approaches a topic from a higher perspective, and from different angles".

> It may be less urgent, but not less important.

Can also be called:

* Discussion;
* Background;
* Conceptual guides;
* Topics.

Explanation will help the user to understand what's needed to use the product. It answers the why questions asked by the user while reading the other 3 types of docs. It is for the users who are thinking about the product, not for those trying to use it.

"It can make connections to other things, even to things outside the immediate topic, it that helps".

"Provides background and context in your explanation".

Things to discuss in explanation docs:

* The bigger picture;
* History;
* Choices, alternatives, possibilities;
* Why: reasons and justifications.

It demands the "about" word on the H1. Like:

*"About user authentication"* or *"About database connection policies"*.

"You are not giving instructions or describing facts, you are opening up the topic for consideration".

Explanation language examples:

```
* The reason for x is because historically, y...
* W is better than z, because...
* An x is system y is analogous to a w in system z...
* An x interacts with a y as follows...
```

## Difference between tutorials and how-to guides

They are indeed similar. Both are practical guides. "They exist to guide the user in what to do rather than what there is to know or understand [...] They both describe ordered sequences of actions".

However, a **tutorial** serves the needs of the user who is at study. Its obligation is to provide a successful learning experience and a **how-to guide** serves the needs os the user who it at work. Its obligation is to help the user accomplish a task.

> Tutorials are learning-oriented and how-to guides are task-oriented.

Tutorials doesn't offer choices or alternatives. A how-to guide will typically describe different routes to the same destination.

## The best way to implement Diátaxis

The author recommends that instead of starting everything from scratch, you should update your docs to fit Diátaxis principles.

"Choose something -> Assess it -> Decide what to do -> Do it!

Documentation is never finished. It is like a live organism.

"Similarly, documentation is also never finished, because it always has to keep adapting and changing to the product and to users needs, and can always be developed and improved further. However, it can always be complete: useful to users, appropriate to its current stage of development, and in a healthy structural state and ready to go on to the next stage.