#LVTools Palettes
================
#####This project serves as a repository of tools which we have found useful in our day-to-day work.
================
This repository and any materials provided by NI therein are provided AS IS. NI DISCLAIMS ANY AND ALL LIABILITIES FOR AND MAKES NO WARRANTIES, EITHER EXPRESS OR IMPLIED, INCLUDING WITHOUT LIMITATION ANY WARRANTIES OF MERCHANTABILITY, FITNESS FOR  PARTICULAR PURPOSE, OR NON-INFRINGEMENT OF INTELLECTUAL PROPERTY. NI shall have no liability for any direct, indirect, incidental, punitive, special, or consequential damages for your use of the repository or any materials contained therein. 
================

##Goals:
Develop a large set of palettes which provide common tools that can be shared across our organization and with our partners and customers.
 
##Background:
Our organization does a reasonable job of promoting reuse of reference designs and specific APIs, but does not do a good job of sharing or aggregating less complete sets of tools. The LabVIEW community has done a good job of this in the past, with toolsets like OpenG, MGI, and GPower. This project does not aim to replace these tools, but to instead make additional toolsets available to the community.
 
##Overview:
At present, the project is in an exploratory stage. The concept is that individual contributors to this project should create a fork and add their own tools to the project in a way that is as organized as possible. Based on those forks and contributions, project maintainers will attempt to organize the tools in a logical fashion and  then pull changes from other contributors into the main line of the project. These will then be packaged and made available for distribution.
 
##Repository Overview:
The repository has a single main trunk. Contributors should create forks and then generate a branch for every contribution. This makes it easier to merge specific contributions into the main codebase.
 
##Test Process:
Because this is a toolset, we don't expect most users to have tests built and ready to go. However, tests are encouraged whenever possible, as this allows later contributors to be sure that they are not modifying the expected functionality of the API. 
Any FGVs should have tests. Any APIs should have tests. Individual functions do not require tests, but complex functions should have tests.
 
##Build Process:
Describe how to build the code, and what the expected build artifacts are. This is critical, as all submissions should result in code that builds. If applicable, describe a test plan for the generated build artifact (required if the result is an executable, not required if the result is a source API).
 
##Contribution Workflow:
*For a more complete workflow, view [this set-up guide](https://decibel.ni.com/content/docs/DOC-37416) and [this workflow guide](https://decibel.ni.com/content/docs/DOC-37417).*

1. Fork this repository into your account.
2. Create a branch for your contributions.
3. Make changes, periodically pulling and merging any updates from the central repository.
4. Push your changes up to your branch in your copy of the repository.
5. Send a pull request to the owner of this primary repository. Follow the contribution guidelines.
 
##Contribution Guidelines:
- Limit the scope of your change as much as possible. Smaller changes are easier to process. Any major changes should be discussed beforehand with the managers of the repository to ensure that it fits within the goals and vision of the project.
- Explain the reason for your change with as much detail as possible. If it is a bugfix, link it to an issue in the issues tracker. If it is an enhancement, consider making an issue in the issue tracker to discuss the enhancement before making it. This ensures that the enhancement will provide value to other users.
- Run through the style guidelines and any available VI analyzer tests to ensure compliance with the general style of the project. Don't go crazy trying to make the code perfect. Do make sure there are no glaring issues.
- Before committing a change, be sure to rebase or merge your code off of the most up-to-date source in the master. This reduces the risk of merge conflicts and makes it that much easier to merge your pull request and that much more likely that the change will be accepted.
- Ensure that all builds are successful with your change in place, after rebasing.
- Ensure that all tests pass with your change in place, after rebasing.

##Special Contribution Guidelines:
- Keep all commits and/or pull requests organized along atomic units. That is, a FGV and enum should be submitted in one commit and one pull request. An API should be one commit and one pull request. A library of N functions related to manipulation of time should be N commits and N pull requests.
