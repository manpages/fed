fed
===

Feature-oriented Erlang-backed Development Framework.

Q&A
===


### What is FED?

FED is a framework to rapidly develop feature-oriented applications in any programming languages any given team member is comfortable with.

### What is feature-oriented programming?

Feature-oriented programming is a way to rapidly write projects of any sort. When we implement a feature, we have it's formal description that enlists what does it provide and what features does it consume in order to work correctly.
It optionally can declare something similar to application-level protocol of interaction.

Those definitions are fed to the FED Gateway which is a part of a virtual cluster and programmer has to do little to none to receive data from the features his feature relies on — just make a request to the Gateway and let it handle the rest.

### How are the features described?

JSON. Details soon.

### How is the interaction between Gateway and feature backend is organized?

In general — JSON over some transport. Whatever way works for you. Though I want to support two transports — HTTP and UNIX pipes.

### Do I need to know Erlang in order to use FED?

No. I'm not even sure if you'll need to know how to install Erlang on your server once FED is done.

### But that kind of architecture is slow!

Indeed, having your feature implementation distributed across the servers and across the technologies will probably cause the whole project to be unstable and slow. Though as we all know, programming in particular and engineering in general is all about trade-offs. In FED we trade speed of applications for the speed of development.

The idea here is not to spend much time for the projects that aren't interesting to the people while having an opportunity to implement a [pretotype](http://www.youtube.com/watch?v=X1jWe5rOu3g) of a project. Because who could have known that Twitter will be useful for the general public.

### License?

MIT. Do whatever.
