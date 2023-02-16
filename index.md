### Git basics
# What is Git?
 Git is a version control system and is used to manage changes in source code during software development.
# Why use Git? What problem does it slove?
A way for developers to work togeather simultaeously and merge their changes togeather and keep track of edit made to code over time is a few things using git helps with.
# What is the difference between Git and Github?
The difference between Git and GitHub is that Git is a stand-alone version control system used to manage changes to source code, while GitHub is a cloud-based platform that offers Git repository hosting as well as various additional functionalities to facilitate software development workflows.
### Git rebase

# What is Git rebase?
Git rebase integrates changes from one branch into another, usually the main branch, in a more organized way than Git merge.

# What are some advantages and disadvantages of Git rebase? (At least 2 of each)
**Advantages**
- Streamlined and well-organized project history due to a linear incorporation of changes into the target branch.
- Allows for a cleaner commit history that facilitates debugging and code reviews.
**Disadvantages**
- The risk of data loss, as changes made in the current branch are rewritten and can cause conflicts or data loss if the operation is not carried out carefully.
- The possibility of accidentally overwriting changes made in the target branch if changes are made to a branch that is later rebased onto another branch.

# When shouldn't you use Git rebase? Why?
If you are working on a branch that is shared publicly with other developers, it is not recommended to use Git rebase since it can lead to confusion and conflicts for those who have already incorporated your changes.

# Create a new repo and demonstrate your knowledge of the following items with screenshots:
- A rebase merge
![merge rebase example](/img/merge%20rebase.png)
- An interactive rebase merge
![interactive rebase example](/img/rebase_i.png)

- When you shouldn't rebase with a remote repo.
On a branch that has been pushed to a remote repository, especially if the branch is being worked on by multiple developers. 

### Git reset, checkout, and revert

* What is Git reset?
* What is the difference between hard, mixed and soft?
* What is Git checkout?
* What is Git revert?
* In what ways are these commands the same and what ways are they different?
* When would you use reset, checkout, or revert? Why?

Create a new repo and demonstrate your knowledge of the following items with screenshots:

# Git reset
Move the HEAD and the branch pointer to a different commit, essentially resetting the branch to an earlier state.
# Git checkout
Switch between branches, create new branches, and move the HEAD (the pointer to the current branch) to a specific commit. 
# a commit
Captures a snapshot of the repository at a specific point in time, including all the changes that were made since the last commit.
# Git revert
Allows you to undo one or more existing commits in a repository. 

### Git submodules

# What are Git submodules?
Git submodules are a feature that allows one Git repository to be embedded within another Git repository. This enables you to manage separate projects within a larger project or integrate third-party code into your own codebase. Submodules can be useful for organizing complex projects, but they can also add complexity to your workflow and require additional management.

#  When would you use a submodule?
This can be useful when working on a larger project with smaller projects or external dependencies. Submodules simplify the management of different versions of external code and make it easier to keep the codebase organized. For example, if a web application relies on a third-party library, a submodule can be used to manage the library's code and update it separately from the main codebase.

# What are the advantages and disadvantages of Git submodules?
 **Advantages**
 - They make it easy to reuse code across multiple projects as you can include a submodule in multiple repositories.
 - They enable you to maintain an organized codebase by separating external code from your own code.
 - They simplify the management of different versions of external code used in your project by allowing you to update and manage them independently.

**Disadvantages**
-  Submodules require a good understanding of Git and can be difficult to use for beginners.
- Managing submodules requires additional commands and can add complexity to your workflow.
- Using different versions of submodules across different branches or repositories can cause versioning issues and make it challenging to maintain consistency across your codebase.