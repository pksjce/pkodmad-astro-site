---
external: false
date: 2025-08-15
title: "Copilot makes me feel..."
---

When I joined  back to work after my parental leave, I was intimidated by the advances in AI. I was determined to give it a fair shot and I am truly convinced that it is a compelling tool for developers that has pretty good future potential.
But this post is about how copilot makes me feel. Specifically when it writes large swathes of code for me.

Many times as a react developer, I do the same things all the time. Spinning up the configuration, setting up folder structure, testing infrastructure, stories etc. And  Generative AI will help me reduce the toil. 
So I've been using it wherever I can. 

I started with the "ask" mode on copilot, used it as I would google. I've since stopped doing this as the information is verbose and tedious to read. There's a reason we read content on websites and not on long chat threads. Since then I have discovered roles for AI and have mostly used it cut back on the agreeablitiy and verbosity. A huge improvement.

Within the first week, I hear everyone raving about agent mode. That copilot can take over for you and do multiple steps to write affect a broader section of the codebase. Copilot instructions can add any guardrails.

The second week, I learned about assigning issues to copilot. Ever since then, I've never scrimped on the issue description. I write everything I know about it as though it was a journal and simply assign it to the agent to create PRs. A few cases when I need multiple PRs or cross reference issues in other repos, I copied all the instructions on to copilot chat and had it take everything from there.

I will then meticulously review this PR that copilot has created. This is where my feelings have come into play.

I have generated a lot of PRs with copilot this month. The work has spanned a broad range of tasks. Pull requests to migrate between jest to vitest, writing new lint rules, fixing small bugs, fixing bugs that have a complex root cause, adding a new feature and so on. 

Copilot is a different kind of coder compared to me. It's characteristics include being thorough in its code covering multiple edge cases, writing a lot of comments, writing large if statements, repeating code and so on. As a reviewer, I feel myself constantly compromising by agreeing with its approach. If it was me, I wouldn't have written it that way. When in actuality, it is me who is supposed to be writing this and I have all the autonomy to change it however I want.

This is where Generative AI goes up in flames. Making changes to an initial draft. Its so insidious in its changes that I find myself reverting it to start over. Arguing with it over a PR to make changes is even more tedious in my opinion, the code feels more set in stone when its hosted. 
So I've been making all changes, bug fixes and additions to this generated code. Few of my changes were not too big and with the lint rules I don't really care about the code style as it will probably be deleted soon. But now I'm at a stage where I genuinely wish I'd started this whole thing from scratch.
The over eagerness to solve for edge cases seems to be the primary motivation for this code. The main feature remains incomplete. And then I hit the Maximum stack exceeded error and knew I had been screwed over by this code. Something like that typically warrants unnecessary debounces or a complete overhaul of code. 

So, next I'm kind of working on maintaining a document with all the instructions for developing a new feature. It's been a similar kind of frustration. It has made deep errors that will require a lot of untangling and has basically created legacy code from the get go. In a classic case of sunken cost fallacy, I've been manually sorting and restructuring this code myself. I don't presume to have a better brain than the hive mind of copilot. So I'll accept its code and grumble over it just as if it were my code, except my code would have been shorter, would have hit the brief perfectly, would be testing the core feature, would have as less number of new lines added as possible. *crying emoji*