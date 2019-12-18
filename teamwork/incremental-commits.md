# Incremental Commits

Many developers that are new to `git` and GitHub may have the habit of waiting until all of their work is done before making their first commit.

This results in a commit that is *big*, by which we mean:
* It contains many files (more than 10 is a lot)
* It addresses more than one thing (e.g. it adds several features, or several aspects of a single feature)

These commits are challenging for your fellow developers to understand.  Indeed, they are challenging for *you* to understand, as they represent a big
change to the code base.

Professional software developers prefer "small, frequent, incremental" commits.   These have several advantages:
* Each commit is easy to understand.  It affects only a handful of files.
* If you are working with automatic tests that kicked off when you commit, those tests are run frequently.
* If you are working with other developers, or asking instructional staff for help, they can see your code on GitHub
* If you have to back out a change, it is easier to back out in small incremental steps.

Perhaps the most important aspect is the very fact that constructing your 
commits this way it helps guide you towards break down the task you are doing into small incremental steps.


# But, what if ... ?

There are *always exceptions* to the guidelines above.   

For example, there may be a case where it is appropriate for a single commit to touch dozens of files.  Such a case might if you are changing the name of a module or
package, which requires changing, for example:

```java
package edu.myschool.sample;
```

to 

```java
package edu.myschool.rideshare;
```

across dozens of files.  

However, in that case, the spirit of the guideline still applies!

* Your commit to do this refactoring should DO NOTHING ELSE
* That way, even though the code reviewer may have to look a dozens of files, the changes in each one are *easy to understand*,
  and all have a *single purpose*
  
