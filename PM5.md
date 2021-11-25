## Project Milestone 5

Version History: 

- Released, 2021-11-24

Due TUESDAY December 7, 11:59PM

In this milestone we are:

- Performing initial evaluations of our projects when applicable and/or
  writing our final analyses of our literature surveys.
- Creating artifacts regarding our evaluations and analyses.
- Reflecting on our projects
- Getting more practice with LaTeX


Create a repository for this milestone at this following Github Classroom
link:
[https://classroom.github.com/a/W89CWGzu](https://classroom.github.com/a/W89CWGzu)

All material you want graded should be in that repository. All the files
needed to compile your document, a no more than those files, should be in that
repository. The `PM5.tex` file should be in the root of the repository. **NO
Auxiliary files should be in that folder. Do not include PM5.pdf, PM5.aux,
etc.** 

Continue to use the LaTeX files required to format an IEEE VGTC-style
document. As in the previous milestones, I am not providing the rest of the
files. You will likely want to copy files from you last milestone and adapt it
to the requirements below.

There should be a `PM5.tex` file that compiles into a `PM5.pdf` file when I
type `make`. Include the updated Makefile. Additionally, there should be a
short movie demonstrating your functioning prototype.

Include files regarding any study/evaluation you have done in a directory
called `Evaluation`. It should include the materials you used for evaluation
(e.g., datasets, scripts (both coding scripts and human scripts), and raw data
collected during evaluation).

If you made significant changes to your project, please include them in a
`Project` directory. If related code has not changed significantly since PM4,
you do not need to include the directory.

## Report

Your PM5 report should include several sections:

### Abstract (5 pts)

Briefly describe your project and contributions you have made for this
milestone.

### Section: Overview (5 pts)

Create a top level section called `Overview`. In this section, describe the
overall goal of your project -- what overarching problem is it trying to help
solve (not necessarily a visualization problem) and then what is the
visualization aspect of that problem that your project entails.

Then, summarize what work was completed for this milestone. 

### Section: Refinements to {Your Project Type}

**This section is for Visualization Design, System Design, and User Study
Projects.**

Create a section called `Refinements to {Your Project Type}` where `{Your
Project Type}` is either `Visualization Design`, `System Design` or `User
Study`. If you continued to refine these pieces of this project past PM4,
describe how you have done so in this section. If you made these changes
before the evaluation, put this section before the `Evaluation` section. If
you made them after, put them after. If you did both, create two sections, one
with the title `Refinements to {Your Project Type} before Evaluation` and one
with `after Evaluation`.

If you have not, create the section and write `Not Applicable`.  Note: if your
system is too buggy for your evaluation, then your evaluation results may not
be valid.

##### Movie

If there are changes beyond minor bug fixes, please create a movie like you
did for PM4 showing these changes. 

The video should include some description of what is going on. This can be
done in a separate text file (`.tex`, `.txt`, or `.md`) or can be done through
voice over. If a file is used, please name it `pm4-movie`. If no such file is
found, audio will be assumed.

**There are several ways to share your movie. Github may not be the best way
due to file size issues. You can create an unlinked video on Youtube. You can
also use Google Drive for sharing. If the latter, please share with my kisaacs
account at `cs.arizona.edu` as that's the one associated with Google. I cannot
read from an `email.arizona.edu` share.**

If the changes are minor such that you do not need a movie, write in this
section that they are and thus you have not created a movie.


### Section: Evaluations 

**This section is for Visualization Design, System Design, and User Study
Projects.**

**If you are not conducting an evaluation, it must be approved by the
instructor first and similar work must be present in the technical progress
section. Furthermore, you must still include this section noting the
evaluation was not conducted and write the Future Evaluation subsection
described below.**

Create a top level section called `Evaluation`. For each form of evaluation
you have, create a subsection. In those subsections, create a subsubsection to
describe the design of your evaluation and your rationale for that design.
Create another subsubsection to describe the results of the evaluation. For
qualitative evaluations, I expect a summary of observations and/or responses.

The raw data from your evaluations should be available in the `Evaluation`
directory. In that directory, include a `README.md` that explains what each
file in the `Evaluation` directory is, such as a script for an evaluation
session, a list of interview questions, or responses from a single individual.
Please anonymize the names of individual participants but basic demographic
information about them and their familiarity with your project domain should
be described.

Create two subsections, `Results` and `Discussion`. The Results section should
as factually as possible describe the results of the evaluation. The
Discussion section considers the meaning of those results and what they
indicate regarding your project.

Create a subsection called `Limitations and Threats to Validity` where you
discuss the limitations and threats to validity of your evaluation approach,
what other forms of evaluation you could *feasibly* conduct to mitigate those
limitations and threats, and what these limitations and threats mean for your conclusions.

Create a subsection called `Future Evaluation` where you discuss how you would
evaluate this project if you had more time and resources. The proposed
evaluation should be **feasible**. For example, it's possible you may recruit
several rocket scientists for a half hour study but you probably cannot
recruit 100s of rocket scientists for a 2 hour study. 

### Sections for Literature Surveys

**These Sections are for Literature Surveys only.**

If you are doing a literature survey, write up your results as you would a
survey paper. You are given flexibility in how many sections you want to use
and how you want to organize them. I suggest looking at existing literature
surveys for ideas.

You are not required to re-write the methodology section. You may choose to
re-write it (or copy it from the previous milestones and refine it) if it has
changed. The same is true for the related work sections. 

I expect the literature survey sections will include a categorization or
taxonomy of the papers considered with figures or tables to describe the
categorization as well as metrics describing the reviewed papers (e.g., how
many per major category). Then, each category will be described with the
relevant work therein summarized. Where helpful, include (cited) figures from
the reviewed work. 

There should also be a section that describes open challenges and
opportunities in the area of your literature survey.


### Section: Lessons Learned (20 pts)

In this section, reflecting upon your project milestones, discuss what lessons
were learned that could possibly be transferred to other visualization
problems and contexts.

These lessons do not need to be novel. You can confirm or refute existing
visualization knowledge in this discussion.


### Section: Project Summary (5 pts)

In this section, summarize your project as a whole, discussing what you did
during the course of this project and what contributions were presented in
this milestone and the ones before it. 

