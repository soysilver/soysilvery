---
layout: post
title: NMR Two Level GNN (2024)
description: Nuclear Magnetic Resonance Spectroscopy Signal Prediction with Two Level GNNs 
image: /assets/images/preparing.png
---


Nuclear Magnetic Resonance Spectroscopy Signal Prediction with Two Level GNNs 
============


 Nuclear magnetic resonance (NMR) is the primary method used to estimate the properties of unknown molecules, and NMR machines are now one of the most commonly used instruments in organic chemistry laboratories. NMR spectroscopy takes advantage of the fact that the nuclear magnetic moment of each atom, which is the specific frequency of electromagnetic waves that it absorbs and emits when exposed to an external magnetic field, varies slightly depending on the environment around the atom. This information can then be used to reconstruct the environment around the atom, ultimately revealing the molecule of interest. 
 NMR is divided into 1H NMR and 13C NMR depending on the type of target atom that is the center of the reconstruction. 1H NMR uses the chemical mobility of a hydrogen nucleus, or one lone proton, to determine the number of hydrogen atoms in a molecule, how they are bonded, and their ionization state. It is a common method for determining the structure of organic matter because the major atoms in organic compounds, such as carbon and oxygen, bond with the most common and lightest form of 1H hydrogen to form an octet of electrons. 13C NMR analyzes the chemical shifts of the carbon nucleus, which is composed of six protons and seven neutrons. Since the definition of an organic compound is a compound with a carbon atom as its backbone, 13C NMR is often used to determine the structure of complex molecules. 1H NMR has the advantage of high sensitivity and relatively quick results with a small sample volume. In contrast, 13C NMR is less sensitive and requires a large amount of sample, but it is relatively stable and accurate.

Paragraphs are separated by a blank line.

!2nd paragraph. *Italic*, **bold**, and `monospace`. Itemized lists
look like:

  * this one
  * that one
  * the other one

Note that the actual text
content starts at 4-columns in.

> Block quotes are
> written like so.
>
> They can span multiple paragraphs,
> if you like.


H2 Header
------------

Here's a numbered list:

 1. first item
 2. second item
 3. third item

Note again how the actual text starts at 4 columns in (4 characters
from the left side). Here's a code sample:

    # Let me re-iterate ...
    for i in 1 .. 10 { do-something(i) }

As you probably guessed, indented 4 spaces. By the way, instead of
indenting the block, you can use delimited blocks, if you like:

~~~
define foobar() {
    print "Welcome to flavor country!";
}
~~~

(which makes copying & pasting easier). You can optionally mark the
delimited block for Pandoc to syntax highlight it by specifying the languagae after the start of a block (e.g. `~~~python`) which would look like :

~~~python
import time
# Quick, count to ten!
for i in range(10):
    # (but not *too* quick)
    time.sleep(0.5)
    print(i)
~~~

### An H3 header ###

Now a nested list:

 1. First, get these ingredients:

      * carrots
      * celery
      * lentils

 2. Boil some water.

 3. Dump everything in the pot and follow
    this algorithm:

        find wooden spoon
        uncover pot
        stir
        cover pot
        balance wooden spoon precariously on pot handle
        wait 10 minutes
        goto first step (or shut off burner when done)

    Do not bump wooden spoon or it will fall.

Notice again how text always lines up on 4-space indents (including
that last line which continues item 3 above).

Here's a footnote [^1].

[^1]: Some footnote text.

Tables can look like this:

| Header 1 | Header 2                   | Header 3 |
|:--------:|:--------------------------:|:--------:|
| data1a   | Data is longer than header | 1        |
| d1b      | add a cell                 |          |
| lorem    | ipsum                      | 3        |
|          | empty outside cells        |          |
| skip     |                            | 5        |
| six      | Morbi purus                | 6        |


A horizontal rule follows.

***

Here's a definition list:

apples
  : Good for making applesauce.

oranges
  : Citrus!

tomatoes
  : There's no "e" in tomatoe.

Again, text is indented 4 spaces. (Put a blank line between each
term and  its definition to spread things out more.)

Here's a "line block" (note how whitespace is honored):

| Line one
|   Line too
| Line tree

and images can be specified like so:

![example image](https://images.unsplash.com/photo-1488190211105-8b0e65b80b4e?w=300&h=300&fit=crop "An exemplary image")

Inline math equation: $\omega = d\phi / dt$. Display
math should get its own line like so:

$$I = \int \rho R^{2} dV$$
