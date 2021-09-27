## Project Milestone 2

Version History: 

- Released, 2021-09-26


Due Thursday October 7, 11:59PM

In this milestone we are:

- Reporting on our progress with the project
- Creating artifacts of our progress on the project, e.g., task abstractions,
  design sketches, interview data, code, writing
- Assessing changes made since our first milestone
- Correcting deficiencies in our proposal
- Demonstrating we can adapt an existing LaTeX document to new specifications

Create a repository for this milestone at this following Github Classroom
link: [https://classroom.github.com/g/7rdOUkr8](https://classroom.github.com/g/7rdOUkr8).

All material you want graded should be in that folder at the deadline. All the
files needed to compile your document should be in that folder. **NO
Auxilliary files should be in that folder. Do not include PM2.pdf, PM2.aux,
etc.** 

Continue to use the LaTeX files required to format an IEEE VGTC-style
document. However, this time I am not providing the rest of the files. You
will likely want to copy `proposal.tex` from last milestone and adapt it to
the requirements below.

There should be a `PM2.tex` file that compiles into a `PM2.pdf` file when I
type `make`. Thus, you will also need to modify the `Makefile` you turn in.

Create a folder named `Project` in your repository. This folder should include
code and any other files required to eventually run your project. It may also
include data for data-collection-centric projects.

Your PM2 report should include several sections described below. Also, see my
comments in Project Milestone 1 for any additional information I expect to see
in this milestone.

#### Abstract (5 pts)

Briefly describe your project and contributions you have made for this
miletsone.


#### Section: Overview (5 pts)

Create a top level section called `Overview`. In this section, describe the
overall goal of your project -- what overarching problem is it trying to help
solve (not necessarily a visualization problem) and then what is the
visualization aspect of that problem that your project entails. This will be
like your first section in the first milestone, but shortened. It should be a
reminder to the readers what your project is about to frame what it being
contributed this milestone.

Then, summarize what work was completed for this milestone. 


#### Section: Related Work (10 pts)

Create a top level section called `Related Work`. Cite and describe existing
work related to your project, including but not limited to academic papers and
existing software (both open and closed source).

There are several ways in which work can be related beyond existing work that
is exactly what you propose to do. Consider other research that tries to solve
the overall question motivating your work but in a different way. Consider
visualizations that try to solve a similar problem to yours. You may want to
look in the citations of the existing work you already cited and/or papers
that cite them.

#### Section: Technical Progress (60 pts)

Create a top level section called `Technical Progress`. In this section,
describe what progress has been made. Such progress may include (1)
understanding any systems with which you will use or integrate, (2) coding in
service of the goals of your project (e.g., data reader, views, etc), (3)
proof of concepts, and (4) data collection and analysis.

Please note the *required subsections* for specific types of problems below.
If something is covered by a required subsection, you do not need to repeat it
elsewhere. You are free to create your own subsections in addition to the
required ones and/or write ones not required by your type of project.

If the progress includes a better understanding of how the systems work, use
this section to describe that understanding for others. For example, if your
project requires understanding multiple modules interact, describe how those
modules interact here, as if you were writing up that knowledge for a final
paper.

Proof-of-concepts may include code that will not be part of your final
project, but demonstrate that some technical piece of your project will work.
For example, if you plan to rely on a third party library, it could be a short
script demonstrating that library works. 

If there is code associated with the contribution, including proof of
concepts, it should be available in the repository under a folder named
`Project`. It need not run at this milestone. Please describe its status. 

If you collected data for this milestone and it is not discussed in another
subsection, please describe your data collection efforts in their own
subsection. What did you do to collect the data? Is there still more that you
have to do? What are the results of your collection efforts? 


#### Subsection: Methodology (Required for Literature Surveys)

Describe in detail your methodology for finding papers for your literature
survey, including intial search criteria, limitation criteria, and stopping
criteria. State how many papers have been collected. Inside the `Project`
directory should be a data file listing all the papers in your collection.


#### Subsection: Task and Data Abstraction (Required for Visualization Design Projects)

Create a top level section called `Task and Data Abstraction`. In this
section, describe your data both in terms of format and data types as we
discussed in class. If you have already done this in the proposal, you may
copy and refine it from the proposal. If your project is extending from an
existing task and data abstraction, summarize those abstractions and cite
them.

Describe your task abstraction in a subsection here. You must describe how you
gathered data to support your task abstraction (e.g., interviews, literature).
Then you must describe your tasks in terms of one or more task taxonomies (you
must cite which one). For each visualization task you identify, describe how
it related to the domain and to the data. Note the PAVED paper read in HA2 has
an example of such a description.

If you are using a hierarchical task taxonomy, all applicable levels of the
hierarchy should be explained.


#### Section: System Design (Required for System/Library Projects)

Create a top level section called `System Design`. In this section,
describe the design and architecture of your system. If it alters a
pre-existing system, describe the architecture of that system and where your
changes and workflow fit in. Creating a flow chart may be helpful in
communicating your design. Discuss the rationale behind your design,
including technical concerns.

Discuss your initial API design if writing a library.


#### Section: Preliminary Designs (Required for Visualization Design Projects)

Create a top level section called `Preliminary Designs`. In this section,
describe at least three different design approaches. Each design should be in
its own subsection. Include sketches or other mock up figures to help describe
the design. For each design, include a *rationale* for why this design is
appropriate. A good rationale will appeal to multiple sources of support
including design principles and best practices, existing work, support from
the task abstraction, and feedback from users. 

The designs should be reasonable in detail to solve your problem. For example,
if you need to support multiple tasks, you may have multiple views in each
design. 

Include a final subsection called `Chosen Design`. In this section, describe
which of the preliminary designs you intend to implement and why you think
this design is better than the others. 


#### Section: Preliminary Study Design (Required for Evaluation Study Projects)

Create a top level section called `Preliminary Study Design`. In this section,
describe the initial design of your experiment. Clearly state the research
question you are trying to answer, the conditions, variables and factors, and
plans for tasks and analysis. Describe the study population and plans for
recruitment. Include a *rationale* for your choices, explaining why they were
chosen. A strong rationale can appeal to other studies but may not always be
possible.


#### Section: Refinement from Previous Milestone (10 pts)

Create a top level section called `Refinement from Previous Milestones`. If
you were told to refine any subsection of the previous milestone, included the
refined version of that section as a subsection here. If you were not told to
refine any section, simply write `None requested.`

These requests will be made through D2L by Monday September 27th. Common
requests will be refining the evaluation or background subsections.


#### Section: Schedule (10 pts)

Create a top level section called `Schedule`. In this section, describe what
parts of your proposed milestone two goals have been met. Then describe which
goals were not met and an explanation of what choices or unexpected challenges
led them not to be met.

Describe what work will be done for the next three milestones, in light of
what was done for this milestone. 



