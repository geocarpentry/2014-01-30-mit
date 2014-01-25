% Software Carpentry - Overview
  ERDC 
% Software Carpentry Team
% January 2014

## Copy This Lecture!
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<br></br>
<a rel="license" href="http://creativecommons.org/licenses/by/3.0/deed.en_US"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/InteractiveResource" property="dct:title" rel="dct:type">Software Carpentry Overview</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="http://software-carpentry.net" property="cc:attributionName" rel="cc:attributionURL">Software Carpentry</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/3.0/deed.en_US">Creative Commons Attribution 3.0 Unported License</a>.

# More About Software Carpentry

## History

* Founded by Greg Wilson in 1998, teaching scientists how to use supercomputers at LANL.
* Open sourced materials 2004-present
* Currently funded by the Sloan Foundation and the Mozilla Foundation

## What We Teach

* Unix Command Line Interface (Shell)
* Shell automation 
* Version Control
* Python
* Testing
* Some nice python modules (numpy, pandas) 

## What We *Actually* Teach

* A program is just another piece of lab equipment
* Programming is a human activity
* Little pieces loosely joined
* Let the computer repeat it
* Paranoia makes us productive
* Better algorithms beat better hardware

*How to THINK like a programmer*

## Who We Teach

<div align="center">
<table>
<tr>
<td><img src="swc-demographics/thumb-age.png" /></td>
<td><img src="swc-demographics/thumb-role.png" /></td>
</tr>
<tr>
<td><img src="swc-demographics/thumb-gender.png" /></td>
<td><img src="swc-demographics/thumb-platform.png" /></td>
</tr>
</table>
</div>

## Who We Are

* Aron Ahmadia (ERDC)
* Chris Kees (ERDC)
* Matthew Farthing (ERDC)
* Randal Olson (MSU)
 
## Our Goals for You

### We will take you on a tour of:

* Managing and sharing Software, Data, and Manuscripts with **Git**
* Automating things with the **shell**
* Practical Programming with **Python**
* Scientific Computing with Python (numpy, matplotlib)
* Data munging / parsing with python

# Some High-Level Advice

## Be fluent in multiple languages
<comment>
You speak multiple languages when interacting with a computer.
Choosing to use a new tool, library, or language can be similar to
learning a new language:
</comment>


+ There is a high initial startup cost as you learn vocabulary, grammar, and
idioms
<font color=blue>`sum(x*y for x,y in itertools.izip(x_vector, y_vector))`
</font color>
+ But once you have gained some fluency, you will find yourself capable of
new things!
+ You will learn faster by observing and working with others who are more
skilled than you
+ Aim for languages and tools that allow you to express your models and
manage your data simply. 

## Make it work right first, make it fast later.
* "Premature optimization is the root of all evil." -- Donald Knuth
* Directing your attention to making it use less disk / less memory /
less time from the start is wrongly directed attention.

## Increase debugging bandwidth

* **REPL (read-eval-print-loop)** environments tighten the coupling between
the code you write and the results you see, increasing productivity.
* Development environments and debuggers give you more information at once 
* Test your procedures on subsets of your data **so that you learn whether
it works faster**

# Don't Repeat Yourself (or Others)

## Automate common actions by saving simple blocks of code into **scripts**

* A script is a set of commands organized into a single file
* The script is the basest unit of scientific programming, you should be
comfortable writing these whenever you want to save or otherwise document or
repeat your actions
* Use scripts to explore new ideas, they are easy to write and throw away
* **Don't repeat commands into your REPL, save them to a script**

## Refactor commonly used blocks of code into **functions**

* Eventually, you will find that your scripts have a lot of repeated code,
or that you are spending a lot of time adjusting parameters at the top of
the file
* Refactor out repeated code into **function calls** in your scripts and
implement the **function** either in the same file or a separate one
* Be comfortable with the calling and return syntax of your programming language
environment, whether it is bash or Python
* **Don't repeat code in scripts, refactor them to functions**

## Group commonly used functions into **libraries**

* If you have to write a lot of software functions,
consider designing and releasing a library so that
others do not have to share your misfortune
* Check that nobody else has implemented the functionality you need
* If something close exists, it may be worth adapting to your needs if the
project is of high quality and suitably licensed
* *Openly licensed non-commercial libraries tend to have a much longer effective
lifespan than unreleased codes*
* **Share your code with others, and use their code**

# Reduce Complexity

## Basic strategies

* Use languages and libraries that reduce the complexity of
your work
* It is worth installing a complicated or expensive software tool if your
computations or model are naturally expressed with it
* Always look for opportunities to write **less** code
    + you will have to do less initial work (sometimes)
    + you will introduce less bugs
    + your code will be easier to understand and maintain
* Keep individual functions short, single-purpose, possible
 to be confident in festooning.

## Back up your data!

## Use version control for checkpointing and collaboration

* use local version control software to checkpoint personal code development
  + checkpointing your work encourages wild ideas and late-night coding sessions
  + you can easily restore back in the morning if it was a bad idea
* use **distributed version control** to collaborate with others
* We advocate *Git*, but you may be stuck with whatever your group uses


# Verify and Validate your Code

## Principles of verification and validation
* **verification** - is your code correctly written?
* Be paranoid.
  + test small things!  
  + test that what you assume is TRUE is in fact so.
* test frameworks can help you verify your code
* **validation** - do your computations accurately model the phenomena in question?
  + not a good candidate for automation.  (Not sad at all)

## Document your computational work
* Save every bit of code you use for generating publishable results
* Document and comment your code for yourself as if you will need to understand
it in 6 months
  + use README files liberally
  + as well as file-level, function-level, and inline documentation
* If any piece of code is too complex to easily describe, consider refactoring
it

## Schedule 
* Today 
* **9:00-12:00** Shell / python 
* **1:00-4:30**  Python 
* Tomorrow
* **9:00-12:00** Version control with Git 
* **1:00-4:30**  Application Vignettes

# Closing Thoughts

## You sometimes need geeks.  You never need dorks.
<div align="center">
<table>
<tr>
<td><img src="swc-demographics/careful.png" /></td>
</tr>
</table>
</div>

# References and Further Reading

# Research Literature

## Programming Languages for Scientific Computing
Matthew G. Knepley

Preprint: http://arxiv.org/pdf/1209.1711.pdf

*Gives an overview of modern programming languages and techniques such as code
generation, templates, and mixed-language designs. This is a preprint,
so expect some rough spots.*

## Two Solitudes
Greg Wilson

Slides: http://www.slideshare.net/gvwilson/two-solitudes

*Describes Greg's journey as a scientist and leader for the Software Carpentry
project, provides some insight into the differences between industry and
academics.*

## Best Practices for Scientific Computing
D. A. Aruliah, C. Titus Brown, Neil P. Chue Hong, Matt Davis, Richard T. Guy,
Steven H. D. Haddock, Katy Huff, Ian Mitchell, Mark Plumbley, Ben Waugh,
Ethan P. White, Greg Wilson, Paul Wilson

Preprint: http://arxiv.org/abs/1210.0530

*Good summary paper of many fundamental practices for working with and
developing scientific software. This is a preprint, so expect some rough spots.*

# Web References

## What Every Computer Scientist Should Know About Floating-Point Arithmetic
David Golberg

Web article: http://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html

*Introduction to the IEEE floating-point standard, its implications, and many of
the common pitfalls when using floating-point numbers in scientific computing*

## Science Code Manifesto

http://sciencecodemanifesto.org

*Publicly signed commitment to clear licensing and curation of software
associated with research publications.*

