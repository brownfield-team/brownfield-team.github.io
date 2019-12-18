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
   * <tt>git commit -m <em>"commit message"</em>
   * <tt>git push origin master</tt>

This is fine for beginners, and when there is only one individual programmer (or perhaps a pair working together) contributing changes to a repo.

However, for real world software projects, it is more common to have many programmers, indeed many teams of programmers, working simultaneously on the same
code base.

To support this use case, `git` provides for multiple <em>branches</em> and GitHub provides a feature called <em>pull requests</em>.
