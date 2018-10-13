// TODO table of content

# Definition
"Service-oriented architecture composed of loosely coupled elements that have
bounded contexts" by Adrian Cockcroft (Amazon)

"[Conway's Law states that] Organizations that design systems are constrained to produce copies of the communication structures of these organizations [...] the organization chart will initially reflect the first system design, which is almost surely not the right one [...] as one learns, he changes the design [...]. Management structures also need to be changed as the system changes..."

https://martinfowler.com/articles/microservices.html
http://www.neverletdown.net/2015/05/introduction-to-microservices.html
https://www.slideshare.net/adriancockcroft/dockercon-state-of-the-art-in-microservices

# Monoliths vs Microservices

## Monoliths Advantages 
* A single (layered) architecture 
* A single technology stack 
* A single code base maintained by multiple teams 

## Monoliths Disadvantages 
* All parts are interconnected 
* Many other systems are connected to your system 
* Hard to change, hard to maintain 
* Long time between releases, thereby increasing risks  Slow innovation 
* Hard to move to newer technologies 
* Doesn’t scale very well 

## Microservices Promises
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

## Microservices. But… 
* What is a microservice exactly? 
* How small is a microservice? https://youtu.be/YQp85GzoxqA?t=2m48s
* Requirements in a microservice world 
* Components or services 
* Who owns a microservice? 
* What technologies do you use? 
* What protocols do you apply? 
* How to define messages 
* How to test microservices 
* How to coordinate when business services run across components? 
* How to build deployment pipelines?

https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell
https://martinfowler.com/articles/microservice-trade-offs.html
https://martinfowler.com/bliki/MicroservicePrerequisites.html
https://martinfowler.com/bliki/MonolithFirst.html

* https://github.com/mfornos/awesome-microservices
* https://github.com/theanalyst/awesome-distributed-systems
- https://youtu.be/YQp85GzoxqA?t=2m48s  Microservices - the naked truth of the maintainability
- https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell
- http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf
- https://martinfowler.com/articles/microservices.html
- https://martinfowler.com/articles/microservice-trade-offs.html
- https://www.youtube.com/watch?v=JXEjAwNWays Golang UK Conference 2016 - Peter Bourgon - Go + Microservices = Go Kit
- https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing
- https://www.youtube.com/watch?v=yxZm0Fhn9Tk  Microservices architecture pitfalls
- https://martinfowler.com/bliki/MicroservicePrerequisites.html
- http://callistaenterprise.se/blogg/teknik/2015/05/20/blog-series-building-microservices/
- https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/
- https://12factor.net
- https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/
- https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it
- https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework
- https://gist.github.com/staltz/868e7e9bc2a7b8c1f754  The introduction to Reactive Programming you've been missing
- https://www.youtube.com/watch?v=QfpCF_Eo4V0  Asynchronous by default, synchronous when necessary
- https://www.reactivemanifesto.org/
- https://thenewstack.io/succeed-failure-microservices/
- https://gist.github.com/chitchcock/1281611
- https://plus.google.com/+RipRowan/posts/eVeouesvaVX
- https://www.nginx.com/blog/service-discovery-in-a-microservices-architecture/
- http://opensourceconnections.com/blog/2015/06/25/why-cassandra/
- http://guide.couchdb.org/draft/consistency.html
- https://plus.google.com/+RipRowan/posts/eVeouesvaVX
- https://martinfowler.com/eaaDev/EventSourcing.html
- https://dzone.com/articles/failure-mongodb-bitcoin
- https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/
- https://thehftguy.com/2017/02/23/docker-in-production-an-update/
- https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f
- https://jakubn.gitlab.io/keepitclean/#1
- http://tidyjava.com/hexagonal-architecture-powerful/
- http://www.javapractices.com/topic/TopicAction.do?Id=205
- https://martinfowler.com/bliki/MonolithFirst.html
- http://microservices.io/patterns/apigateway.html
- https://vimeo.com/233798451  HTTP clients: silent heroes of distributed systems
- https://content.pivotal.io/blog/should-that-be-a-microservice-part-4-independent-scalability
- https://speakerdeck.com/wendigo/jdd-dlug-techniczny
- Microservices architecture pitfalls https://youtu.be/yxZm0Fhn9Tk (polish)
- 4lata rewolucji mikrousługowej https://youtu.be/_X89vxbuExE (polish)
- Microservices https://youtu.be/GPj_KuWB7xA (polish)
- Building distributed systems with OSS https://youtu.be/_2VuUr-LgLw (polish)
- Scaling apps on local DC and cloud https://youtu.be/uSeaJcShLZk (polish)
- A Hitchhiker's Guide to the Functional Exception Handling in Java https://www.youtube.com/watch?v=Fxyezv_a0Fk (polish)
- https://allegro.tech/2016/03/Managing-Frontend-in-the-microservices-architecture.html
- https://www.mosaic9.org/
- https://www.slideshare.net/adriancockcroft/dockercon-state-of-the-art-in-microservices
- https://youtu.be/YQp85GzoxqA?t=2m48s
- https://www.slideshare.net/aahoogendoorn/designing-and-building-a-microservices-architecture-stairway-to-heaven-or-a-highway-to-hell
- http://www.infoq.com/resource/minibooks/domain-driven-design-quickly/en/pdf/DomainDrivenDesignQuicklyOnline.pdf
- https://martinfowler.com/articles/microservices.html- https://www.youtube.com/watch?v=JXEjAwNWays
- https://en.wikipedia.org/wiki/Fallacies_of_distributed_computing
- https://www.youtube.com/watch?v=yxZm0Fhn9Tk
- https://martinfowler.com/bliki/MicroservicePrerequisites.html
- https://developers.redhat.com/blog/2016/12/09/spring-cloud-for-microservices-compared-to-kubernetes/
- https://12factor.net
- https://blog.codecentric.de/en/2016/04/event-driven-microservices-spring-cloud-stream/
- https://techbeacon.com/what-apache-kafka-why-it-so-popular-should-you-use-it
- https://github.com/vaquarkhan/vaquarkhan/wiki/CQRS-and-Event-Sourcing-in-Java-with-Spring-Framework
- https://gist.github.com/staltz/868e7e9bc2a7b8c1f754- https://www.youtube.com/watch?v=QfpCF_Eo4V0
- https://www.reactivemanifesto.org/
- https://thenewstack.io/succeed-failure-microservices/
- https://www.nginx.com/blog/service-discovery-in-a-microservices-architecture/
- http://opensourceconnections.com/blog/2015/06/25/why-cassandra/
- http://guide.couchdb.org/draft/consistency.html
- https://plus.google.com/+RipRowan/posts/eVeouesvaVX
- https://martinfowler.com/eaaDev/EventSourcing.html
- https://dzone.com/articles/failure-mongodb-bitcoin
- https://thehftguy.com/2016/11/01/docker-in-production-an-history-of-failure/
- https://thehftguy.com/2017/02/23/docker-in-production-an-update/
- https://blog.pragmatists.com/refactoring-from-anemic-model-to-ddd-880d3dd3d45f
- https://jakubn.gitlab.io/keepitclean/#1
- http://tidyjava.com/hexagonal-architecture-powerful/
- http://www.javapractices.com/topic/TopicAction.do?Id=205
- https://martinfowler.com/bliki/MonolithFirst.html
- http://microservices.io/patterns/apigateway.html
- https://vimeo.com/233798451https://speakerdeck.com/wendigo/jdd-dlug-techniczny
- https://threedots.tech/post/microservices-or-monolith-its-detail/
- http://www.dwmkerr.com/the-death-of-microservice-madness-in-2018/
