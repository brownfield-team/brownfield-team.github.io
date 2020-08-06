# BP-Pro (Brownfield Project Dashboard)

BP-Pro provides a portal for instructors and student to integrate 
data from GitHub and Slack, and tools to more effectively adapt
GitHub for a course with software projects.

It helps automate:
* Student signup for a course GitHub organization
* Mapping students from a course roster to Github accounts
* Assignment of students to teams in GitHub
* Creating repositories with the correct team permissions
* Gathering data from GitHub on a per student or per team basis.

# Who can use bp-pro

Currently, only partner instructors enrolled in the NSF Brownfield project.
It is possible that we may open up usage to other instructors in the future.
Contact Phill Conrad (phtcon@ucsb.edu) to sign up.

# Tutorial Materials

| Topic | Slide Deck | Video |
|-------|------------|-------|
| Setting up a New Course | [slides](https://docs.google.com/presentation/d/1KbNZROA-Y3Ybz2c18RyDedCOYiUaZkiOA42AHIWeEUQ/edit?usp=sharing) |  Coming soon | 
| Setting up Teams | [slides](https://docs.google.com/presentation/d/1B83b2RJpEu_xqIKNLvjrbVlHQdZei9eIsvp2DYJ1Gk0/edit?usp=sharing) |  Coming soon | 
| Adding a Slack Workspace | [slides](https://docs.google.com/presentation/d/1AZESrHQYOUVPMxW3tL1IxeBYml0BOffCnFl2MPGWloE/edit?usp=sharing) |  Coming soon | 
| Data Insights | Coming soon |  Coming soon | 


# Is BP-Pro open source?  Can I host my own instance?

Yes.  It's implemented in Ruby on Rails (with a little React on the top).  The source code is currently at https://github.com/project-anacapa/anacapa-github-linker
so in principle, you could host your own copy.   We are currently unavailable, however to assist or
advise on deployment issues, so you're on your own for that.  Having said that, we deploy on
Heroku and it's pretty straightforward if you are familiar with Ruby on Rails.   For a small
instance with few courses and modest enrollments, it should fit on the free tier of Heroku just fine,
thought you might need to keep any eye on your total database rows if you turn on Hooks.





