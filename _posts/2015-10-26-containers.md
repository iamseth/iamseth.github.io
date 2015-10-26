---
layout: post
title: Containers and the Unix way
---

Well, I’m finally getting around to starting this blog and what better way than with a post on containers? Every tech focused blog blog ought to have at least one article on the subject.

I’m a big fan of containers and specifically the Docker project. Containerization is a fantastic idea and we’re going to see a lot more of it in the next 2-5 years. There’s a lot if dislike for containers but I think that comes from a misunderstanding of where they excel.

To really understand what containers are for we should look at real world containers. I’m talking about the CONEX shipping containers used to move goods around the world.

Before containers, longshoremen would have to handle cargo in all sorts of non-standard formats. Someone working the docks may have to move boxes, sacks, barrels, cars, pallets, or even bare items like racks of bananas.

It’s easy to see how moving to a standard size and maximum allowed weight would dramatically improve efficiency. With containers longshoremen needn’t handle grapefruit any differently from cars or rice. It’s all standardized.

OK, now back to the technical kind of container. A common gripe with containers is that we’re regressing to the golden image. If you lose the build instructions or were never given any, you’ll have to reverse engineer the damn thing. I’ve had to reverse engineer VMware templates and Amazon AMI and it’s a nightmare.

The proper use of containers is to standardize shipping. That’s it. It just creates a standard interface for dealing with an application during deployment. Handling dependencies and build procedures should be handled elsewhere. Probably using some form of configuration management and/or build tool.

Now operations doesn’t care if you’re shipping a Tomcat application or something in Rails. Ops can be made dumber or non-existent for deployment just like longshoremen have mostly been replaced by robots. It would have been too difficult to get robots to handle items like bananas, sacks of rice and cars without containers.

If you’re only shipping the same application over and over, containers don’t make sense. Any operations or development team can script a deployment and be done with it.

Containers start making sense when you’re deploying dozens of different applications. It would be expensive to cope with so much variety. Containers wrap the complexity in a simple, standard interface just like CONEX containers. They don’t solve all problems, just one problem well. The Unix way.
