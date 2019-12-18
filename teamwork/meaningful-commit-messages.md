# Writing Meaningful Commit Messages

Most folks that have worked with `git` and GitHub for any length of time have experienced the phenomenon illustrated in this XKCD comic by Randall Munroe:

![https://xkcd.com/1296/ about Git Commit Messages](/teamwork/meaningful-commit-messages/git_commit.png)

It's funny because it's true. 

However, in professional software development practice, it turns out to be important to write meaningful commit messages.  This is especially as code bases get large and live for a long time (in contradistinction to short lived personal projects or assignments).

Many IDEs, as well as the GitHub web interface, have a feature that will annotate each line of source code with the commit that produced it, along with the SHA, the commit message, and *your name* as the developer that made the commit.

It is a matter of professional pride that you'll want your commit messages to be meaningful and useful.

# How to write good commit messages

There are many articles on this topic, so rather than reinvent the wheel, we will refer you to a few of them.

Chris Beams' article <https://chris.beams.io/posts/git-commit/> includes this list of seven rules, along with a great explanation of each of them.  Note that his post assumes that you are going to write a multi-line commit message.   The most important line, though is the
subject line.

1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs. how

Chris Beams' also links to six other articles on this topic with the sentence:

> <em>Keep in mind: <a href="http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html">This</a> <a href="https://www.git-scm.com/book/en/v2/Distributed-Git-Contributing-to-a-Project#_commit_guidelines">has</a> <a href="https://github.com/torvalds/subsurface-for-dirk/blob/master/README.md#contributing">all</a> <a href="http://who-t.blogspot.co.at/2009/12/on-commit-messages.html">been</a> <a href="https://github.com/erlang/otp/wiki/writing-good-commit-messages">said</a> <a href="https://github.com/spring-projects/spring-framework/blob/30bce7/CONTRIBUTING.md#format-commit-messages">before</a>.</em>

