# My weekly project plan

> Inspired by
>
> - [DataFusion weekly project plan (Andrew Lamb) - May 6, 2024](https://github.com/apache/datafusion/issues/10395)
> - [DataFusion weekly project plan (Andrew Lamb) - April 29, 2024](https://github.com/apache/datafusion/issues/10283)

## My (personal) North ⭐ :

- work for a great company and contribute to great open source project
  - Great company
  - Great open source project
    - Agones
    - kubeflow
- work from anywhere
- It would be great for other contributors to DataFusion who plan non trivial work could try to make them visible somehow as well 🙏 (feel free to copy / modify the format)

## My Highlights from Last Week

- [x] We have completed all subtasks of [EPIC] Tasks for a new Top Level Apache Project #9691 and expect that we will publish the blog Blog Post about graduating to a new top level project #10135 next week
- [] We made planning (even) faster with several more PRs for [EPIC] Stop copying LogicalPlan during OptimizerPasses #9637 (and [this pr](Stop copying LogicalPlan and Exprs in TypeCoercion (10% faster planning) #10356 gets another 10% faster)). Thanks @dmitrybugakov, @emgeee, @rohitrastogi,

## Looking for help

- [] Reviews of Add SessionContext/SessionState::create_physical_expr() to create PhysicalExpressions from Exprs #10330 and Stop copying LogicalPlan and Exprs in TypeCoercion (10% faster planning) #10356
- [] Someone to work on Make it easier to create WindowFunctions with the Expr API #6747 (there is a draft PR as @timsaucer hit this last week working with window functions

## My (personal) plans for this week

- [x] Complete removing copies to make planning faster: [EPIC] Stop copying LogicalPlan during OptimizerPasses #9637
- [] Help with DataFusion 38.0.0 Release #10217 with @andygrove

## Project Queue (list of future projects)

Not at the moment

## Projects I plan to help actively help review / plan

- [] Implement StringViewArray and BinaryViewArray arrow-rs#5374 (I am struggling to find time, but we are making progress, slowly)
- [] [EPIC] Collection of SQL to/from LogicalPlan/Expr tickets #9494
  Algorithm for (my) prioritizing PR reviews
  Note there are many committers who can and do review and merge PRs, so this is not the priorities of the project as a whole, just the approximate algorithm I use to prioritize my own time.

## Algorithm for (my) prioritizing PR reviews

Note there are many committers who can and do review and merge PRs, so this is not the priorities of the project as a whole, just the approximate algorithm I use to prioritize my own time.

Priority:

1. Bug fixes (where something is just incorrect), especially regressions (where it used to work and now does not)
2. Improvements directly related to features needed for InfluxDB (my employer)
3. Documentation and test improvements (I view these as very strategically important)
4. PRs that I think are strategically important
5. Other new features / additions to functionality (note this is the lowest)

The top strategically important projects in my head are:

- Anything that makes it easier to use DataFusion as a user (docs, examples, better APIs, etc), including Getting started guide for new users (who want to use DataFusion in their project)
- Anything that improves DataFusion's quality such as bug fixes, and improved / expanded tests, etc
- Making function packages modular and easier to mix/match
- Improved performance (with benchmarks)

Thus, if you are interested in contributing to DataFusion and are interested in a fast turn around time I would recommend looking into bug fixes / test improvements / documentation or the projects named above.

If you propose adding new functionality, especially if the PR is large/complex and not connected to a wider need, the review cycle will likely be longer. You can make it a shorter cycle by looking at the comments on other recent PRs and following the same model (e.g. ensure there are tests in sqllogictest for example, the CI passes, includes documentation, etc)

## Background

The idea of this ticket is make my plans for DataFusion visible, largely for my own personal organizational needs, but also to:

- Communicate / coordinate in the community
- Help provide an interesting summary of what is happening in DataFusion this week
