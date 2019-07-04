# Microservices

## Definition

"Service-oriented architecture composed of loosely coupled elements that have bounded contexts" by Adrian Cockcroft \(Amazon\)

"Conway's Law states that Organizations that design systems are constrained to produce copies of the communication structures of these organizations \[...\] the organization chart will initially reflect the first system design, which is almost surely not the right one \[...\] as one learns, he changes the design \[...\]. Management structures also need to be changed as the system changes..."

* [https://martinfowler.com/bliki/MicroservicePrerequisites.html](https://martinfowler.com/bliki/MicroservicePrerequisites.html) 
* [https://martinfowler.com/articles/microservices.html](https://martinfowler.com/articles/microservices.html) 
* [https://martinfowler.com/microservices/](https://martinfowler.com/microservices/)
* [https://martinfowler.com/articles/microservice-trade-offs.html](https://martinfowler.com/articles/microservice-trade-offs.html) 
* [https://martinfowler.com/articles/break-monolith-into-microservices.html](https://martinfowler.com/articles/break-monolith-into-microservices.html) 
* [https://martinfowler.com/bliki/MonolithFirst.html](https://martinfowler.com/bliki/MonolithFirst.html)
* [http://www.neverletdown.net/2015/05/introduction-to-microservices.html](http://www.neverletdown.net/2015/05/introduction-to-microservices.html)
* [https://www.slideshare.net/adriancockcroft/dockercon-state-of-the-art-in-microservices](https://www.slideshare.net/adriancockcroft/dockercon-state-of-the-art-in-microservices)
* [https://github.com/mfornos/awesome-microservices\#theory](https://github.com/mfornos/awesome-microservices#theory)
* [https://github.com/theanalyst/awesome-distributed-systems](https://github.com/theanalyst/awesome-distributed-systems)
* [https://www.infoq.com/presentations/google-microservices](https://www.infoq.com/presentations/google-microservices)
* Book: Martin Kleppmann, Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems

## Monoliths vs Microservices

### Monoliths Advantages

* A single \(layered\) architecture 
* A single technology stack 
* A single code base maintained by multiple teams 

### Monoliths Disadvantages

* All parts are interconnected 
* Many other systems are connected to your system 
* Hard to change, hard to maintain 
* Long time between releases, thereby increasing risks 
* Slow innovation 
* Hard to move to newer technologies 
* Doesn’t scale very well 

### Microservices Promises

* Products not projects 
* Scalable 
* Decentralized governance 
* Replaceable parts 
* High performance 
* Technology independent 
* Polyglot persistence 
* Easy to build 
* Easy to test 
* Easier deployment than monoliths Product Account Order Customer

### Microservices. But…

* What is a microservice exactly? 
* How small is a microservice? [https://youtu.be/YQp85GzoxqA?t=2m48s](https://youtu.be/YQp85GzoxqA?t=2m48s)
* Requirements in a microservice world 
* Components or services 
* Who owns a microservice? 
* What technologies do you use? 
* What protocols do you apply? 
* How to define messages 
* How to test microservices 
* How to coordinate when business services run across components? 
* How to build deployment pipelines?

References:

* [https://www.martinfowler.com/microservices/\#when](https://www.martinfowler.com/microservices/#when)
* [https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell](https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell)
* [https://martinfowler.com/articles/microservice-trade-offs.html](https://martinfowler.com/articles/microservice-trade-offs.html)
* [https://martinfowler.com/bliki/MicroservicePrerequisites.html](https://martinfowler.com/bliki/MicroservicePrerequisites.html)
* [https://martinfowler.com/bliki/MonolithFirst.html](https://martinfowler.com/bliki/MonolithFirst.html)
* [https://thenewstack.io/ten-commandments-microservices/](https://thenewstack.io/ten-commandments-microservices/)
* [https://threedots.tech/post/microservices-or-monolith-its-detail/](https://threedots.tech/post/microservices-or-monolith-its-detail/)

## Breaking the Monolith

* [https://martinfowler.com/articles/break-monolith-into-microservices.html](https://martinfowler.com/articles/break-monolith-into-microservices.html)
* [https://www.nginx.com/blog/refactoring-a-monolith-into-microservices/](https://www.nginx.com/blog/refactoring-a-monolith-into-microservices/)
* [https://www.dynatrace.com/news/blog/breaking-the-monolith-an-8-step-recipe/](https://www.dynatrace.com/news/blog/breaking-the-monolith-an-8-step-recipe/)
* [https://www.dynatrace.com/news/blog/fearless-monolith-to-microservices-migration-a-guided-journey/](https://www.dynatrace.com/news/blog/fearless-monolith-to-microservices-migration-a-guided-journey/)
* [https://techbeacon.com/how-break-apart-monolith-without-destroying-your-team](https://techbeacon.com/how-break-apart-monolith-without-destroying-your-team)
* [https://medium.com/weebly-engineering/how-to-organize-your-monolith-before-breaking-it-into-services-69cbdb9248b0](https://medium.com/weebly-engineering/how-to-organize-your-monolith-before-breaking-it-into-services-69cbdb9248b0)
* [https://www.appcelerator.com/blog/2018/01/5-strategies-for-making-the-switch-from-monolith-to-microservices/](https://www.appcelerator.com/blog/2018/01/5-strategies-for-making-the-switch-from-monolith-to-microservices/)
* [http://enos.itcollege.ee/~jpoial/allalaadimised/reading/microservicesguide-2017.pdf](http://enos.itcollege.ee/~jpoial/allalaadimised/reading/microservicesguide-2017.pdf)

## Fallacies of distributed computing

The fallacies of distributed computing are a set of assertions made by L Peter Deutsch and others at Sun Microsystems describing false assumptions that programmers new to distributed applications invariably make.

### The fallacies

"Essentially everyone, when they first build a distributed application, makes the following eight assumptions. All prove to be false in the long run and all cause big trouble and painful learning experiences." by Peter Deutsch 

1. The network is reliable. 
2. Latency is zero. 
3. Bandwidth is infinite. 
4. The network is secure. 
5. Topology doesn't change. 
6. There is one administrator. 
7. Transport cost is zero. 
8. The network is homogeneous. So a design is bad if one these aspects is neglected.

### The effects of the fallacies

* Software applications are written with little error-handling on networking errors. During a network outage, such applications may stall or infinitely wait for an answer packet, permanently consuming memory or other resources. When the failed network becomes available, those applications may also fail to retry any stalled operations or require a \(manual\) restart.
* Ignorance of network latency, and of the packet loss it can cause, induces application- and transport-layer developers to allow unbounded traffic, greatly increasing dropped packets and wasting bandwidth.
* Ignorance of bandwidth limits on the part of traffic senders can result in bottlenecks.
* Complacency regarding network security results in being blindsided by malicious users and programs that continually adapt to security measures.
* Changes in network topology can have effects on both bandwidth and latency issues, and therefore can have similar problems.
* Multiple administrators, as with subnets for rival companies, may institute conflicting policies of which senders of network traffic must be aware in order to complete their desired paths.
* The "hidden" costs of building and maintaining a network or subnet are non-negligible and must consequently be noted in budgets to avoid vast shortfalls.
* If a system assumes a homogeneous network, then it can lead to the same problems that result from the first three fallacies.

References:

* [https://en.wikipedia.org/wiki/Fallacies\_of\_distributed\_computing](https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing)
* [http://principles-wiki.net/principles:fallacies\_of\_distributed\_computing](http://principles-wiki.net/principles:fallacies_of_distributed_computing)
* [https://www.youtube.com/watch?v=yxZm0Fhn9Tk](https://www.youtube.com/watch?v=yxZm0Fhn9Tk)

## Microservices Concerns

* Config Management
* Service Discovery & LB
* Resilience & Fault Tolerance
* Api Management
* Service Security
* Centralized Logging
* Distributed Tracing
* Scheduling & Deployment
* Auto Scaling & Self Healing
* Service Mesh

References:

* [https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/](https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/)
* [https://12factor.net](https://12factor.net)
* [https://dzone.com/articles/what-are-concerns-about-microservices](https://dzone.com/articles/what-are-concerns-about-microservices)
* [https://martinfowler.com/articles/microservice-trade-offs.html](https://martinfowler.com/articles/microservice-trade-offs.html)
* [https://www.martinfowler.com/microservices/\#when](https://www.martinfowler.com/microservices/#when)
* [https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell](https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell)
* [https://martinfowler.com/articles/microservice-trade-offs.html](https://martinfowler.com/articles/microservice-trade-offs.html)
* [https://martinfowler.com/bliki/MicroservicePrerequisites.html](https://martinfowler.com/bliki/MicroservicePrerequisites.html)
* [https://martinfowler.com/bliki/MonolithFirst.html](https://martinfowler.com/bliki/MonolithFirst.html)
* [https://dwmkerr.com/the-death-of-microservice-madness-in-2018/](https://dwmkerr.com/the-death-of-microservice-madness-in-2018/)
* [https://www.infoq.com/articles/seven-uservices-antipatterns](https://www.infoq.com/articles/seven-uservices-antipatterns)
* [https://stackify.com/communication-microservices-avoid-common-problems/](https://stackify.com/communication-microservices-avoid-common-problems/)
* [https://www.oreilly.com/library/view/microservices-antipatterns-and/9781492042716/](https://www.oreilly.com/library/view/microservices-antipatterns-and/9781492042716/)
* [Microservices in the Cloud with Kubernetes and Istio \(Google I/O '18\)](https://youtu.be/gauOI0O9fRM)

## The 10 commandements of Microservices

1. Clean Separation of Stateless and Stateful Services
2. Do Not Share Libraries or SDKs \(Dependencies will kill you\)
3. Avoid Host Affinity
4. Focus on Services with One Task in Mind
5. Use a Lightweight Messaging Protocol for Communication
6. Design a Well-Defined Entry Point and Exit Point
7. Implement a Self-Registration and Discovery Mechanism
8. Explicitly Check for Rules and Constraints
9. Prefer Polyglot Over Single Stack
10. Maintain Independent Revisions and Build Environments

[https://thenewstack.io/ten-commandments-microservices/](https://thenewstack.io/ten-commandments-microservices/)

## Microservices and Teams

\(Again\) "Conway's Law states that Organizations that design systems are constrained to produce copies of the communication structures of these organizations \[...\] the organization chart will initially reflect the first system design, which is almost surely not the right one \[...\] as one learns, he changes the design \[...\]. Management structures also need to be changed as the system changes..."

'Inverse Conway Maneuver' recommends evolving your team and organizational structure to promote your desired architecture. Ideally your technology architecture will display isomorphism with your business architecture. [https://www.thoughtworks.com/radar/techniques/inverse-conway-maneuver](https://www.thoughtworks.com/radar/techniques/inverse-conway-maneuver)

* [https://martinfowler.com/articles/microservices.html\#OrganizedAroundBusinessCapabilities](https://martinfowler.com/articles/microservices.html#OrganizedAroundBusinessCapabilities)
* [https://www.nginx.com/blog/adopting-microservices-at-netflix-lessons-for-team-and-process-design/](https://www.nginx.com/blog/adopting-microservices-at-netflix-lessons-for-team-and-process-design/)
* [https://techbeacon.com/want-develop-great-microservices-reorganize-your-team](https://techbeacon.com/want-develop-great-microservices-reorganize-your-team)
* [https://dzone.com/articles/microservices-and-team-organization](https://dzone.com/articles/microservices-and-team-organization)
* [https://opensource.com/article/18/8/microservices-team-challenges](https://opensource.com/article/18/8/microservices-team-challenges)
* [https://www.slideshare.net/ConfluentInc/microservices-in-the-apache-kafka-ecosystem](https://www.slideshare.net/ConfluentInc/microservices-in-the-apache-kafka-ecosystem)

## Microservices should be organized around Business Capabilities and Domain

* [https://martinfowler.com/articles/microservices.html\#OrganizedAroundBusinessCapabilities](https://martinfowler.com/articles/microservices.html#OrganizedAroundBusinessCapabilities)
* [https://martinfowler.com/bliki/BoundedContext.html](https://martinfowler.com/bliki/BoundedContext.html)
* [https://docs.microsoft.com/en-us/dotnet/standard/microservices-architecture/microservice-ddd-cqrs-patterns/ddd-oriented-microservice](https://docs.microsoft.com/en-us/dotnet/standard/microservices-architecture/microservice-ddd-cqrs-patterns/ddd-oriented-microservice)
* [http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf](http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf)
* [https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f](https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f)
* [https://jakubn.gitlab.io/keepitclean/\#1](https://jakubn.gitlab.io/keepitclean/#1)
* [http://tidyjava.com/hexagonal-architecture-powerful/](http://tidyjava.com/hexagonal-architecture-powerful/)

## Reactive Programming and Microservices

Reactive Systems are:

* Responsive
* Resilient
* Elastic
* Message Driven

"The driver is efficient resource utilization, or in other words, spending less money on servers and data centres. The promise of Reactive is that you can do more with less, specifically you can process higher loads with fewer threads. This is where the intersection of Reactive and non-blocking, asynchronous I/O comes to the foreground."

"The Reactive Essence of a Microservice. Asynchronous Communication, Isolation, Autonomicity, Single Responsibility, Exclusive State, and Mobility. These are the core traits of Microservices." by Jonas Boner

* [https://www.reactivemanifesto.org/](https://www.reactivemanifesto.org/)
* [http://heidloff.net/article/introduction-reactive-microservices](http://heidloff.net/article/introduction-reactive-microservices)
* [https://www.oreilly.com/ideas/what-is-a-reactive-microservice](https://www.oreilly.com/ideas/what-is-a-reactive-microservice)
* [https://gist.github.com/staltz/868e7e9bc2a7b8c1f754](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754) - The introduction to Reactive Programming you've been missing
* [https://spring.io/blog/2016/06/07/notes-on-reactive-programming-part-i-the-reactive-landscape](https://spring.io/blog/2016/06/07/notes-on-reactive-programming-part-i-the-reactive-landscape)
* [http://rxmarbles.com/](http://rxmarbles.com/)
* [https://vimeo.com/233798451](https://vimeo.com/233798451) - HTTP clients: silent heroes of distributed systems
* [https://www.youtube.com/watch?v=QfpCF\_Eo4V0](https://www.youtube.com/watch?v=QfpCF_Eo4V0) - Asynchronous by default, synchronous when necessary
* [http://jonasboner.com/bla-bla-microservices-bla-bla/](http://jonasboner.com/bla-bla-microservices-bla-bla/)

## Microservices solve organizational problems and cause technical problems

From Go + Microservices = Go Kit \[I\] - Peter Bourgon, Go Kit  
[https://youtu.be/NX0sHF8ZZgw?t=729](https://youtu.be/NX0sHF8ZZgw?t=729)

## Problems solved, Problems caused, Lessons learned

inspired by "Peter Bourgon - Go + Microservices = Go Kit" [https://www.youtube.com/watch?v=JXEjAwNWays](https://www.youtube.com/watch?v=JXEjAwNWays)

### Problems solved

* Team is too large to work effectively on shared codebase
* Teams are blocked on other teams — can't make progress
* Communication overhead too large
* Velocity stalled
* Gives more freedom about technology and ability to replace it
* Teams in different timezones
* Scalability and some technical issues

### Problems caused

* Need well-defined business domains for stable APIs
* How to make it decoupled?
* No more shared DB — distributed transactions?
* Testing becomes really hard \(chaos monkey anyone?\)
* Require dev/ops culture: devs deploy & operate their work
* Job \(service\) scheduling — manually works, for a while…
* Addressability i.e. service discovery
* Monitoring and instrumentation — tail -f? Nagios & New Relic?
* Distributed tracing?
* Your SLA?
* Audits?
* Production database snapshots
* Code reuse

### Lessons learned

* Distributed systems are hard to do
* Evolutionary architecture!
* Microservices are changing organisations
* Devops/SysOps skill required, High level automation needed
* Just another level of complexity
* Always check if your framework solved your problem, already
* Code reuse might be hard \(or you just don’t want to do this\)
* Async communication / Event sourcing may help with decoupling
* Config / Discovery should exist from day one?
* One team per microservice?
* Think twice before going Micro
* Micro solves organisation problems, causing technical ones
* Hard to manage Micro when business requirements are unknown, where are correct split lines?
* Using Open Source Software is the way to go ?
* Don’t start with microservices ? Monolith First, Microservices later
* Software Houses - not sure if they possible to do such thing - time to market?
* One team and microservices? - Nope.
* It is easy to create distributed monolith
* ‘distributed’ tools by default are hard too
* Designed for failure

With bad decisions you can develop: "Distributed Monolithic Applications: a monolithic application disguised as a collection of microservices, stitched together using JSON, simultaneously writing to a single database" by Kelsey Hightower

References

* [https://www.youtube.com/watch?v=JXEjAwNWays](https://www.youtube.com/watch?v=JXEjAwNWays)
* [https://martinfowler.com/bliki/MonolithFirst.html](https://martinfowler.com/bliki/MonolithFirst.html)

## Internal communication and REST vs messaging

"Communication between Microservices needs to be based on Asynchronous Message-Passing \(while the logic inside each Microservice is performed in a synchronous fashion\). As was mentioned earlier, an asynchronous boundary between services is necessary in order to decouple them, and their communication flow, in time—allowing concurrency—and in space—allowing distribution and mobility. Without this decoupling it is impossible to reach the level of compartmentalization and containment needed for isolation and resilience.

Asynchronous and non-blocking execution and IO is often more cost-efficient through more efficient use of resources. It helps minimizing contention \(congestion\) on shared resources in the system, which is one of the biggest hurdles to scalability, low latency, and high throughput."

"It is unfortunate that synchronous HTTP is widely considered as the go-to Microservice communication protocol. Its synchronous nature introduces strong coupling between services which makes it a very bad default protocol for inter-service communication." by Jonas Boner

* [https://dev.to/matteojoliveau/microservices-communications-why-you-should-switch-to-message-queues--48ia](https://dev.to/matteojoliveau/microservices-communications-why-you-should-switch-to-message-queues--48ia)
* [http://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying](http://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying)
* [https://www.oreilly.com/ideas/what-is-a-reactive-microservice](https://www.oreilly.com/ideas/what-is-a-reactive-microservice)
* [https://solace.com/blog/products-tech/experience-awesomeness-event-driven-microservices](https://solace.com/blog/products-tech/experience-awesomeness-event-driven-microservices)
* [https://solace.com/blog/messaging-between-microservices](https://solace.com/blog/messaging-between-microservices)
* [https://www.slideshare.net/ewolff/rest-vs-messaging-for-microservices](https://www.slideshare.net/ewolff/rest-vs-messaging-for-microservices)
* [https://www.slideshare.net/ConfluentInc/microservices-in-the-apache-kafka-ecosystem](https://www.slideshare.net/ConfluentInc/microservices-in-the-apache-kafka-ecosystem)
* [https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it](https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it)
* [https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework](https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework)
* [https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/](https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/)
* [https://martinfowler.com/eaaDev/EventSourcing.html](https://martinfowler.com/eaaDev/EventSourcing.html)
* [https://capgemini.github.io/architecture/is-rest-best-microservices/](https://capgemini.github.io/architecture/is-rest-best-microservices/)
* [https://softwaremill.com/mqperf/](https://softwaremill.com/mqperf/)
* [https://softwareengineering.stackexchange.com/questions/339817/should-services-talk-directly-to-each-other-in-a-microservice-architecture](https://softwareengineering.stackexchange.com/questions/339817/should-services-talk-directly-to-each-other-in-a-microservice-architecture)
* [https://container-solutions.com/argument-rest-microservices/](https://container-solutions.com/argument-rest-microservices/)
* [http://jonasboner.com/bla-bla-microservices-bla-bla/](http://jonasboner.com/bla-bla-microservices-bla-bla/)
* [https://medium.com/@diogo.lucas/communication-patterns-in-a-microservice-world-af07192b12d3](https://medium.com/@diogo.lucas/communication-patterns-in-a-microservice-world-af07192b12d3)
* [https://docs.microsoft.com/en-us/dotnet/standard/microservices-architecture/architect-microservice-container-applications/communication-in-microservice-architecture](https://docs.microsoft.com/en-us/dotnet/standard/microservices-architecture/architect-microservice-container-applications/communication-in-microservice-architecture)
* [https://github.com/dotnet/docs/blob/master/docs/standard/microservices-architecture/architect-microservice-container-applications/communication-in-microservice-architecture.md](https://github.com/dotnet/docs/blob/master/docs/standard/microservices-architecture/architect-microservice-container-applications/communication-in-microservice-architecture.md)
* [https://www.infoq.com/news/2018/03/events-distributed-systems](https://www.infoq.com/news/2018/03/events-distributed-systems)
* [https://github.com/kgoralski/personal-wiki-and-learning-resources/blob/master/kafka.md\#apache-kafka-and-microservices](https://github.com/kgoralski/personal-wiki-and-learning-resources/blob/master/kafka.md#apache-kafka-and-microservices)
* [https://www.confluent.io/solutions/microservices/](https://www.confluent.io/solutions/microservices/)
* [https://www.confluent.io/blog/building-a-microservices-ecosystem-with-kafka-streams-and-ksql/](https://www.confluent.io/blog/building-a-microservices-ecosystem-with-kafka-streams-and-ksql/)

## Microservices Antipatterns & Pitfalls



Microservices Common Mistakes:

* Wrong service boundaries - not based on business domain
* Lack of Business Alignment - microservice needs to deliver clear business value, so we need to work closely with business
* Lack of code modularity \(or lack of Common Closure Principle\)
* Shared data or shared database between services
* Sharing “common” dependencies - shared pieces of code requiring updating more than one service at once
* Forgetting about Fallacies of distributed computing
* Treating services as programming language-level modules / temporal coupling
* Forgetting about Conway’s Law & lack of clear ownership
* Cascading failures & lack of designing for Failure \(circuit breakers, retries etc.\) and flooding other services with errors
* Everything RESTful, chatty microservices and Lack of async communication
* Lack of APIs compatibility/versioning
* Lack of infrastructure/platform automation, monitoring, tracing & proper logging
* Lack of idempotency
* Lack of service discovery, api gateway and orchestration
* Trying to do everything ACID instead of BASE \(CAP Theorem\)
* Not taking care about resource utilization
* Low amount of tests and lack of acceptance tests
* Trying to do everything at once
* Microservices as the goal - they are solution for a specific problem, not a goal.
* Hype driven and too optimistic



* [http://highscalability.com/blog/2015/8/3/seven-of-the-nastiest-anti-patterns-in-microservices.html](http://highscalability.com/blog/2015/8/3/seven-of-the-nastiest-anti-patterns-in-microservices.html)
* [https://container-solutions.com/the-seven-deadly-sins-of-microservices-redux/](https://container-solutions.com/the-seven-deadly-sins-of-microservices-redux/)
* [https://www.infoq.com/articles/seven-uservices-antipatterns](https://www.infoq.com/articles/seven-uservices-antipatterns)
* [https://opencredo.com/microservices-anti-patterns-its-all-about-the-people/](https://opencredo.com/microservices-anti-patterns-its-all-about-the-people/)
* [https://blog.appdynamics.com/engineering/how-to-avoid-antipatterns-with-microservices/](https://blog.appdynamics.com/engineering/how-to-avoid-antipatterns-with-microservices/)
* [https://www.oreilly.com/library/view/microservices-antipatterns-and/9781492042716/](https://www.oreilly.com/library/view/microservices-antipatterns-and/9781492042716/)
* [https://www.infoworld.com/article/3254777/application-development/3-common-pitfalls-of-microservices-integrationand-how-to-avoid-them.html](https://www.infoworld.com/article/3254777/application-development/3-common-pitfalls-of-microservices-integrationand-how-to-avoid-them.html)
* [http://www.michaelnygard.com/blog/2017/12/the-entity-service-antipattern/](http://www.michaelnygard.com/blog/2017/12/the-entity-service-antipattern/)
* [https://enterprisersproject.com/article/2017/9/using-microservices-containers-wisely-5-pitfalls-avoid](https://enterprisersproject.com/article/2017/9/using-microservices-containers-wisely-5-pitfalls-avoid)
* [https://medium.com/walmartlabs/avoiding-pitfalls-in-microservice-architecture-ba038340f8c1](https://medium.com/walmartlabs/avoiding-pitfalls-in-microservice-architecture-ba038340f8c1)
* [http://chrisrichardson.net/post/antipatterns/2019/01/28/melbourne-microservices.html](http://chrisrichardson.net/post/antipatterns/2019/01/28/melbourne-microservices.html)
* [https://messente.com/blog/most-recent/5-mistakes-transition-to-microservices](https://messente.com/blog/most-recent/5-mistakes-transition-to-microservices)
* [https://walkingtree.tech/7-common-pitfalls-avoid-migrating-microservices/](https://walkingtree.tech/7-common-pitfalls-avoid-migrating-microservices/)
* [https://www.slideshare.net/InfoQ/microservices-antipatterns](https://www.slideshare.net/InfoQ/microservices-antipatterns)
* Pitfalls by Mateusz Gajewski [https://www.youtube.com/watch?v=yxZm0Fhn9Tk](https://www.youtube.com/watch?v=yxZm0Fhn9Tk)

## References

* [https://www.martinfowler.com/microservices](https://www.martinfowler.com/microservices)
* [https://github.com/mfornos/awesome-microservices](https://github.com/mfornos/awesome-microservices)
* [https://github.com/theanalyst/awesome-distributed-systems](https://github.com/theanalyst/awesome-distributed-systems)
* [https://www.vinaysahni.com/best-practices-for-building-a-microservice-architecture](https://www.vinaysahni.com/best-practices-for-building-a-microservice-architecture)
* [https://github.com/katopz/best-practices/blob/master/best-practices-for-building-a-microservice-architecture.md](https://github.com/katopz/best-practices/blob/master/best-practices-for-building-a-microservice-architecture.md)
* [https://youtu.be/YQp85GzoxqA?t=2m48s](https://youtu.be/YQp85GzoxqA?t=2m48s)  Microservices - the naked truth of the maintainability
* [https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell](https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell)
* [http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf](http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf)
* [https://martinfowler.com/articles/microservices.html](https://martinfowler.com/articles/microservices.html)
* [https://martinfowler.com/articles/microservice-trade-offs.html](https://martinfowler.com/articles/microservice-trade-offs.html)
* [https://www.youtube.com/watch?v=JXEjAwNWays](https://www.youtube.com/watch?v=JXEjAwNWays) Golang UK Conference 2016 - Peter Bourgon - Go + Microservices = Go Kit
* [https://en.wikipedia.org/wiki/Fallacies\_of\_distributed\_computing](https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing)
* [https://www.youtube.com/watch?v=yxZm0Fhn9Tk](https://www.youtube.com/watch?v=yxZm0Fhn9Tk)  Microservices architecture pitfalls
* [https://martinfowler.com/bliki/MicroservicePrerequisites.html](https://martinfowler.com/bliki/MicroservicePrerequisites.html)
* [http://callistaenterprise.se/blogg/teknik/2015/05/20/blog-series-building-microservices/](http://callistaenterprise.se/blogg/teknik/2015/05/20/blog-series-building-microservices/)
* [https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/](https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/)
* [https://12factor.net](https://12factor.net)
* [https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/](https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/)
* [https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it](https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it)
* [https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework](https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework)
* [https://gist.github.com/staltz/868e7e9bc2a7b8c1f754](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754)  The introduction to Reactive Programming you've been missing
* [https://www.youtube.com/watch?v=QfpCF\_Eo4V0](https://www.youtube.com/watch?v=QfpCF_Eo4V0)  Asynchronous by default, synchronous when necessary
* [https://www.reactivemanifesto.org/](https://www.reactivemanifesto.org/)
* [https://thenewstack.io/succeed-failure-microservices/](https://thenewstack.io/succeed-failure-microservices/)
* [https://gist.github.com/chitchcock/1281611](https://gist.github.com/chitchcock/1281611)
* [https://plus.google.com/+RipRowan/posts/eVeouesvaVX](https://plus.google.com/+RipRowan/posts/eVeouesvaVX)
* [https://www.nginx.com/blog/service-discovery-in-a-microservices-architecture/](https://www.nginx.com/blog/service-discovery-in-a-microservices-architecture/)
* [http://opensourceconnections.com/blog/2015/06/25/why-cassandra/](http://opensourceconnections.com/blog/2015/06/25/why-cassandra/)
* [http://guide.couchdb.org/draft/consistency.html](http://guide.couchdb.org/draft/consistency.html)
* [https://plus.google.com/+RipRowan/posts/eVeouesvaVX](https://plus.google.com/+RipRowan/posts/eVeouesvaVX)
* [https://martinfowler.com/eaaDev/EventSourcing.html](https://martinfowler.com/eaaDev/EventSourcing.html)
* [https://dzone.com/articles/failure-mongodb-bitcoin](https://dzone.com/articles/failure-mongodb-bitcoin)
* [https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/](https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/)
* [https://thehftguy.com/2017/02/23/docker-in-production-an-update/](https://thehftguy.com/2017/02/23/docker-in-production-an-update/)
* [https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f](https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f)
* [https://jakubn.gitlab.io/keepitclean/\#1](https://jakubn.gitlab.io/keepitclean/#1)
* [http://tidyjava.com/hexagonal-architecture-powerful/](http://tidyjava.com/hexagonal-architecture-powerful/)
* [http://www.javapractices.com/topic/TopicAction.do?Id=205](http://www.javapractices.com/topic/TopicAction.do?Id=205)
* [https://martinfowler.com/bliki/MonolithFirst.html](https://martinfowler.com/bliki/MonolithFirst.html)
* [http://microservices.io/patterns/apigateway.html](http://microservices.io/patterns/apigateway.html)
* [https://vimeo.com/233798451](https://vimeo.com/233798451)  HTTP clients: silent heroes of distributed systems
* [https://content.pivotal.io/blog/should-that-be-a-microservice-part-4-independent-scalability](https://content.pivotal.io/blog/should-that-be-a-microservice-part-4-independent-scalability)
* [https://speakerdeck.com/wendigo/jdd-dlug-techniczny](https://speakerdeck.com/wendigo/jdd-dlug-techniczny)
* Microservices architecture pitfalls [https://youtu.be/yxZm0Fhn9Tk](https://youtu.be/yxZm0Fhn9Tk) \(polish\)
* 4lata rewolucji mikrousługowej [https://youtu.be/\_X89vxbuExE](https://youtu.be/_X89vxbuExE) \(polish\)
* Microservices [https://youtu.be/GPj\_KuWB7xA](https://youtu.be/GPj_KuWB7xA) \(polish\)
* Building distributed systems with OSS [https://youtu.be/\_2VuUr-LgLw](https://youtu.be/_2VuUr-LgLw) \(polish\)
* Scaling apps on local DC and cloud [https://youtu.be/uSeaJcShLZk](https://youtu.be/uSeaJcShLZk) \(polish\)
* A Hitchhiker's Guide to the Functional Exception Handling in Java [https://www.youtube.com/watch?v=Fxyezv\_a0Fk](https://www.youtube.com/watch?v=Fxyezv_a0Fk) \(polish\)
* [https://allegro.tech/2016/03/Managing-Frontend-in-the-microservices-architecture.html](https://allegro.tech/2016/03/Managing-Frontend-in-the-microservices-architecture.html)
* [https://www.mosaic9.org/](https://www.mosaic9.org/)
* [https://www.slideshare.net/adriancockcroft/dockercon-state-of-the-art-in-microservices](https://www.slideshare.net/adriancockcroft/dockercon-state-of-the-art-in-microservices)
* [https://youtu.be/YQp85GzoxqA?t=2m48s](https://youtu.be/YQp85GzoxqA?t=2m48s)
* [https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell](https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell)
* [http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf](http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf)
* [https://martinfowler.com/articles/microservices.html-](https://martinfowler.com/articles/microservices.html-) [https://www.youtube.com/watch?v=JXEjAwNWays](https://www.youtube.com/watch?v=JXEjAwNWays)
* [https://en.wikipedia.org/wiki/Fallacies\_of\_distributed\_computing](https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing)
* [https://www.youtube.com/watch?v=yxZm0Fhn9Tk](https://www.youtube.com/watch?v=yxZm0Fhn9Tk)
* [https://martinfowler.com/bliki/MicroservicePrerequisites.html](https://martinfowler.com/bliki/MicroservicePrerequisites.html)
* [https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/](https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/)
* [https://12factor.net](https://12factor.net)
* [https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/](https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/)
* [https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it](https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it)
* [https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework](https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework)
* [https://gist.github.com/staltz/868e7e9bc2a7b8c1f754-](https://gist.github.com/staltz/868e7e9bc2a7b8c1f754-) [https://www.youtube.com/watch?v=QfpCF\_Eo4V0](https://www.youtube.com/watch?v=QfpCF_Eo4V0)
* [https://www.reactivemanifesto.org/](https://www.reactivemanifesto.org/)
* [https://thenewstack.io/succeed-failure-microservices/](https://thenewstack.io/succeed-failure-microservices/)
* [https://www.nginx.com/blog/service-discovery-in-a-microservices-architecture/](https://www.nginx.com/blog/service-discovery-in-a-microservices-architecture/)
* [http://opensourceconnections.com/blog/2015/06/25/why-cassandra/](http://opensourceconnections.com/blog/2015/06/25/why-cassandra/)
* [http://guide.couchdb.org/draft/consistency.html](http://guide.couchdb.org/draft/consistency.html)
* [https://plus.google.com/+RipRowan/posts/eVeouesvaVX](https://plus.google.com/+RipRowan/posts/eVeouesvaVX)
* [https://martinfowler.com/eaaDev/EventSourcing.html](https://martinfowler.com/eaaDev/EventSourcing.html)
* [https://dzone.com/articles/failure-mongodb-bitcoin](https://dzone.com/articles/failure-mongodb-bitcoin)
* [https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/](https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/)
* [https://thehftguy.com/2017/02/23/docker-in-production-an-update/](https://thehftguy.com/2017/02/23/docker-in-production-an-update/)
* [https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f](https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f)
* [https://jakubn.gitlab.io/keepitclean/\#1](https://jakubn.gitlab.io/keepitclean/#1)
* [http://tidyjava.com/hexagonal-architecture-powerful/](http://tidyjava.com/hexagonal-architecture-powerful/)
* [http://www.javapractices.com/topic/TopicAction.do?Id=205](http://www.javapractices.com/topic/TopicAction.do?Id=205)
* [https://martinfowler.com/bliki/MonolithFirst.html](https://martinfowler.com/bliki/MonolithFirst.html)
* [http://microservices.io/patterns/apigateway.html](http://microservices.io/patterns/apigateway.html)
* [https://vimeo.com/233798451https://speakerdeck.com/wendigo/jdd-dlug-techniczny](https://vimeo.com/233798451https://speakerdeck.com/wendigo/jdd-dlug-techniczny)
* [https://threedots.tech/post/microservices-or-monolith-its-detail/](https://threedots.tech/post/microservices-or-monolith-its-detail/)
* [http://www.dwmkerr.com/the-death-of-microservice-madness-in-2018/](http://www.dwmkerr.com/the-death-of-microservice-madness-in-2018/)
* [https://gist.github.com/chitchcock/1281611](https://gist.github.com/chitchcock/1281611)
* [https://plus.google.com/+RipRowan/posts/eVeouesvaVX](https://plus.google.com/+RipRowan/posts/eVeouesvaVX)

## Docker in production

* [https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/](https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/)
* [https://thehftguy.com/2017/02/23/docker-in-production-an-update/](https://thehftguy.com/2017/02/23/docker-in-production-an-update/)



