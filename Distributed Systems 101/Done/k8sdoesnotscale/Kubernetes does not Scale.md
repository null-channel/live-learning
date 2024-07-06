So you want to scale? But do you know what that even means? To often I hear people talk about the scale of kubernetes and so often I physically cringe when I hear this type of statement as I fear it means people have no idea what problem they are trying to solve.

we are engineers. understanding the problem we need to solve is our top priority.

Let me be clear.

Kubernetes does NOT let you scale your application. It does not fix a bad architecture and it will not enable you to handle more transactions, more throughput or any other metric. 

Scalling your application is a part of your applications architecture, kubernetes or not. Any application that runs in kubernetes could run in a different environment, including bare metal. I actually mean that. now you might argue that your application would be difficult to manage in another environment because you designed it to run nicely in kubernetes. and that is fine. But it could run on bare metal, ec2 or friking raspbery pies... or even somewhere else.

I know. you are about to stop me and say microservices enable you to scale. and i'm going to stop you before you make a fool of yourself. Microservices do NOT enable you to scale. I mean it.

This actually annoys me a lot as it means there are a lot of engineers that don't understand the problem microservices solve, but I already made a video on that, go check it out.

The only thing you CAN say with regards to is that microservices and scaling is that it enables you to scale individuates chucks of code more granularity... but i'm going to actually successfully show you this could hurt your scaling performance... especially with small code bases. So don't count this as a win.

Anyhow. I love kubernetes. I just want people to use it because it solves the problem they have. Not that it creates problems they did not have.