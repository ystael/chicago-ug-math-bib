# The foundation

## Contents

* [Introduction](#introduction)
* [Recommended](#tldr)
* [Calculus of one variable](#calculus-one)
* [Calculus of several variables](#calculus-several)
* [Linear algebra](#linear)
* [Ordinary differential equations](#ode)

## <a name="introduction"></a>Introduction

There is a set of math topics which used to be thought of as covering the first two years of an
undergraduate curriculum in any quantitative discipline. Roughly speaking these are calculus of
one and several variables, linear algebra, and ordinary differential equations. Depending on
the specific discipline you might throw in the basics of Fourier analysis, or a bit of
statistics, but fundamentally calculus, linear algebra, and differential equations are what you
have to have.

Nowadays it's common for strong students to arrive at university with most or all of this from
high school, or maybe calculus and some other enrichment topics. And linear algebra and
differential equations are so often _taught_ with an applied and computational bias, because
that's what students outside pure math need, that pure math students and teachers might ignore
these topics, or hand-wave them away as "something you can pick up in a few weeks when you need
to". It's entirely possible to emerge from a strong undergraduate program in pure mathematics
almost completely ignorant of what the eigenvalues of a matrix are good for, or how to solve
even the simplest differential equation. I know, because I did!

But these topics _are_ foundational, and I wish I had learned them better when I had the
chance. Having applications doesn't magically make a piece of math boring, and it doesn't mean
you have to approach it as an unmotivated cookbook of procedures to memorize. 

## <a name="tldr"></a> Recommended

* Calculus of one variable
  * [Spivak](#spivak-calculus) if you want to bias toward theory ("baby real analysis")
  * [Apostol volume I](#apostol-calculus-i) if you want to bias toward computations and
    applications
* Calculus of several variables
  * [Apostol volume II](#apostol-calculus-ii)
* Linear algebra
  * [Artin](#artin-algebra) for a theory bias
  * [Strang](#strang-linear-algebra) for an applications bias
* Ordinary differential equations
  * [Arnol'd](#arnold-ode) for a theory bias
  * [Birkhoff & Rota](#birkhoff-rota-ode) for an applications bias

## <a name="calculus-one"></a> Calculus of one variable

For students who want to focus on learning theory, the One True Calculus Book is what Chicago
uses for honors calculus:

#### <a name="spivak-calculus"></a> Michael Spivak, *Calculus*

This is a book everyone should read. If you don't know calculus and have the time, read it and
do all the exercises. Parts 1 and 2 are where I finally learned what a limit was, after three
years of bad-calculus-book "explanations". The whole thing is the most coherently envisioned
and explained treatment of one-variable calculus I've seen (you can see throughout that Spivak
*has a vision* of what he's trying to teach).

The book has flaws, of course. The exercises get a little monotonous because Spivak has a few
tricks he likes to use repeatedly, and perhaps too few of them deal with applications (but you can
find that kind of exercise in any book). Also, he sometimes avoids sophistication at the expense
of clarity, as in the proofs of Three Hard Theorems in chapter 8 (where a lot of epsilon-pushing
takes the place of the words "compact" and "connected"). Nevertheless, this is the best calculus
book overall, and I've seen it do a wonderful job of brain rectification on many people.

**[Pete Clark]** Yes, it's good, although perhaps more of the affection comes from more advanced
students who flip back through it? Most of my exposure to this book comes from tutoring and
grading for 161, but I seriously believe that working as many problems as possible (it must be
acknowledged that many of them are difficult for first year students, and a few of them are
*really* hard!) is invaluable for developing the mathematical maturity and epsilonic technique
that no math major should be without.

#### <a name="apostol-calculus-i"></a> Tom Apostol, *Calculus* volume I

If you're looking for a rigorous treatment of calculus that makes more contact with applications
and provides more computational practice problems than Spivak does, Apostol is what you want. MIT
uses this book for 18.014, their honors single variable calculus class.

Apostol's writing is fairly dry -- this book won't change your life or your perspective on math
the way Spivak can. But it's a clean, careful exposition of the standard single-variable calculus
material, *including* the standard applications, and even a brief introduction to ordinary
differential equations. You get complete proofs, and you don't get the endless, dubiously helpful
pedagogical apparatus that makes mainstream textbooks so heavy and so unbearably tedious.

Incidentally, this book follows the tradition of Courant in presenting the integral before the
derivative, or even limits and continuity.

#### <a name="hardy-course-pure-mathematics"></a> G. H. Hardy, *A course of pure mathematics*

#### <a name="courant-diff-int-calculus-i"></a> Richard Courant, *Differential and integral calculus* volume I

These two are for "culture". They are classic treatments of the calculus, from back when a math
book was rigorous, period. Hardy focuses more on conceptual elegance and development (beginning by
building up **R**). Courant goes further into applications than is usual (including as much about
Fourier analysis as you can do without Lebesgue integration). Think of Spivak and Apostol as the
lineal descendants of Hardy and Courant respectively.

They're old, and old books are hard to read, but usually worth it. (Remember what Abel said about
reading the masters and not the pupils!)

Courant's book was revised with Fritz John as *Introduction to calculus and analysis* (about which
see more [below](#courant-john-calculus-analysis-ii)).

## Calculus of several variables

By this I mean the traditional three-space vector calculus, including line, surface, and volume
integrals, the theorems of Green, Gauss and Stokes, and usually some extra topics such as
constrained optimization using Lagrange multipliers. This material can be treated at a wide
variety of levels of sophistication. To do differential calculus in space ethically requires at
least a bit of topology; to prove Stokes's theorem fully needs quite a bit more.

For this reason some people might urge ambitious pure mathematics students to skip this area
entirely in favor of deriving it from analysis in **R**^n later (as Baby Rudin does in a few pages
at the end of Chapter 10). I can't recommend this. It's worth sharing a language with the people
around you and knowing what their applications are, and if you never learned basic vector
calculus, you're going to have a lot of trouble when you want to study magnetic fields! (If you
had the cookbook version in high school and you're comfortable doing computations, the advice to
skip is much more reasonable.)

For these more sophisticated treatments, see [Calculus in Euclidean
space](ground-floor-analysis.md#calculus-euclidean) -- although the books reviewed here already
lie quite a bit farther in that direction than, say, Stewart.

#### <a name="apostol-calculus-ii"></a> Tom Apostol, *Calculus* volume II

If you read Apostol volume I, you know what to expect here; in fact the last two chapters of
volume I reappear at the beginning here, as part of a nearly complete first course in linear
algebra. Following that, and a good chunk of a first course in differential equations too, Apostol
covers the multivariable calculus material in about 200 densely packed pages. In a sense there's
nothing surprising here, except that there are so few books on this topic at this level that you'd
want to keep.

#### <a name="courant-john-calculus-analysis-ii"></a> Richard Courant & Fritz John, *Introduction to calculus and analysis* volume II

The second volume of Courant's *Differential and integral calculus* was revised much more
substantially than the first, and because of the way standards of rigor have evolved, you're
likely to find the older one quite confusing. Courant and John cover linear algebra and
differential equations in much less depth than Apostol does. In exchange, there's a wider variety
of applications treated at length, and a more in-depth discussion of the geometry and topology
involved in multivariable calculus.

## Linear algebra

Every student of mathematics needs the basics of linear algebra, but not every student needs to
get them from a linear algebra textbook. If you went through Volume II of Apostol's calculus book,
you have most of a first course in linear algebra already. He doesn't cover some more advanced
topics, but the fundamental language you use every day is in there, and you may well be able to
put off learning the rest.

I *don't* recommend, however, doing as I did and trying to extract what you need from the
structure theory for modules over a principal ideal domain. A misguided belief in the superiority
of Bourbakiste abstraction over pedestrian applicable mathematics meant I stayed far too ignorant
for far too long. Learn the basics properly, and you will find their mirrors everywhere.

#### <a name="artin-algebra"></a> Michael Artin, *Algebra*

Strong, theory-minded students should consider starting here rather than a linear algebra
text. Uniquely among first courses in abstract algebra, Artin's book puts matrices and vector
spaces front and center from the very beginning, and keeps them there for the entire first half as
an explicit object of study and an endless source of motivating and justifying examples for group
theory. This is the *only* book I would recommend to someone who wants to "skip linear algebra"
and go straight to abstract algebra, because it is the only book I know that won't leave you
dangerously ignorant at the end. If you are able and willing to invest some time into group
theory, you'll come out with a very strong unified picture of the subject. The chapters on matrix
groups and representation theory are just the cherry on top of a wonderful, rewarding book that
never loses sight of the concrete reasons to study any given abstraction.

#### <a name="strang-linear-algebra"></a> Gilbert Strang, *Linear algebra and its applications*

Students looking for emphasis on applications should start here instead. Instead of unifying
linear algebra with group theory as Artin does, Strang's book unifies linear algebra with the
computational algorithms and processes that matrix operations represent. The emphasis on
techniques used in real scientific computing begins at the very start, with a discussion of why
you use Gaussian elimination rather than determinants, and continues throughout. The Jordan
canonical form is relegated to an appendix; in its place appears the (vastly more useful in
practice) singular value decomposition.

This book definitely does not assume as much sophistication from the student as Artin. If you made
it through multivariable calculus, you'll be fine here. It's hard to be rigorous, accessible, and
enjoyable at the same time, but Strang pulls it off brilliantly; his enthusiasm for the subject as
it appears in everyday applied practice is evident throughout.

#### <a name="axler-linear-algebra"></a> Sheldon Axler, *Linear algebra done right*

This book is really a polemical project. Axler set out to write a rigorous linear algebra text
(it's advertised as a "second course", for students who have already seen a low-level treatment)
that avoids discussing determinants until the very end. His argument is that determinants are an
opaque and magical construction, by which you get too-quick proofs of basic facts that obscure the
underlying geometric structure. (The book being aimed at pure math students, "determinants are
numerically horrible" is mentioned only in passing.)

I think he's right, and it's a good book for what it is, but if you can handle this book, you can
probably handle Artin, and get your linear algebra embedded in a wider context with a richer set
of examples.

See also the polemical reaction to this polemic, namely [Linear algebra done
wrong](http://www.math.brown.edu/~treil/papers/LADW/LADW.html) by Sergei Treil.

#### <a name="halmos-fdvs"></a> Paul Halmos, *Finite dimensional vector spaces*

This is a linear algebra book written by a functional analyst, and the crux of the book is a
treatment of the spectral theorem for self-adjoint operators in the finite-dimensional case.
It's a beautiful, wonderful book, but not a very good reference for traditional linear algebra
topics or applications.  You also have to read a fair distance before you even see a linear
map, and the exercises are mostly too easy, with a few too hard.  But this book was where I
first learned about tensor products, and why the matrix elements go the way they do and not the
other way (Halmos is very careful on this point).

**[Pete Clark]** I own this book and read through it often, but it's never taught me linear
algebra per se.  Let's agree that it's too abstract for a reasonable first introduction to
linear algebra; it's really meant for students who already know (some) linear algebra to read
through and appreciate one particular, and particularly elegant, presentation of the material.
If you want to know about the linear algebra which surrounds functional analysis, then by all
means read this book, but much of the material is nonstandard and a bit curious from the
perspective of mainstream linear algebra; projections seem to be the most important linear map,
and there are many sections lovingly devoted to commuting projections, decomposing projections,
etc.  I still am not sure why Halmos deifies the \[,\] as much as he does, and quite honestly,
I would learn multilinear algebra anywhere but here.

#### <a name="curtis-abstract-linear-algebra"></a> Morton Curtis, *Abstract linear algebra*

If you can stand terrible typesetting and an unexciting prose style, this tiny little book is a
good rigorous reference for traditional linear algebra (i.e., it doesn't assume you're a tree).
A nice bonus at the end is the Wedderburn theorem for division algebras over **R**, although
the lack of sophistication makes for some unmotivated technical carpentry.

## Ordinary differential equations

Unlike the case of linear algebra, *how much* you need to know about ordinary differential
equations is often debated. Some people argue that the classical techniques of solving
differential equations are basically useless -- that all you really need are the basic existence
theory (local straightening of vector fields) and linear systems with constant coefficients (via
the matrix exponential); and all the interesting material beyond there belongs to dynamical
systems. Gian-Carlo Rota himself famously espoused this view in his essay "Ten lessons I wish I
had learned before I started teaching differential equations", where he criticized most of the
content of standard texts (including his!) as historical relics.

Students considering analysis or applied mathematics, however, might find themselves wishing they
had learned more about Laplace transforms or Bessel functions or the hypergeometric equation; and
in cases like this a more traditional text might be called for.

#### <a name="arnold-ode"></a> V. I. Arnol'd, *Ordinary differential equations*

This book set the standard for the theory-centered or dynamical-systems-centered point of view
described above. This is first and foremost a book about the flows of vector fields. Even in the
case of first-order linear systems with constant coefficients, primary emphasis is given not to
computational techniques of solution but on what linear algebra can tell you about the structural
properties of the system's flow. Nevertheless there is substantial material on how to reduce a
differential equation to linear form and solve it, although no Laplace transform techniques or the
like. Arnold explains it all coherently at an advanced-calculus level (manifolds appear at the
end), complete with many beautiful diagrams.

Like many Russian books, this one can feel discursive and unsystematic to readers accustomed to
the section-exercises-section-exercises flow of standard American texts. It's worth getting used
to it, because Arnol'd is a master expositor.

#### <a name="birkhoff-rota-ode"></a> Garrett Birkhoff & Gian-Carlo Rota, *Ordinary differential equations*

Think of this book as the Apostol of differential equations: a concise, rigorous first course in
the traditional material, without all the blather of standard texts. It's used for 18.034, the
honors first course at MIT. Laplace transforms are not discussed, but several of the classical
special functions appear throughout, and the book ends with a discussion of orthogonal
polynomials.

I have heard, though I do not know from my own experience, that this book is notoriously full of
errors, particularly in the exercises. Independent students should be accordingly wary.

#### <a name="ross-diffeq"></a> Shepley Ross, *Differential equations*

If you're looking for more exposition about the methods of solution of differential equations than
you can find in Birkhoff & Rota, you could do much worse than this older (1984) standard
text. Yes, it's fat, but mostly quite clear.

