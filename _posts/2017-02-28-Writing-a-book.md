---
layout: post
title: "Writing a book: Functional PHP"
category: programming
tags: [ php, book, functional-programming ]
published: true
---
Introduction
------------
At the end of July last year, I got contacted by Packt Publishing to write 
a book about a topic that is of particular interest to me: Functional Programming.
More specifically, how to use functional techniques in PHP. It didn't took me long 
to accept. From there, the process moved quickly, by mid August we agreed on an Outline
for the book and I started working on the chapters.

After nearly 5 months of writing and two more of reviews, the result was published on 
February the 14th 2017. It is available both in print and in most digital formats. You
can find all relevant information on the dedicated webpage: [Functional PHP][book].

<!--more-->

It was hard work sometimes, but I am really glad to have been offered this opportunity.
I learned a lot, both about the topic and myself. It was my first experience as an author,
and in this post I want to share a bit about how it was for me. Obviously, I will also try
to present the book as best as I can to give you some incentives to buy it...

[book]: https://www.packtpub.com/application-development/functional-php

Working for Packt
-----------------

This whole book business is new to me, and I don't know how it works with other publisher.
In my case, I was first contacted by an "Aquisition Editor". From what I gathered, their 
role is too find potential new book topics and their authors. Once someone is interested
about writing, they introduce them to the process and help them starting on the outline of
the book. The outline is then vetted by Packt, a schedule is put in place and work on the
content can begin. This step took more or less 3 weeks.

At this point, I was introduced to my "Content Development Editor". They helped me fleshing
out the content of the book by giving me various writing advice and helping me with any
questions I had along the way. They also took care of coordinating the work of the technical
reviewer so that I could act on the received feedback. Due to the holidays, finalizing the
content took a bit more time than expected, but everything went fine.

Mid January, I was introduced to the "Technical Editor". They sent me the final drafts of each
chapters formatted mostly as they now are in the final version so that I could make a last
review of the content. Despite a small issue where some parts of the texts were modified
probably due to some automatic spelling correction, this step went pretty smoothly and 
resulted in the publication of the book in February.

I was well accompanied during the whole time I worked on the book and I heartily thank the
three Packt employees and my technical reviewer for helping me bringing this project to
fruition. I always felt well surrounded.

My writing environment
----------------------

The templates I received from Packt at the beginning where all in Word format. As a Linux
user and open-source proponent, I immediately asked if there was another option to send them
my work. I probably wasn't the first with this kind of request, so I quickly received an
open-document version of the templates.

As I prefer putting everything I work on in version control, I looked for a way use some kind 
of markup language like markdown and then transform it to the final version.

My first try was with [Pandoc][pandoc], but Packt templates have their own styles that must be 
applied on the content, and at the time it was not possible to export Word or OpenDocument files 
with custom styles. This [issue][pandoc-issue] is now resolved, but in the meantime I had to
use some other tool.

[Docutils][docutils] allows to transform reStructuredText to OpenDocument with custom style 
mapping. I've never used reStructuredText before, but as it seemed to be close to Markdown and 
the processor was able to use the styles provided by Packt, I gave it a try. This is finally 
the solution I used to write the book. It wasn't perfect, but in the end it worked out pretty well. 

I wrote a bunch of tooling to help me, you can find it on GitHub: [rst2packt][rst2packt]. The 
scripts were with the idea of publishing them in mind, so they are a bit rough on the edges, but 
they might still help someone also wanting to write a book for Packt, or other publishers for 
that matter.

I wrote the content using the [Atom][atom] editor. I wanted something without too much clutter. 
I didn't bother to find a plugin to help me with reStructuredText as it is a pretty simple markup 
language. The reviews were initially done by sending the OpenDocument files around, but we ended 
up using Google Docs because it was easier for every one. The final drafts were sent to me in PDF 
and I was asked to use FoxIt Reader to add comments. I was happy to find out that they have a Linux 
version that worked quite well.

I opted for a simple writing environment as I hadn't wanted to spent too much time learning new 
tools or setting up things before starting to write. In the end, I think it was a good idea because 
it allowed me to focus on the content itself.

[pandoc]: http://pandoc.org/
[pandoc-issue]: https://github.com/jgm/pandoc/issues/2106
[docutils]: http://docutils.sourceforge.net/
[rst2packt]: https://github.com/krtek4/rst2packt
[atom]: http://atom.io/

Writing Functional PHP
----------------------

This book was my first real writing experience. Sure, I had written some blog posts in the past, 
but the scope of a whole book is something else.

When writing for a blog, you either brush a broad topic or go in depth on a particular specificity,
usually something you just finished doing. This means you can rely mostly on your memory for the 
content while doing only minimal research, at least in my case. Writing a book forces you to revisit
everything you know, or think you know, about a topic to get everything right.

I was mostly able to stay on schedule during the whole process, but looking back I would have loved 
to have more time to write some parts. I agreed to work on this project knowingly, but now that it is
finished, I somehow regret not being able to polish some chapters more.

The review process was also done swiftly and I am pretty sure some silly mistakes on my part weren't
catched by the expert eyes of Packt people. I am however pretty sure the book is fully understandable,
and a potential second edition might correct the few errors left.

I learned a lot both about myself and technically during this whole process. I never had issues writing,
but upon beginning I was a bit stressed that I could experience writer's block. Luckily, it seems I am 
not subject to the condition and I was able to stick to my plan. Obviously I hit some bumps along the way.
For example, my kids fell sick at some point. Packt was however really understanding and I was able to
catch up in the end.

There's a quote going around on the Internet and attributed, probably wrongly, to Einstein stating that 
"You do not really understand something unless you can explain it to your grandmother.". Even if the 
quote is bogus, it proved out to be true for me if we are a bit lax on the grandmother part. I was under
the impression that I understood a lot of the topics discussed in the book, but having to explain them
in writing really forced me to get further. 6 months later I am a much better developer than I was before
starting this book.

Why you should buy it
---------------------

I am not good at selling myself or my work, so instead I will try to sell you functional programming
itself in the hope to spark your interest. I will not discuss the topic at length here however, 
especially since I already wrote a blog post about it in the past: [Functional programming in PHP][liip]

Functional programming is not a new idea. It has its roots in lambda calculus, an idea formalized 
in the thirties. Lisp, one of the first programming language, has a lot of functional features. Since 
then, a lot of languages either takes a lof of concepts from the functional paradigm or a purely 
functional. Today, Haskell and Scala are probably the functional languages ones hear the most about.

In the last years, we hear of functional programming in a regular basis. New languages, like Swift, 
have deep ties to the functional ideas. The Javascript community expresses lots of interests for the 
concept. In 2012 already, John Carmack, famous for being of the creator of Doom and Quake, offered 
a [pragmatic approach to improve C code using functional programming][carmack].

Why such an interest? There are multiple reasons, here is my own opinion on the topic:

* By removing the need for a global state, encouraging small functions and improving the locality of 
  concerns, functional programming **reduces the cognitive burden** on the developer and makes it 
  easier to understand and reason about a piece of code
* Pure functions, or a function for which the output is always the same for a given set of input, 
  are a **lot easier to test** than functions having side-effects. This helps writing robust software 
  with less bugs.
* Code without side-effect is also a **easier to refactor** because your modifications won't have 
  unforeseen results in other parts of the application.
* Most of what is enforced by functional programming is more often than not considered a **best practice**.
* Writing **distributed code** or code executed in parallel is a made easier by not having a global state.

Without some prior knowledge about functional programming, my list might be a bit difficult to completely 
understand, but this post is already long enough. All of those points and a lot more is explained more in 
depth in the book.

Also, in order to be completely transparent, I must warn you that you won't be able to get the full
benefits of functional programming when developing in PHP. Each version has more features allowing
for advanced techniques, but PHP is still an imperative language at its core. However, as I try to
explain in the book, functional programming is first and foremost a way of thinking. It means that
even if you are not able to write purely functional code, you will grow as a developer by learning
about functional programming.

If you want to learn some novel ways to approach a problem, learn to write cleaner code, or be 
introduced to functional programming using a language you know and love, I think my book can help you.
It is also written in a way that will allow you to understand reference material available both in
books and online but not targetting PHP directly.

Obviously, I am a bit biased, but I would have loved having such an introductory book at my disposition
when trying to learn functional programming instead of having to learn a completly new language at
the same time. By leveraging the knowledge you already have in PHP, you will be able to be up to
speed far quicker.

I can only hope I convinced you to learn more about the topic and that you will chose my book
to do so. If you have any questions either about the topic, my book, or the scripts, I will gladly
answer to you by e-mail. Finally, here is the link to the book webpage once again: [Functional PHP][book].

[liip]: https://blog.liip.ch/archive/2014/11/05/functional-programming-in-php.html
[carmack]: https://web.archive.org/web/20130819160454/http://www.altdevblogaday.com/2012/04/26/functional-programming-in-c/
