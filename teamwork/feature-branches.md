# Feature Branches

This document describes a "feature branch" / "pull request" work flow that is typical of real-world software development both in the commercial 
software industry, and
on open-source software projects used in industry and in academic research.

We encourage all participants in the project to teach this model and use it in their courses, for three reasons:
* It teaches a widely used professional practice.
* It provides a "code review" stage which assists in evaluating student work.
* It helps teams coordinate when working a large scale code base.

# How is this different from what I'm used to?

When folks are first learning to work with `git` and GitHub, they often do all of their work on the `master` branch.

The typical work cycle is as follows:

* To start, you clone a repo from GitHub with <tt>git clone</tt> <i>repo-url</i>
* Then, each time you want to make a change, you use these steps:
   * <tt>git add</tt> <em>files...</em>
   * <tt>git commit -m</tt> <em>"commit message"</em>
   * <tt>git push origin master</tt>

This is fine for beginners, and when there is only one individual programmer (or perhaps a pair working together) contributing changes to a repo.

However, for real world software projects, it is more common to have many programmers, indeed many teams of programmers, working simultaneously on the same
code base.

To support this use case, `git` provides for multiple <em>branches</em> and GitHub provides a feature called <em>pull requests</em>.

# The feature-branch / pull request work flow, briefly summarized.

In this workflow, each time you want to work on adding a feature, or fixing a bug, you:

* First create a new branch, usually off a "fresh copy of master"
* You then make all of your changes to that branch, and that branch only.
* You make individual commits to this branch, early and often.
  * If possible, try to do the bug fix, or feature addition over multiple commits
  * Break up the work into small increments, where possible, each one being a version that compiles and moves closer to the goal
  * Each commit message should be meaningful and describe the work done in that commit.
* When all finished, you "rebase on master" (described below) 
  * This step integrates any changes that have been made to master in the meantime into your branch.
  * This doesn't not prevent, but it can help to simplify dealing with so-called "merge conflicts"
* Finally, you do a "pull request" to the master branch; this is done on the GitHub website.
  * This step indicates that you are requesting the manager of the project (typically your instructor, or someone they have 
    designated, such as a teaching assistant, or group leader) to merge your code into the master branch.
  * At this step, it is typical to perform one or more code reviews; GitHub has features to support this.
  * You may be asked to make revisions before your pull request is accepted.
* When the pull request is accepted, you are ready to start a new feature branch for your next bug fix or feature request.

# TODO: More detailed description of the steps above.

