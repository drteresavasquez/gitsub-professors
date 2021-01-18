# Foundations Group Project - GitSub Website

As a team, build a clone of the GitHub website as outlined below. Be creative and have fun.

## Requirements

### Theme

Use the Github website as a foundation for layout and styles that you will need to try to implement. 

* Your team can only have 1 CSS and 1 JS file
* Vanilla HTML, CSS, and JS only
* Your team should be using bootstrap

### Pages
Each team member is going to be responsible for the content of a different page, so decide on the name and content for each of those pages. We know that Githib uses tabs, but we want you to create separate pages with the same styles applied to them for consistency.

Some possible options are:

- Overview page
  - Includes a form that allows a user to add a pinned repository
- Repositories page
  - Includes a form that allows a user to create a new repository
- Projects Page with at least 5 projects listed on the page
  - Includes a form that allows a user to add a new project
- Packages Page
  - Includes a form that allows a user to add a package to the list of packages

### Data

Create data objects that you can use for your website. Do not duplicate objects or arrays. If multiple team members need the same data, create one data source for everyone to use.

### Teamwork

Create a Project board for your site and make the columns for 'Backlog', 'Todo', 'Doing', 'Code Review', 'Done'. Create notes for different units of work, make the notes into issues, and assign it to the team members doing to work. When you are assigned to an issue, make sure that you are moving it over to the right column on the board.

### Planning
Your team **MUST** use github projects to track tickets and progress on tickets.  We expect to see detailed wireframes for all different views in your project. These wireframes should be included in the appropriate ticket.

### Git
Your team is going to learn how to use git to enable good teamwork when building a software product.

1. Follow the instructons in class to clone down the repo
1. `cd` into the directory that got created.
1. Before anyone on the team writes a single line of code, the team will decide on a branch naming strategy. Branches should be descriptive of the work that is going to be done on that branch. Some teams also decide to add the developer's information to the branch name, such as initials. For example, a developer named Jasmine Sheboygen is going to work on the navbar for the web site. A good name for the branch would be `js-navbar`.
1. Your team already has a README.md file so there is no reason anyone should push to the main branch - LIKE EVER.  Also at some point there should probably exist a good, proper readme with screenshots

Now everyone will work on their page on those individual branches. Once a teammates feels that their work is complete, the teammate will push up their branch to Github and create a pull request. Decide as group your standard for reviewing and approving pull requests, for example, you may decide that each PR needs one thumbs up from another teammate, you may decide that everyone in the group needs to give it a thumbs up, etc. At the very least, one of the other teammates must review the pull request and give a thumbs up (Just type :+1 in the comment box).
```bash
# Check to make sure that your working tree is clean. Add and commit all that you need to.
git checkout main
git fetch
git branch -al
# ^ The code above shows you all active branches that are available to you on GitHub.
git checkout your-teammates-branch-name
# Test test test
```

Once the PR gets a thumbs up, the teammates should merge the current version of main (the one with all their teammate's fancy additions) to their current working branch by following this process:

```bash
# Check to make sure that your working tree is clean. Add and commit all that you need to.
git checkout main
git pull origin main
git checkout your-branch-name
git merge main
# Fix any merge conflicts, if you have them
# git add and git commit any files affected by the merge conflict.
```

Now you have all of your work, plus all of your teammate's approved work on one branch. :cool:

### Javascript
* EVERY SINGE PAGE must include a JS loop of some kind
* Your team can only have 1 JS file - main.js
* All your JS should be written in functions.  Wherever possible reuseable functions.

**:warning:** DO NOT start coding until an instructor has looked at your github project.

### Twists
Your project must include each of the following:
* **Complex Data** - At least 1 of your pages should use a more complex data structure.  This means that one of your arrays should have an array inside each object.  For example:  your repos could have an array of objects called users and each of your users could have an array called social media in it.  You then would have to figure out how to display all the users and their social media in the domString
* **Dynamic Buttons** - somewhere in your project there should be some dynamically created buttons (NOT IN THE HTML...RENDERED USING JAVASCRIPT) - clicking each button should perform some sort of action
* **Form** - Each page in your project should have at least 1 form.  Submitting that form via a button click should do something.
