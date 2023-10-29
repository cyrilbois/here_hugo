---
title: "Pull Request Etiquette"
date: 2023-08-06T07:15:54+02:00
description: We’ll look at this from two perspectives, the pull request author, and the reviewer
tags: [process, collaboration, communication, git]
images: ['https://images-here-hugo.vercel.app/api/og-image?title=Pull%20Request%20Etiquette']
aliases: ['pr-et']
---

# Author Etiquette
The idea is to make a pull request easy on the reviewer. Another opportunity to reduce [irrelevant cognitive load](/cognitive-load-theory/#2-extraneous-irrelevant-load), and increase profit 💸.

**This is done by providing as much context as possible.**
- Link to ticket
- Link to designs
- A summary of the work done. this can be a few bullet points
- Explicitly point out areas you want the reviewer to pay close attention to
- Steps to reproduce (if it’s a bugfix)
- How to test - if you describe the happy path, the reviewer knows which areas to look out for error handling

Michael Lynch has great articles about code review. He shares [How to Make Your Code Reviewer Fall in Love with You](https://mtlynch.io/code-review-love/)

# Naming Conventions

## Branch Names
I've seen naming conventions exist at branch level, and commit messages.

When naming branches, usually the ticket number alone is enough. You can also prefix them to indicate the type of work being done
eg `bug`, `hotfix`, `feat`, `chore` etc.

[Tyler](https://www.tylerpillay.co.za/) mentioned:
> personally I’m not a fan of the ticket number in the branch name because it adds noise. I’d rather have like `feat/submit-claim-logic` or similar and on your PR you link the ticket there.
> If you’ve got the **Jira/Github integration** then it’s very useful because the branch will be populated in the ticket just by virtue of having the ticket number in the branch name so that’s pretty dope and useful depending on who’s looking at it

I agree, the real value in naming branches with ticket number is with the automation you can do with it.

The idea is to pick one approach as a team, and go with it.

## Commit Messages
Commit messages accompanied with prefixes also provides rich context. [Angular conventional commits](https://www.conventionalcommits.org/en/v1.0.0-beta.4/) is a good standard to start from.
When done well, good commit messages are an area to provide rich context to your reviewer, it allows one to jump in and out of points of interest, and give more insight into how you came to your eventual solution.

Two articles on the topic:
1. [How to Write a Git Commit Message](https://cbea.ms/git-commit/)
2. [My favourite Git commit](https://dhwthompson.com/2019/my-favourite-git-commit)

---

# Reviewer Etiquette
Michael Lynch has written very well detailed notes on doing code reviews well.
- [How to Do Code Reviews Like a Human \(Part One\)](https://mtlynch.io/human-code-reviews-1/)
- [How to Do Code Reviews Like a Human \(Part Two\)](https://mtlynch.io/human-code-reviews-2/)

# related reading
- [Ship, show, ask](https://martinfowler.com/articles/ship-show-ask.html)
- [My thoughts on Work In Progress Pull requests](/on-prs)
- [Analysis: The Quickest Path To Halving Software Delivery Time](https://devinterrupted.substack.com/p/analysis-the-quickest-path-to-halving)