# Contributing Guidelines

Thank you for considering contributing to the MEDIANE Brevo-Rust API! We welcome contributions from everyone.

Following these guidelines helps to communicate that you respect the time of the developers managing and developing this open source project. In return, they should reciprocate that respect in addressing your issue, assessing changes, and helping you finalize your pull requests.

As we are a new project, we are looking for any kind of contribution starting with technical contribution to review the code and propose / implement new features. Though help developing the community and documentation are very welcome :) 

Here are some guidelines to help you get started:

## Your First contribution:
Unsure where to begin contributing to Brevo-Rust API? 
You can start by looking through beginner and help-wanted issues: Beginner issues - issues which should only require a few lines of code, and a test or two.
Help wanted issues - issues which should be a bit more involved than beginner issues.
Both issue lists are sorted by total number of comments.
While not perfect, number of comments is a reasonable proxy for impact a given change will have.

##Let's contribute !

1. **Claiming an issue / feature**
A first step in contributing to our project, is to find an issue that you’d like to work on.
You can explore currently available issues by navigating to the repository and clicking on the Issues tab.
Many of the issues will already be claimed, meaning that there is already a contributor working on the issue. If you really feel like working on this issue, you can contact the contributor and ask if they seek for help.
If you want to work an issue on your own, in order to see which ones are unclaimed you can scan the list and look to see if there is a contributor featured in the Assignee column, or look for a ‘claimed’ label.
Another method is to select the Labels drop-down menu and option-click ‘claimed’, which will filter the results to only show issues that are currently unassigned.

2. **Submit an Issue**
It is also possible to submit a new issue. If you have noted an error such as a typo or broken link, feel free to create a new issue for that correction. You can submit a new issue by clicking the *New Issue* button on the right-hand side of the page, selecting the applicable template and filling out the associated form.
While submitting an issue, please try to keep in mind that we need as much information as possible such as:
Clear and concise title:
Detailed description: Please use clear and concise language, avoid assumptions or ambiguous language.
If related to a bug add:
- Steps to reproduce
Visual screenshots if necessary: An image sometimes worth any words ;) 
OS: kind and version
WebBrowser: kind and version
Proposed solution: If you have an idea on how to solve the issue, please include it.


2. **Fork the Repository**: Click the "Fork" button at the top right of this page to create your copy of the repository.

3. **Clone the Repository**: Clone your forked repository to your local machine.
   ```bash
   git clone git@github.com:Juris-Power/brevo-rust.git
   ```
4. **Create a Branch** 
Create a new branch for your new feature or bug fix.  
If this is a new feature the branch name should be feature/name_of_feature  
If the is a bug fix, the name should be fix/num_of_issue
   ```bash
   git checkout -b feature/new_feature
   ```
4.1 **Additional setup**
@Claire please add here additional setup (languages and tools versions) in order to start using the API


5. **Commit your changes**

When writing, please follow our best practices and naming rules.
Try to commit as often as possible in order to separate different subtasks required. 
e.g. if implementing a new API endpoint, you can commit together the api file and the 200 post restponse to that request and on other commits the error management files; the update; delete if pertinent. 
 
   ```bash
   git commit -m "My clear commit message
   ```
6. **Push / submit your changes**
First you'll have to push your changes to your branch in order to make them visible.
We do that with a push to the separate branch we created earlier.
In order to do this we need remotes set up to connect to the repos on GitHub.
The origin remote is important. It is the connection between your local repo and your remote repo.
It can be set with the git remote add command. It is also recommended that you set up an upstream remote that points to the base juris-power/brevo-rust repo itself:
   ```bash
   # First check the remotes you have set up:
   git remote -v
   # if no upstream remote is already set up
   git remote add upstream https://github.com/Juris-Power/brevo-rust.git
   # Then push your code
   git push origin branch-name
   ```


7. **Open a pull request**
You’ll want to create a pull request (PR) so the maintainers can see the changes you want to make on the main Docs repo. After pushing your file to your forked repo, when we open up our forked or original repo on GitHub, you will notice a notification that appears near the top.

7.1 Click on "Compare & pull request"
You'll be redirected to a page with a markdown editor to create the PR.
As a title use the feature name / issue related to you PR. 
Add a description including any necessary information such as the approach you used, link to any external useful documentation.
Once created, your PR will be listed on the dedicated tab of the project.
It’s here that you will see the maintainers comment on and review your work.
It is possible you will see a review where a maintainer requests changes to your entry, these will be in a list of comments under the review and generally come in one of two flavors: 
a. A general comment describing specific changes that require rewriting parrt of the entry.
b. An edit suggestion. It comes with a box labeled "suggested change" and quote your entry with specific edit to the line in question.

Then you can now implement the changes either via your local repo or directly on the UI. 
Every new commit pushed will be visible in the PR. 
It is good practice to tag the reviewer when done with your changes so they can keep track of the PR and come back to you in a timely maner.
Once your PR has been reviewed and accepted, one of the maintainers will merge it to the Dev repo and your contribution will be soon online with the new production merge. Congratulations !
