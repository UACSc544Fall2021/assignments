## Homework Assignment 3

Version History: 

- Released, 2021-09-19


Due Thursday September 30, 11:59PM

In this assignment we are:

- Gaining familiarity reading and interpreting a user study
- Reviewing material from lecture and practicing short answer questions
- Gaining more practice using the d3js library for visualization

The artifacts generated should be presented in the HTML pages or LaTeX
documents as described below. No style information should be in the HTML tags
unless explicitly allowed. Do not use HTML tags like `<center>`, `<b>`, or
`<i>` to alter visual appearance.  Programmatically added SVG elements may
have style attributes.

Github Classroom Assignment link: [https://classroom.github.com/a/krAs-gP7](https://classroom.github.com/a/krAs-gP7).

Anything you want graded should be in the repository at the due date in the
`master` (default) branch. Do not forget to `git commit` and `git push` to
`github.com`. You may want to verify through the web client or cloning to
another place to ensure your commits have been made.


### Paper Reading (20 pts)

Read the paper "Evaluating the Impact of Binning 2D Scalar Fields" by Lace
Padilla, P. Samuel Quinan, Miriah Meyer, and Sarah H. Creem-Regehr. Answer the
following questions. These are the same questions from your previous paper
reading assignment, with the exception of the final one which has been updated
as the PM1 deadline will have passed..

1. What problem is this paper trying to solve?

2. Why is this problem considered a visualization problem?

3. Why is the problem important?

4. How does this paper contribute to solving the problem? 

5. What approaches are used to construct the contributions?

6. How are the contributions of the paper evaluated, justified, or evaluated? 

7. What do you think are this paper's strengths? 

8. What do you think could be improved about this paper?

9. What future directions do the authors suggest? 

10. What future directions not mentioned in the paper would you suggest?

11. What questions do you have about this paper? For example: Were these things
   you find difficult to understand? Are there details left unanswered? Do you
have philosophical questions regarding some of the points made?

12. How might the concepts or approaches in this paper relate to your course
   project? 

Note: These questions have been adapted from similar guides and assignments by
William G.  Griswold, Premkumar Devanbu, and Michelle Strout.

The results should be submitted as a LaTeX `.tex` file that will compile into
a `.pdf` with the command `pdflatex`. Use the template from the previous
assignment. The name of the `.tex` file should be `reading.tex.`

This portion will be graded on whether you have answered all the questions,
including sub-questions, the thoughtfulness of your answers, and the
readability of your answers.

### Short Answer (16 pts)

Answer the following questions:

1. Explain why it is considered bad practice to encode one attribute with
   mark-height and a second attribute with mark-width. (2 pts) 

2. In the PAVED paper in HA2, what sections correspond to the Discover phase
   in terms of the Design Study Methodology framing? (2 pts)

3. Of the six criteria for rigor in design studies proposed by Meyer and
   Dykes, which one do you think is the most important and why? This answer
will be assessed on selecting one of the six criteria (1 pt), demonstrating
you understand its meaning (1 pt), and the depth reasoning in explaining why
it is the most important (2 pts). 

4. Suppose you want guidance regarding possible bias effects that color choice
   has on bars in a bar choice. You design an experiment to help provide this
guidance. What are you independent and dependent variables and why? (4 pts)

5. In terms of van Wijk's economic model for the value of visualization, are
   experiments to understand bar chart design valuable? If so, how? If not,
why not? (4 pts) This answer will be assessed on the strength of the
justification of your answer and how well it ties into the model.


The results should be submitted as a LaTeX `.tex` file that will compile into
a `.pdf` with the command `pdflatex`. You may want to follow the template from
your paper reading. The name of the `.tex` file should be `short.tex`.

This portion will be graded on whether you have answered all the questions,
the thoughtfulness and correctness of your answers, and the readability of
your answers including whether they are still "short answers". If you were
given these questions on an exam, I would give you half a page of space to
write your answers by hand.

If I ask for X of something in a problem, I will grade only the first X
listed if you list more than X.


### Visualization with d3js (64 pts as divided below) 

Add to the scatter visualization and UI from HA2 as shown in the movie linked
here: [HA3/images/HA3.mov](HA3/images/HA3.mov)

A still shot fo the entire framework is further down.

You are expected to start from the HA2 files you already have but rename them
to `HA3.html`, `HA3.css`, and `HA3.js` respectively. You will likely edit the
HTML, CSS, and JS. You may ask to see/discuss HA2 code from others in the
class, but you must clearly comment if you are using someone else's HA2.

Use the d3js **version 7** library **and no other** for everything involving
SVGs. **You will need to update this in your HTML file from HA2.** 

For any scaling you must do, you should use the d3js scale functions (e.g.,
`d3.scaleLinear()`).

Do not use other libraries with the exception that you may use a library to
implement MVC or any other design pattern for managing multiple views
*provided it does not require anything but loading the page in a browser to
run.* I **will not** launch a server, `npm install` anything, run Node, or
similar to grade this assignment. You should only use the calls in that library
to implement the UI architecture, not other functionality.

Remove everything related to the bar chart from HA2. 

This assignment adds/changes the following:

- The color dropdown is now limited to the `Genre`, `Platform`, and `Rating`
  fields. The default is `Platform`.

- The color of the dots is now categorical, using d3's `Accent` color scheme.

  - Make a legend for the colors so viewers can match the color to the value. 
    The video has one example, but you are free to do this as you choose.

- All dots have a black border. The default has a 1 pixel width, the hovered
  has a 3 pixel width. This updates as soon as the mouse enters or leaves (no
transition time).

- There are two new dropdowns, `a` and `b`:
 
  - Note the `a` and `b`labels are on the same line as the dropdown

  - Above each is a 100 by 300 pixel SVG. 

  - Within the SVG is a histogram. It has 25 pixels to the left and right
    (some of which is taken by the scale), 5 pixels on top, and 20 pixels on
the bottom (most of which is taken by the scale. The color of the bars is up
to you but must be visible through the brush.

  - The histogram bars and axes update when the dropdown changes over 750ms.
    New bars grown from the bottom axis. Exiting bars shrink down into the
bottom axis.

  - The histogram is calculated with
    [d3-bin](https://observablehq.com/@d3/d3-bin). There is a good example of
it in use [here](https://observablehq.com/@d3/histogram). Note you are not
expected such attention to the tick marks as in this example. You must still
cite this example in the comments if you use it.
    
    - *Extra Credit* (5 points) Without changing the font size, improve the axes
    so the tick labels don't run into each other even when the drop down is
changed. There should still be more than two tick marks.

  - The default for `a` and `b` is the same as `x` and `y`.

  - There is a [d3-brush](https://github.com/d3/d3-brush) over each histogram.
    The default spans the whole histogram.

  - Items selected by BOTH brushes (from both histograms) have radius 5 and
    opacity 1 (both the fill and stroke). Items not selected by BOTH (even if
selected by 1) have radius 3 and opacity 0.5. These update as soon as the
brush is moved (no transition time). As nice example of a d3-brush is
[here](https://observablehq.com/@d3/focus-context?collection=@d3/d3-brush).
You must still cite this example in the comments if you use it.


![](HA3/images/CSC544-HA3.png)


*More Extra Credit (10 pts)*: Implement panning and zooming in the scatter
plot. All the other functionality should still work. Dot centers should not be
drawn completely outside the 50 pxiel margins set within the scatterplot SVG.
There should be a button to reset to the original view. Changing an axis
should reset that axis' pan/zoom.  




##### Grading

Here is a breakdown of grading by functionality. Partially credit may be
assigned for partial completion.

- Color dropdown and functionality has been changed to for categorical color:
  10 pts
- Legend for categorical colors: 6 pts
- `a` and `b` Histogram drawing and funtionality:
  - histograms calculated with d3-bin and rectangles drawn: 10 pts
  - histogram axes are drawn and and animate when changed: 5 pts
  - histogram bars animate when changde: 5 pts
  - brush and brush functionality (changes in scatter plot): 20 pts
- Functionality from HA2 is preserved unless otherwise noted and bar
  chart-related code is removed: 10 pts

