# Using a GitHub Organization

We would like to ask all project participants to create a single GitHub Organization per course instance, and have students create all of their repos
within this organization.

For example:

* `ucsb-cs56-f19` for UCSB CS56 Fall 2019  
* `ucsb-cs56-w20` for UCSB CS56 Winter 2020

In the guide below, we'll explain:
* How to set this up at no cost, including unlimited public and private repos
* A few of the benefits of using an organization
* How to configure the settings to be appropriate for an academic course

# Setting up an organization at no cost

To set up an organization for your course with unlimited private repos:

1. Login to github.com and first create an organization on the "Free for Open Source" plan.  
  * NOTE: *You will still be able to have closed source private repos*, but creating a repo on the free, open source plan is the first
    step to obtaining your academic discount.
  * Use the "New Organization" menu item

2. Visit the link <https://github.com/education> and click the "Get Benefits" button where you can request to register as an educator.
   * There is a brief verification process.  Once you've completed this, you won't have to do it again for a while.

3. Once you've been verified as an educator:
   * Return to the "Get Benefits" link at  <https://github.com/education>
   * You should see an option to upgrade your organization(s).

If you already know your teaching scbedule a few terms in advance, you may want to go ahead and create the organizations now to ensure that the names
are available to you.

# Default Settings

A very important default setting that you'll want to adjust is the "Default Member Permissions".

1. Visit the settings page for your organization
   * For example, for `ucsb-cs56-f19` this link is `https://github.com/organizations/ucsb-cs56-f19/settings`
2. Find the `Member Privileges` item.
3. Change the default setting to 'None'

This is important because otherwise when you add students as member of the organization, they will be able to see one another's private repos.
You typically do not want that.

# Adding students as members.

There are at least three approaches to adding students as members to your organization:
* Adding manually
* GitHub Classroom <https://classroom.github.com/>
* Eventually, a roster upload feature will be integrated into the brownfield project dashboard.

# Benefits of using an organization

1. It gives you, the instructor, full access to all of the repositories in which your students are working,
   without them having to manually add you as a collaborator.
2. It allows you to also provide this access to any other individuals that should have it with a single command
   (by giving them admin access on the repo.)
3. It provides a single place where all of the repos for your course live.
4. You can create "teams" under the organization to control access to individual repositories.
   
   Typically, you'd give these teams "Maintain" access, which gives them access to do everything to the repo except push
   changes to the `master` branch.   This forces the feature-branch/pull-request work flow.
5. The PI team is planning to develop a brownfield dashboard that will interact with course organization to support
   academic workflows for brownfield courses.  The dashboard will be based on the assumption that each course is associated
   with a GitHub organization, and that the software development for the brownfield projects is done within that organization.
