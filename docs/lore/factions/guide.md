---
title: Faction Guide
description: A guide for creating documentation for your faction
author: Foxtrek64
---

# Faction Guide

Welcome, prospector! I see you're here to see about making a page for your faction! This document has a handy little guide for you. If you have any questions, please feel free to reach out to a member of the RavenRock or LuzFaltex Documentation Staff, either on Discord or by creating an issue here.

## The Technical Side

This section will provide an overview for the process of submitting your own faction documentation. There are three major steps with this process:

1. Fork the repository
1. Make any changes or additions you would like
1. Push the changes and make a PR.

For experienced GitHub users, this will be the flow you are used to. For those who are not familiar with this process, we recommend reading our [Contribution Guide](https://docs.luzfaltex.com/contribute/index.html), which will walk you through the process of setting up your machine to be able to contribute.

### I've written my documents, how do I make them show in the Table Of Contents?

After writing your documents, you will need to modify the toc.md document. How you do this will vary based on the size of your contribution, however the format is as below:

```md
# [Index](index.md)
# [First Level Link](factions/myFaction/index.md)
## [Child page](factions/myFaction/laws.md)
# First Level Label (clicking on this one just expands the category)
## [Child page 2](factions/otherFaction/index.md)
```

The system will automatically parse this out and display it in the side menu. Child items will appear underneath the corresponding item in the side menu.

## The Contribution Itself

Factions should be placed in their own folder provided in `camelCase`. Additionally, any special characters in folder and file names should be removed or changed to their "safe" equivalent (e.g. é -> e). Here are a few examples:

| Faction Name | Folder Name |
|---|---|
| Havana | havana |
| Montréal | montreal |
| Ville de Montréal | villeDeMontreal |

If you would like to create child folders within your category, you may do so. However, you will be required to make a new file called `toc.md` inside of your faction folder. If you do this, please only link to your `index.md` document.

### Best Practice and Standards

1. Your faction entry in the `toc.md` document should be a First Level Label (not a link).
1. Your first document should be named `index.md`. You can give it whatever title you would like and you may call it whatever you like in the table of contents.
1. Always provide your GitHub username in the `authors` section at the top of the document. This allows us to properly attribute your changes and other users know who to contact if needed.
1. Alphabetize the `toc.md` file (or at least the top level)! It makes it far easier for people to find your faction if it's in alphabetical order.