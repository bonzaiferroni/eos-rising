When I was in my 30s I finally learned how to understand computer code and it changed the way I think about almost everything. Programming textbooks teach us about algorithms by using real world examples, like a dog or a tree. Any creature, thing, or process that you can imagine can be modeled as computer code. The closer your model is to reality, the better it works.

There is a part of every computer program that declares its own understanding of reality, at least the part that is relevant to the problem at hand. Sometimes you find it in a folder called `domain` or `model`. For example, maybe you are creating an email app. Within the `model` folder you can expect to find code that declares the essence of an email. 

What is an email? At it's core, it is a document with a subject, a list of recipients, a sender, and a message. So you might write something like this:

```kt
data class Email(
	val to: List<Address>,
	val from: Address,
	val subject: String,
	val message: String,
)
```

It looks innocent but this is a very powerful block of code. Declaring the parts of an email within a `class` gives you the power to summon as many email objects as your heart desires. You could create a legion of emails out of thin air and have them march upon the evil lord of Inboxia. The power to conjure any object I can describe and use it to solve the problem at hand, it feels like a superpower, even if it is all happening inside the computer. So many problems come from inside computers so it is an important power to wield. 

As if that wasn't enough, other developers have captured their most useful spells in code and published them as libraries to import into your code, so that now you can summon all *their* objects too. It is important not to get drunk on the power.

And now I'll get to the point. This morning I was thinking about how to start writing this series of articles and I wished that I could import the work of a sociologist from the nineteenth century, Émile Durkheim. If Émile were alive today, it is possible he'd publish some of his research as Python code that he might use to produce his analysis or simulations of his work. Perhaps he might have elaborate simulations of all his ideas. If he did, I'm certain he would make it open source. I might be able to import the library and play with his ideas.

I will basically do this anyway, at least in my own mind, just in the fuzzy syntax of English. There are a couple reasons I find Durkheim compelling. First, he studied religion and spirituality as if they are real