---
title: Update GitHub fork
layout: post
---

[github]: http://help.github.com/fork-a-repo/ "Fork a repo"

You need *A feature* and you know how to make it by extending *B*,
an open source project repo hosted on GitHub.

You first should **fork** *B repo*, edit, test and commit your changes.

Than you send your *pull request* and you're done.

After some inactivity on your fork your local repo is outdated, how can
you update your fork getting code from the main repo?

1. Add `upstream` remote to track main repo

        $ git remote add upstream git://github.com/octocat/Spoon-Knife.git

1. Fetch upstream remote in your local repo

        $ git fetch upstream

1. Merge `upstream/master` in your current branch to apply updates

        $ git merge upstream/master 

Resources:

[GitHub Help - Fork a repo][github]
