# Getting started - Git


This session I will show you the basic notion when using Git. To make it
easier the content of documentation are gonna display under the couple
of questions. So don\'t waste your time anymore. let\'s get started

## What is Git?

Git is a distributed version control system (DVCS) widely used in
software development to track changes in source code and collaborate on
projects.

Overall, Git is a powerful tool that simplifies version control and
enables efficient and collaborative software development. Developers use
Git to track changes, work on different aspects of a project
simultaneously, and maintain a reliable history of their work.

## Why do we need to use Git?

Here are some key reasons why we need to use Git:

-   **Version Control:** Git allows developers to track changes made to
    their codebase over time. This is essential because software
    development is an iterative process, and having a version history
    helps manage and reference different stages of a project.
-   **Collaboration:** In software development, multiple team members
    often work on the same project simultaneously. Git enables seamless
    collaboration by allowing developers to work on their own branches,
    merge changes, and resolve conflicts. This prevents conflicts from
    disrupting the development process and makes it easier to work
    together on a codebase.
-   **Branching and Experimentation:** Git makes it easy to create
    branches, which are separate lines of development. Developers can
    create branches to work on new features, bug fixes, or experiments
    without affecting the main codebase. This helps maintain a clean and
    organized code repository.
-   **Code Review:** Git integrates well with code review processes.
    Developers can create \"pull requests\" (or \"merge requests\" on
    some platforms) to propose changes for review by their peers. This
    ensures that code changes are thoroughly examined before they are
    merged into the main codebase, enhancing code quality and catching
    potential issues early.
-   **Fault Tolerance:** Git is distributed, which means that every
    developer has a complete copy of the code and its history on their
    local machine. This redundancy provides a level of fault tolerance
    and ensures that even if a central server goes down, development can
    continue from individual copies of the repository.
-   **Documentation:** Git commit messages serve as a form of
    documentation. Developers can provide detailed explanations of the
    changes they\'ve made, making it easier for others (and their future
    selves) to understand the purpose and context of each change.
-   **Reproducibility:** Git allows you to precisely reproduce any
    previous state of your project. This is valuable for debugging,
    testing, and ensuring that you can recreate a specific version of
    your software if needed.
-   **Open Source and Community Collaboration:** Git\'s open-source
    nature has led to a vast ecosystem of tools, extensions, and
    resources. It\'s the backbone of many collaborative development
    platforms like GitHub, GitLab, and Bitbucket, which facilitate
    community involvement and sharing of open-source projects.
-   **Scalability:** Git is scalable and can be used for projects of
    various sizes, from small personal projects to large
    enterprise-level software development. Its flexibility and robust
    branching and merging capabilities make it adaptable to diverse
    development needs.

## What is GitHub/GitLab?

GitHub and GitLab are two popular web-based platforms that provide
hosting and collaboration services for Git repositories. They serve
similar purposes but have some differences in their features, target
audiences, and business models.

## What is Repository? What kind of Repository?

### Repository

A repository, in the context of version control systems like Git, is a
data structure that stores a collection of files, their revision
history, and metadata related to those files. It serves as a centralized
location where you can manage and track changes to your project\'s
source code or other files. Repositories are fundamental to version
control, as they enable you to:

-   **Track Changes:** A repository records every change made to the
    files it contains, including who made the change, when it was made,
    and what was changed. This historical information is crucial for
    understanding the evolution of a project.
-   **Collaborate:** Multiple developers can work on the same project
    simultaneously by cloning a repository, making changes, and then
    merging those changes back into the main repository. This enables
    collaboration and prevents conflicts when multiple people are
    working on the same codebase.
-   **Backup:** Repositories serve as a backup mechanism for your
    project. If you lose local copies of your files or encounter issues,
    you can always recover the latest version from the repository.

### Types of Repositories

There are different types of repositories based on their purpose and
hosting location:

-   **Local Repository:** This is a repository stored on your local
    computer. When you initiate a new Git repository in a directory, you
    create a local repository. It\'s used for individual development or
    as a starting point for sharing your code with others.
-   **Remote Repository:** Remote repositories are hosted on a server or
    a cloud-based platform. These repositories allow collaboration among
    multiple developers. GitHub, GitLab, Bitbucket, and similar
    platforms provide remote repositories where teams can push and pull
    changes.
-   **Centralized Repository:** In some version control systems, like
    Subversion (SVN), there is a single centralized repository that all
    developers commit to. Git\'s distributed nature means it doesn\'t
    require a central repository, but teams often use remote
    repositories on platforms like GitHub or GitLab as a central point
    for collaboration.
-   **Bare Repository:** A bare repository is a special type of remote
    repository that doesn\'t have a working directory. It only contains
    the Git data and is typically used as a central repository for
    collaboration. Developers can\'t work directly in a bare repository;
    it\'s just for storing and sharing changes.
-   **Public Repository:** This type of repository is accessible to the
    public. It\'s often used for open-source projects where anyone can
    view and contribute to the code. GitHub and GitLab host many public
    repositories.
-   **Private Repository:** A private repository is restricted to a
    specific group of users or collaborators. Only authorized users can
    access and make changes to the code. Both GitHub and GitLab offer
    private repository options.
-   **Forked Repository:** A forked repository is a copy of another
    repository. It\'s often used in open-source development when a
    contributor wants to make changes to a project without directly
    modifying the original repository. Changes made in a fork can be
    submitted as pull requests or merge requests to the original
    project.

These various types of repositories cater to different development
scenarios, whether it\'s individual work, collaboration within a team,
open-source contributions, or managing project history and backups. The
choice of repository type depends on your project\'s requirements and
your preferred workflow.

## What is commit? What is branch?

### Commit

In the context of version control systems like Git, a \"commit\" refers
to the act of saving or recording changes to a set of files in a
repository.

### Branch

In Git, a \"branch\" is a lightweight, movable pointer to a specific
commit in the version history of a Git repository. Branches allow you to
work on different lines of development within the same project
simultaneously. Each branch represents an independent line of
development, often focused on a particular feature, bug fix, or task.