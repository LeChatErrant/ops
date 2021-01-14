# Ops

> The generic distributed Cloud-computing platform


### ABANDONED - This project is currently stopped and unmaintained


## Why Ops?

> First of all, hello. I'm [LeChatErrant](https://github.com/LeChatErrant) a young software engineer studying at Epitech Paris, creator and maintainer of [Ops](https://github.com/LeChatErrant/ops)
>
> I'm currently working at [Tresorio](https://tresorio.com/), a green cloud-computing startup, at the position of lead-developer of the cloud-rendering branch (distributed computing for 3D animation)
>
> Passionated by the design of distributed systems and their challenges, I'm aiming to offer tools to help building a complete cloud-computing platform, whatever your usecase is

Let's say you have machines. A bunch of machines. And you want to sell some services on it : *AI trainings*, *video processing*, or any *resource consuming task*

Or maybe would you like to let people do what they want with those resources, letting them launching *custom containers* or running *VPS* (Virtual Private Servers)

Perhaps you don't have machines, but you have found a whole new *usecase of distributed computing*, of course with a super robust buisness model, and you would like to build a platform for this usecase using cloud providers



**But the question is, how are you going to build your platform, to let access to your users to your ressources? Well, you have two solutions**

1. The time/money consuming one. Hire developers. Build your platform from scratch, make errors that other have already made, refactor your infrastructure as many times as your usecase changes, maintain it and face scaling problems, requiring more experienced developers (and more refactor, and more time, and more money). It's an adventure, but I swear it's a good one!
2. Use **Ops**. Focus only on what you offer on your machines, not on how!



## What is Ops?

Ops is an open-source cloud-computing platform

It aims to respond to only one challenge : you have *machines* and you want to offer *services* on it

Ops purpose is to unify all your machines into a single infrastructure and to provide a core API to launch the tasks that **YOU** define. It can be seen as an engine responsible of the cloud-computing logic, where the only thing you have to code are the tasks you want to propose and the logic around it

Ops is composed of multiples *parts*. Each parts purpose aims to be used **separatly**
> e.g. You are not interested at all in the Ops project, but need monitoring to be installed in your Kubernetes cluster? You can use [03_monitoring](/03_monitoring), regardless of the rest of the project

The project provides
 * Servers provisionning from multi cloud providers
 * A way to setup an healthy minimal kubernetes cluster and to maintain it
 * Various Monitoring tools
 * Distributed database
 * Scalable core wrapping the kubernetes API. It includes features such as:
   * Launching of parametrized tasks
   * Compartmentalization of tasks resources, with GPU supported
   * Event-based logic around task lifecycle
   * Storage of tasks history and miscellaneous datas (usefull for users or payment logic)
 * Storage system
 * Payment core
 * Chaotic engineering integration
 * Automated unused resources management (for example, let your unused GPUs be used by [folding@home](https://foldingathome.org/))
 * Environment segmentation (e.g. to allocate a part of your infrastructure for staging)
 * *And there is more to come !*



## Ops guidelines

 - **Open-sourcing** Ops code should be totally transparent and contributions from all developpers should always be welcome
 - **Simplicity** Ops should be simple to apprehend, deploy, maintain and substitute
 - **Scalability** Ops should be performant on large size infrastructure and in stressfull environment
 - **Composability** Every Ops part should be replaceable and removable. Ops parts should all be independants and it should always be possible to use it as separate projects.
 - **Configuration** Ops should be easily configurable. It should be done without any code modification into Ops core
 - **Usecase agnosticity** Ops should provide way to launch tasks and to define logic around their lifecycles, regardless of what the task is
 - **Isolation** Ops should not interfer in any case with external components and easily cohabit with other systems. A micro-service architecture should be used, with a distinct separation of concerns and segmentation of logic, and all good patterns favourable to distributed systems should be used.
 - **Event-base programming** Logic around Ops tasks should only be triggered by the way of events (such as container death, outputs file creation and so on), to force the use of serverless functions around task lifecycle

Those guidelines aim to keep Ops **production ready**



## Ops design and topology
> Coming soon



## Contributions

All contributions are welcome!

This is a huge project, and the knowledge of everyone is needed. Even if it's just to send tips or discuss about the general architecture, don't hesitate to post issues!


To contribute:
1. Fork it (<https://github.com/LeChatErrant/ops/fork>)
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request



### Contributors

![GitHub Logo](https://github.com/LeChatErrant.png?size=30) &nbsp; [LeChatErrant](https://github.com/LeChatErrant) - creator and maintainer
