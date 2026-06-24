# GitHub Data Dictionary

### Introduction
GitHub is the largest code repository and home to the largest developer community in the world with 83+ million developers, 4+ million organizations, and 200+ million repositories on our platform. GitHub is where most of the world’s software development happens, and as such, data on GitHub activity can offer unique insights on developer collaboration, productivity, and innovation over time.

### Software Collaboration Entities
Below is a non-exhaustive list of the most salient entities for studying collaboration on GitHub:
- A **repository** contains a software project that uses the [Git version control system](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F). Available data include: dependency graph (a list of other software projects that a given repository relies on generated from the manifest files contained in the repository), copyright license, contributors (contributing users with emails for the top 500 most prolific), stars, watchers, programming languages, [and more](https://docs.github.com/en/rest/repos/repos).
- A **user** can own repositories, participate as members of Organizations, and collaborate with other users via Issues, Pull Requests, Discussions, etc. Available data include: email, (self-identified) location, company, repositories, [and more](https://docs.github.com/en/rest/users/users#get-a-user).
- An **organization** can own repositories and are made up of Users, whose membership can be public or private. Available data include: email, location, company, repositories, members, [and more](https://docs.github.com/en/rest/orgs/orgs#get-an-organization).
- A **commit** is a snapshot of the state of a project’s files at a point in time. Available data include: committer name, committer email, time committed, [and more](https://docs.github.com/en/rest/commits/commits#get-a-commit).
- A **branch** is a named variant of a repository with a [given set of snapshots applied](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell#ch03-git-branching). Used to develop variations on the software project without changing the current version. Available data include: name, SHA-1 checksum, [and more](https://docs.github.com/en/rest/branches/branches).
- A **Pull Request** is a request for an authorized user to accept a set of proposed changes to a branch. Available data include: title, body, time opened, time closed, time merged, comments, [and more](https://docs.github.com/en/rest/pulls/pulls#get-a-pull-request).
- An **Issue** is a free-form submission associated with a GitHub repository that is often used to track bugs, ask questions, and plan work. Available data include: title, body, comments, time created, time closed, [and more](https://docs.github.com/en/rest/issues/issues#get-an-issue).
- A **Discussion** is a collaborative communication forum associated with a GitHub repository that is geared toward more open-ended conversations than Issues. Available data include: title, body, comments, reactions, [and more](https://docs.github.com/en/graphql/reference/objects#discussion).

### Examples of Research Using GitHub Data
- [McDermott, Grant R., and Benjamin Hansen. “Labor Reallocation and Remote Work During COVID-19: Real-time Evidence from GitHub.” NBER, 2021.](https://www.nber.org/papers/w29598)
- [Wright, Nagle & Greenstein. (2021). Open source software and global entrepreneurship: A virtuous cycle. Harvard Business School Working Paper, 20-139.](https://www.hbs.edu/ris/Publication%20Files/20-139_f108f488-ae3a-45e1-a1c8-38d83dfa661b.pdf)
- [Robbins, et al. (2018). Open source software as intangible capital: Measuring the cost and impact of free digital tools. 6th International Monetary Fund Statistical Forum.](https://www.imf.org/-/media/Files/Conferences/2018/6th-stats-forum/session-3carol-robbinsopen-source-software-as-intangible-capitalmeasuring-the-cost-and-impact-of-fre.ashx)

### Relationship Diagram of Collaboration-related Entities
![data_dictionary_relationship_diagram_light](https://user-images.githubusercontent.com/71285354/189771728-e562c660-971f-41bd-8841-cb17ca50f5fa.png#gh-light-mode-only)
![data_dictionary_relationship_diagram_dark](https://user-images.githubusercontent.com/71285354/189772406-0678dde4-b96b-462e-aa7c-d546369f5f5a.png#gh-dark-mode-only)


### Appendix
**Remaining Entities, relevant to research**
- Actions: [product documentation description](https://docs.github.com/en/actions); [API data availability description](https://docs.github.com/en/rest/actions/workflows)
- Activity: [product documentation description](https://docs.github.com/en/developers/webhooks-and-events/events/github-event-types); [API data availability description](https://docs.github.com/en/rest/activity) (Note: GH Torrent subscribes to this firehose)
- Codes of conduct: [product documentation description](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/adding-a-code-of-conduct-to-your-project); [API data availability description](https://docs.github.com/en/rest/codes-of-conduct)
- Code Scanning: [product documentation description](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning); [API data availability description](https://docs.github.com/en/rest/code-scanning#about-the-code-scanning-api)
- Gists: [product documentation description](https://docs.github.com/en/get-started/writing-on-github/editing-and-sharing-content-with-gists/creating-gists); [API data availability description](https://docs.github.com/en/rest/gists)
- Reactions: emoji reactions for issues/pull requests/discussions; [API data availability description](https://docs.github.com/en/rest/reactions)
- Releases: [product documentation description](https://docs.github.com/en/repositories/releasing-projects-on-github/about-releases); [API data availability description](https://docs.github.com/en/rest/releases/releases#list-releases)
