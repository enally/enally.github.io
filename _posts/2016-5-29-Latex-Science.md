---
layout: post
title: Latex for Lab Science
category: programming
tags: [science, latex, mathjax]
---

<script type="text/javascript" src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>
<style>
table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
}
</style>
# Latex for Lab Science

## First things first, Disclaimer
I am not by any means a programmer. While I enjoy looking into programming languages and technology, my background is in science. I have found that the more you know about programming, markup languages and software, the easier it is to process a lot of the data generated in chemical science. I have used all of these programs, and while I had some sucsess with them, it was not without trial and error. Your milage may vary.

## What is a markup language?
A [markup language](https://en.wikipedia.org/wiki/Markup_language) is essentially a way of writing text with presentiational or descriptive information included for later use. Any website you visit is originally written in a markup language, such as HTML. It is first written in plain text, and information is added to alter its presentation for later (for example, a word may be tagged as bold, but will not appear as bold at the time of writing). While latex is not exactly a markup language, it is similar in a lot of ways. It is written in plaintext format, and information is added to it which will be used as instructions for how the document will look.

It might not sound like the most appealing thing ever if you're coming from a Microsoft Word background (which most people are), but the use of these properties and tags allows for a great deal more control over the presentation and format of the document, and in the long run actually decreases the time required to write the documents. 

If you're in college studying science, chances are you'll need to do a lot more than type up essays. Lab reports are tedious and often boring, but one of the biggest issues I found was with the requirment of electronic submissions. It's pretty easy to write the pH equations and chemical formulas on paper, but it becomes a bit more difficult when you're doing it on a computer.

What follows is a short introduction to using Latex for chemical and maths equations in lab reports. 

## The Basics
So, I should probably mention at this stage that latex isn't easy. It's tough. It's really tough if you're coming into it without any programming or computer know how. This doesn't mean you can't use it though. Latex is versitle, and used throughout academia for journal publications, but because it's

## Basic Syntax

<p> As far as the basics of maths formulas, latex is pretty straight forward. Plus and minus are the usual characters of `+` and `-`.
Mutliplication and division are a little trickier, because there are no characters on the keyboard to represent them. As latex is used to compile and display information later though, we don't need these symbols to look exactly like what we expect to get at the end. While it might be tempting to use `x` for multiplication, you're more likely to use this as a variable symbol and it will be rendered as such. To get around this problem, we use terms. These allow us to use the term that represents the symbol, and it will be rendered as the symbol later on. For multiplication, we use the term `\times`. By including this, latex will render the term as \( \times \) after the document has been finished. Similarly, we use the term `\div` to render division as \( \div \) later on.
</p>

<p>
When working with anything larger and more complicated, it is useful to use brackets such as `{}`. These are used to contain terms and elements of formatting, and have only the figures inside of these brackets effected. An example of this would be when using powers. 
When using powers, we would use the symbol `^` to indicate a superscript character. By typing `x^2` for example, we would be given \( x^2 \) when we render the text. Now, what happens if we we have more than just these 2 characters? Suppose we have x to the power of 2y. If we use `x^2y`, this is rendered as \( x^2y \). To get around this, we use brackets to specify all that should be effected the the preceeding term. By use `x^{2y}`, we tell the computer that everything inside the brackets are to be rendered in superscript, and as such, we are given \( x^{2y} \) as our output.
</p>

<p>
Terms which require more than 1 operator by default may also require brackets, to speicify what characters are part of what part of the term. Take fractions for example, which use the term `\frac`. Fractions are made of a numerator above the line and a denominator below the line. If we were to represent a half as `\frac12`, the computer would not be able to tell whether it was given 1 and 2 as numerator and denominator, or the number 12 as either of these. This becomes even more confusing with larger fractions, especially when involving variable. We use brackets here to specify which part is which, by writing fractions as `\frac{1}{2}` for a half. This allows use render \( \frac{1}{2} \), and clearly shows which number belongs where. We can include as much as we want in either of these brackets, and the will be placed appropriatly. Brackets also have the benefit of nesting, although depending on the type of equation, this can either increase or decrease the clarity when writing it. 
</p>
> Note: While `{}` is not rendered in the final output, brackets such as `()` are rendered.


## Common Chemistry Equations in Latex
### Arrhenius equation
> `K = Ae^{-E_{a}/(RT)}`
<p>\( K = Ae^{-E_{a}/(RT)} \)</p>

### Henderson-Hasselbalch Equations
> `pH = pK_{a} + \log_{10}(\frac{[A^{-}]}{[HA]})`
<p> \( pH = pK_{a} + \log_{10}(\frac{[A^{-}]}{[HA]}) \) </p>

### Michaelis–Menten kinetics
> `\upsilon = \frac{d[P]}{dt} = \frac{V_{max}[S]}{K_{M} + [S]}`
<p> \( \upsilon = \frac{d[P]}{dt} = \frac{V_{max}[S]}{K_{M} + [S]} \) </p>
## Resources

[Latex2png](http://latex2png.com/)
[ShareLatex](https://www.sharelatex.com/)
