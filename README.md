# The Maven Review

Here we propose an updated methodology of a 2-tiered collaborative review process of scientific analyses for large collaborations, such as LHCb. The proposal is based on the [current model used by LHCb](http://lhcb.web.cern.ch/lhcb/lhcb_page/collaboration/organization/editorial_board/Publication_Procedure-Sept2011.pdf) and aims at improving in several points.

## Executive Summary
In order to improve 

* the time when feedback is made available to an analysis team;
* the structure of feedback;
* the transparency of the decision making process when an analysis is ready for approval;
* the reproducibilty and sustainability of the analysis and in particular the tools developed for it;

we propose to establish the following roles and methods in the review process:

* Switch from a two-stage to a two-tier review model.
* Tier 1: Each analysis is from day one accompanied by a working group reviewer, here called **'maven reviewer'**.
* For each analysis there is a prioritized **backlog**, maintained by the maven reviewer.
* The complete analysis code of each analysis is made available and included in the deliverables of the analysis as **reviewed code**.
* Tier 2: Collaboration reviewers are appointed as soon as possible and start to provide feedback on the backlog as well as on components that have been approved by the maven reviewer already.
* The backlog is used for **triage** to decide when an analysis is mature enough to be released, including the transparent decision to leave some questions open.

In the following the reasoning behind these new structures and how they will help improve the flow of feedback during an analysis project is explained in detail.

## The Aim of the Proposal
We try to adress three issues that are recurring problems within the current review process:

1. Feedback on the strategy and technique of the analysis has to be made available to the analysts as early as possible. Few things are as wasteful and frustrating as when someone works for quite some time on a project but gets feedback that requires substantial changes only once the analysis is finished and thought to be ready to be published. 
2. Currently the only basis for a review is the analysis note. The actual tools to obtain the results are largely absent from the discussion. This makes it very hard to ensure the reproducibility of the result and the sustainability and relevance of the work invested for future projects. 
3. To make best use of the limited available resources, feedback has to be well structured. In most cases it is straight forward to request a large number of cross checks and systematic studies. It is less obvious how the available time is spent most usfully. There are two issues connected to this: the ability of the reviewers to ask the right questions, based on the material presented to them; and the priorisation of tasks, possibly requiring triage if the collaboration wants to hit a particular deadline.

The proposal presented here adresses all of these issues while preserving the essential and valuable features of the present review process, in particular the requirement that an analysis is reviewed by independent minds.

### Balancing an unbiased review with the need for early feedback
The main goal of the proposal is to bring feedback to the analysis at an early stage. To explain this a bit more in depth we note the following dynamics in the current review process.

Analysts understand that the collaboration reviewers have the last word on whether a result is ready for release. In principle they can hold off the analysis as long as they believe necessary. In the current process this typically leads to one of two reactions. Both reactions are driven by the completely understandable desire of working groups and analysis teams to get results released as smoothly as possible. 

The first response is to have a rather loose working group review and try to get collaboration reviewers assigned as early as possible, knowing that it only makes sense to start working in earnest on the finalisation when the reviewers are on board. This places a considerable workload on the reviewers. It is, however, less problematic than the second response: In this case the working group uses the working-group-approval as a shield to limit the extent to which the reviewers are allowed to critique the analysis. The argument put forward is, that because a certain method was approved by the working group the review can only happen within the limits of this method. This stance is understandable if a lot of work has already been invested to implement the analysis up to that point. However, it is unacceptable scientific practice if reasonable concerns are brought up in the review process.

To resolve the issue it is important to understand that the conflict is most probably not a disagreement of what is to be considered a "reasonable concern". Conflicts and waste of time results when these concerns are discovered too late in the process. 

## Two Tiers
The two tiers proposed here are organised on the working group level (tier 1) and on the collaboration level (tier  2). However, contrary to the current model they are not stricitly staged in time, as will be discussed below.

Tier number one is the working group review. The goal of this part of the review is to ensure that the analysis is technically and from its physical content of the highest quality permitted by the limits of person power and computing resources. Feedback from relevant experts in the working group (and if needed beyond) is brought to the analysis team at the earliest possible state. The goal is to highlight problems in an early stage to avoid waste of work or sidetracks. A crucial responsibility of tier one is to ensure that the analysis is reproducible and the tools developed are in a state that allows future projects to profit from the invested work. 

Tier number two is the collaboration review. The responibility of this second tier is to provide an external, unbiased perspective on the analysis. The methodology is critically examined. The documentation is checked for completeness and clearness.

The basic idea to use a tiered versus a staged review process is that the review can proceed in parallel to the analysis. Components of the analysis are made public as soon as they are implemented. The reviewers, first on the working group level, then on tier 2, give their feedback on the component immediately. They do not wait until a full analysis note is ready. To organise this process we propose a few simple tools.

## A Few Simple Tools
To attack the problems stated above and to organise the triered review we propose to adopt the following tools as part of the review process:

### Maven Reviewers
On the working group level, **as soon as an analysis is proposed**, a working group reviewer is assigned. They should be experienced in the respective kind of analysis and take the role of a 'maven reviewer' [1]. A maven reviewer accompanies and counsels the analysts during the whole analysis. Their first responsibility is to help the analysis team achieve the highest possible physics goals in the limitations of the available resources. Their second responsibility is to make sure that the analysis is carried out according to adequat technical standards by making detailed feedback available as early as possible. The main tools that helps them achieve this are the **analysis backlog** and the **code review** discussed below.
A maven reviewer does not engage in the day-to-day business of implementing the analyis but is available for questions and clarifications. They meet regularly (biweekly) with the analysis team, outside of the working group meetings, to discuss the progress of the analysis.

Due to the intense involvement such an interpretation of the role of working group reviewer is in conflict with the requirement to have the analysis checked by independent minds. This is the role of the tier 2 reviewers.

Tier 2 reviewers are assigned shortly after the first prototype of the analysis is under review by the maven. At this stage usually a first presentation about the analysis has been given in the working group. The maven, in discussion with the analysis team and the working group has already setup a substantial backlog (see below) that describes the analysis strategy.

By making the backlog (and all other analysis artifacts) immediately available to the tier 2 reviewers, the maven provides the opportunity to collect early feedback on the analysis. More on the interaction between the maven reviewer (tier 1) and the tier 2 review can be found below.

### Analysis Backlog
A backlog is nothing else than a ToDo list with prioritised items. The backlog should be easily accessible to the analysis team, the working group and all reviewers. It is maintained by the maven reviewer. There are a few rules that have proven to be useful when working with such a backlog:

* Items on the backlog should be described as clearly and as specifically as possible. Larger items may be needed to be broken down into several chunks.
* Only the analysts themselves choose what they want to pick from the backlog to work on next.
* The maven reviewer is responsible to always have a clear order of priority of all the items in the list. Only they can remove items from the list or demote them to lower priorities. They assist the analysis team in the decision what to spend their time on. Items from tier 2 reviewers can't be removed from the backlog.
* Every working group member (in the later stages every member of the collaboration) can add items to the list. The maven reviewer has the last word on assigning priorities.
* Tier 2 reviewers can add special tier-2-items to the backlog. Those can only be closed by a tier 2 reviewer.
* Once the maven reviewer considers an item as done they mark it clearly in the backlog. It will be convenient to add a note detailing how the task was completed or how the issue was resolved. Tier 2 reviewers can reopen issues on the backlog if they have concerns. Once the collaboration reviewers are happy with an issue it is marked as approved in the backlog.
* An analysis is considered ready for approval when all open items are marked as approved by the tier 2 reviewers.
* Items can be closed without being done if the decision is taken to not pursue them further (see analysis triage).

### Analysis Triage
With an analysis backlog in place and properly maintained it will become much more transparent what is still needed to bring an analysis to a state where it can be released. The priorisation of items on the ToDo list is crucial because it allows a shift of focus from the question "How can we complete everything requested in time?" to the question: "Which items are the most important to get right? Which of those do we have completed when the deadline hits?". 

Analyses, like any project, are never really finished. At some point the reviewers have to take the decision when the analysis team should stop. We argue that it is better to make this decision transparent in the form of the analysis backlog. This includes stating clearly which items will not be completed for the release (because they are not worth it). On the other hand this kind of transparency should make it also more acceptable to delay an approval to the next opportunity if there are still major issues on the backlog. 

The prioritised backlog provides the basis for this decision making process, which happens in discussion between the reviewers and the analysis team. In practice this will mean that open issues on the backlog are either approved or closed.

### Code Review
In our view a data analysis consists of the following artefacts
* The input data as delivered by the experiment;
* The computer programs encoding the full analysis algorithm;
* The analysis note that explains, documents and justifies the applied techniques;
* The paper that summarises the analysis algorithm and presents the physics results obtained by applying it to the input data;

The actual work delivered as the outcome of a typical analysis project are the code, the note and the paper. While the note and the paper are crucial documentations, the code is the actual tool to perform the study. As such it in itselve often represents a substantial investemnt of time and effort. Furthermore the code contains the most precise (but not most readable) documentation of what has actually been done. It should be reviewed on equal footing with the ANA note and the paper. Given the nature of code the focus of such a review will be different than a paper-review.

The basic necessity to enable code review is that **the complete analysis code is made available to the collaboration**. This is also the only requirment that should be formalised in the review process. Hosting the code on a repository sevice such as http://gitlab.cern.ch will be the most practical solution.

The maven reviewer checks that the code is made available, is complete and documented well enough, such that the analysis can (at least in principle) be rerun by any member of the collaboration.

This last statement has some implications on how analyses are implemented. All of these implications are desired and encouraged by the design of this review process. 

1. The analysis code has to be complete and automatic. The complete recipe, including all the systematic checks has to be made available. It will be convenient to write down this recipe in machine-executable form. This implies that all plots and numbers have to be generated in a scripted manner.
2. The code has to be documented well enough that a skilled person can install and run it. Ideally with the help of a self-executing analysis recipe.
3. All dependencies of the code are well documented. It is known that some of the programs in use are highly specialised and might require special hardware (such as a GPU cluster) to run in a finite time. In that case the dependencies have to be explained well enough that a reproduction is in principle possible. This might require giving the maven reviewer access to specialised computing hardware.
4. It will be convenient, but not necessary, to make intermediate results (ntuples, results of expensive fits,...) available and to finely subdivide the analysis workflow such that a user can rerun only those parts which interest them.

The analysis code repsoitory should be made available as soon as the project starts. **Ideally the maven reviewer can run the current state of the analysis for themself as a preparation for the regular (biweekly) meetings with the analysis team.**
 
The complete working group is invited to contribute improvements to the analysis code. It is the decision of the analysis team whether or not to accept these contributions. A well tested workflow for this can be found [here](https://gitlab.cern.ch/help/workflow/forking_workflow.md).

Requests for improvements to the code can be put onto the analysis backlog. But the analysis should only be delayed by this if either a bug causes wrong results or if the public code is in an incomplete state that does not allow it to be reused. It is appreciated that analysis code represents very personal and valuable contributions to the collaborative effort. As such the reviewing of the code has to adhere to the same high standards of fairness and good conduct as any other interaction in the collaboration. The balance between valueing the individual and the necessity for a common language, understood by all, is particularly delicate when it comes to code. Dogmatism has no place in this. We thus strongly suggest to refrain from the enforcement of formal coding standards.









[1] : the term `maven` comes from Hebrew, loosely translated to "one who understands". There is no particular significance attached to the expression. You can substitute it with "mentor", "senpai", or just "working group reviewer"


