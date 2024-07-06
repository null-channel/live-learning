What problem does Infrastructures as Code solve?
 - Managing infrastructure?
 - resource management?

Questions we have to ask ourselves?

- Are there better ways to solve the problem?
- why do we have the problem? 
	- what made the problem? do bare metal deployments have this issue?
	- Is it a cloud problem? A problem involving just the clouds?
	- are there other ways to solve that problem?
	- If not, are there other ways?


## Root of the issue:
The cloud gave us the ability to arbitrarily, via code stand up infrastructure. And this is AWESOME. But it left us stagnating. 

With great power comes great responsibility.

So now we have this awesome power to programatically stand up infra. What do we do with it? Well we all collectively write and rewrite more and more code to do the same thing everyone else does. Stand up the same infra, set up the same basic auto-scaling, collect the same basic infra stats ect.

## Why?
That is what I keep asking myself.

Was not kubernetes meant to fix this for us?
- no

So I ask you? why.

This is what I want to think about when thinking about the null cloud. This sucks.

Every job I have ever had all had us rewriting the same IaC. and every job bassically was the SAME IaC code as the last job.