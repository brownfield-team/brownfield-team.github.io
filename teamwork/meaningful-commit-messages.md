# Writing Meaningful Commit Messages

Most folks that have worked with `git` and GitHub for any length of time have experienced the phenomenon illustrated in this XKCD comic by Randall Munroe:

![https://xkcd.com/1296/ about Git Commit Messages](/teamwork/meaningful-commit-messages/git_commit.png)

It's funny because it's true. 

However, in professional software development practice, it turns out to be important to write meaningful commit messages.  This is especially as code bases get large and live for a long time (in contradistinction to short lived personal projects or assignments).

Many IDEs, as well as the GitHub web interface, have a feature that will annotate each line of source code with the commit that produced it, along with the SHA, the commit message, and *your name* as the developer that made the commit.

It is a matter of professional pride that you'll want your commit messages to be meaningful and useful.

# How to write good commit messages

There are many articles on this topic, so rather than reinvent the wheel, we will refer you to a few of these, adding some additional commentary.

Note that these rules *apply equally* to writing the *high level description of a Pull Request*, perhaps even more so.

## Three rules

Peter Hutterer, an Australian blogger about software, proposes three rules for commit messages in this [blog post](http://who-t.blogspot.com/2009/12/on-commit-messages.html), which I've paraphrased and summarized here:

1. *Why* is it necessary? 
2. *How* does it address the issue? 
3. *What non-obvious effects* does the change have? 

You typically won't be able to fit all three into 50 characters.  

If so, use the first line to address the most important one or two that you can fit,
and use a multi-line commit message.  (Did you know you can do that?)

Here are a few more notes on each of these:

1. *Why* is it necessary? 
  * Does it fix a bug?
  * Does it add a feature
  * Does it improve performance, reliabilty, stability
  * Does it 

2. *How* does it address the issue? 
  * If it's a short change, and obvious from the code, this can sometimes be omitted.
  * Otherwise, at least a high level description shoudl be there.
 
3. *What non-obvious effects* does the patch have? 
  * Does it introduce a new dependency?
  * Does it change what a developer has to do to launch the application?
  * Does it change how a user interacts with the app in a fundamental way?
  * Are there performance implications or side-effects?
  

## Chris Beams' seven rules

Chris Beams' article <https://chris.beams.io/posts/git-commit/> includes this list of seven rules, along with a great explanation of each of them.  Note that his post assumes that you are going to write a multi-line commit message.   The most important line, though is the
subject line.

1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs. how

Chris Beams' also links to six other articles on this topic with this sentence; each word is a link to another article (one of which is the Peter Hutterer article already linked to above.)

> <em>Keep in mind: <a href="http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html">This</a> <a href="https://www.git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project#_commit_guidelines">has</a> <a href="https://github.com/torvalds/subsurface-for-dirk/blob/master/README.md#contributing">all</a> <a href="http://who-t.blogspot.co.at/2009/12/on-commit-messages.html">been</a> <a href="https://github.com/erlang/otp/wiki/writing-good-commit-messages">said</a> <a href="https://github.com/spring-projects/spring-framework/blob/30bce7/CONTRIBUTING.md#format-commit-messages">before</a>.</em>

