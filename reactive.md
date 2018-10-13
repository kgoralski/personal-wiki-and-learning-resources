# Introduction

http://reactivex.io/

https://www.reactivemanifesto.org/

"Reactive programming is programming with asynchronous data streams. Reactive extensions help with async code."

"Reactive Programming is a style of micro-architecture involving intelligent routing and consumption of events, all combining to change behaviour."

Best intro https://gist.github.com/staltz/868e7e9bc2a7b8c1f754

Rx marbles for better understanding http://rxmarbles.com/


# It is nothing new
"The origins of Reactive Programming can probably be traced to the 1970s or even earlier, so there’s nothing new about the idea, but they are really resonating with something in the modern enterprise. "

# Why Now?

"What is driving the rise of Reactive in Enterprise? Well, it’s not (all) just a technology fad — people jumping on the bandwagon with the shiny new toys. The driver is efficient resource utilization, or in other words, spending less money on servers and data centres. The promise of Reactive is that you can do more with less, specifically you can process higher loads with fewer threads. This is where the intersection of Reactive and non-blocking, asynchronous I/O comes to the foreground. For the right problem, the effects are dramatic. For the wrong problem, the effects might go into reverse (you actually make things worse). Also remember, even if you pick the right problem, there is no such thing as a free lunch, and Reactive doesn’t solve the problems for you, it just gives you a toolbox that you can use to implement solutions.

Functional - Avoid intricate stateful programs, using clean input/output functions over observable streams.
Less is more - ReactiveX's operators often reduce what was once an elaborate challenge into a few lines of code.
Async error handling - Traditional try/catch is powerless for errors in asynchronous computations, but ReactiveX is equipped with proper mechanisms for handling errors.
Concurrency made easy - Observables and Schedulers in ReactiveX allow the programmer to abstract away low-level threading, synchronization, and concurrency issues."

# Implementations
http://reactivex.io/
https://github.com/ReactiveX/
http://reactivex.io/languages.html

Languages

* Java: RxJava
* JavaScript: RxJS
* C#: Rx.NET
* C#(Unity): UniRx
* Scala: RxScala
* Clojure: RxClojure
* C++: RxCpp
* Lua: RxLua
* Ruby: Rx.rb
* Python: RxPY
* Go: RxGo
* Groovy: RxGroovy
* JRuby: RxJRuby
* Kotlin: RxKotlin
* Swift: RxSwift
* PHP: RxPHP
* Elixir: reaxive
* Dart: RxDart
* ReactiveX for platforms and frameworks

* RxNetty
* RxAndroid
* RxCocoa
* Spring Project Reactor (WebFlux) https://projectreactor.io/


# Use Cases
From https://spring.io/blog/2016/06/07/notes-on-reactive-programming-part-i-the-reactive-landscape :



"The hardest question to get an answer to as a newbie seems to be "what is it good for?" Here are some examples from an enterprise setting that illustrate general patterns of use:


External Service Calls Many backend services these days are REST-ful (i.e. they operate over HTTP) so the underlying protocol is fundamentally blocking and synchronous. Not obvious territory for FRP maybe, but actually it’s quite fertile ground because the implementation of such services often involves calling other services, and then yet more services depending on the results from the first calls. With so much IO going on if you were to wait for one call to complete before sending the next request, your poor client would give up in frustration before you managed to assemble a reply. So external service calls, especially complex orchestrations of dependencies between calls, are a good thing to optimize. FRP offers the promise of "composability" of the logic driving those operations, so that it is easier to write for the developer of the calling service.


Highly Concurrent Message Consumers Message processing, in particular when it is highly concurrent, is a common enterprise use case. Reactive frameworks like to measure micro benchmarks, and brag about how many messages per second you can process in the JVM. The results are truly staggering (tens of millions of messages per second are easy to achieve), but possibly somewhat artificial - you wouldn’t be so impressed if they said they were benchmarking a simple "for" loop. However, we should not be too quick to write off such work, and it’s easy to see that when performance matters, all contributions should be gratefully accepted. Reactive patterns fit naturally with message processing (since an event translates nicely into a message), so if there is a way to process more messages faster we should pay attention.


Spreadsheets Perhaps not really an enterprise use case, but one that everyone in the enterprise can easily relate to, and it nicely captures the philosophy of, and difficulty of implementing FRP. If cell B depends on cell A, and cell C depends on both cells A and B, then how do you propagate changes in A, ensuring that C is updated before any change events are sent to B? If you have a truly reactive framework to build on, then the answer is "you don’t care, you just declare the dependencies," and that is really the power of a spreadsheet in a nutshell. It also highlights the difference between FRP and simple event-driven programming — it puts the "intelligent" in "intelligent routing".


Abstraction Over (A)synchronous Processing This is more of an abstract use case, so straying into the territory we should perhaps be avoiding. There is also some (a lot) of overlap between this and the more concrete use cases already mentioned, but hopefully it is still worth some discussion. The basic claim is a familiar (and justifiable) one, that as long as developers are willing to accept an extra layer of abstraction, they can forget about whether the code they are calling is synchronous or asynchronous. Since it costs precious brain cells to deal with asynchronous programming, there could be some useful ideas there. Reactive Programming is not the only approach to this issue, but some of the implementaters of FRP have thought hard enough about this problem that their tools are useful.

This Netflix blog has some really useful concrete examples of real-life use cases:Netflix Tech Blog: Functional Reactive in the Netflix API with RxJava "


From http://www.introtorx.com/content/v1.0.10621.0/01_WhyRx.html : 

* UI events like mouse move, button click
* Domain events like property changed, collection updated, "Order Filled", "Registration accepted" etc.
* Infrastructure events like from file watcher, system and WMI events
* Integration events like a broadcast from a message bus or a push event from WebSockets API or other low latency middleware like Nirvana
* Integration with a CEP engine like StreamInsight or StreamBase.

# Tutorials
* https://github.com/ReactiveX/RxJava/wiki/How-To-Use-RxJava
* http://rxmarbles.com/
* http://reactive.how/
* RxRuby https://ieftimov.com/reactive-programming-rxruby
* RxRuby https://github.com/fteem/RxRubyKoans
* RxRuby https://rubyinrails.com/2017/09/16/async-mongo-queries-in-ruby/
* RxRuby https://www.gitbook.com/book/vovayartsev/reactive-rails-app/details
* RxJava https://github.com/Froussios/Intro-To-RxJava
* RxJava http://www.baeldung.com/rxjava-tutorial
* Project Reactor (Java) http://www.baeldung.com/spring-reactor
* RxJS https://github.com/Reactive-Extensions/RxJSKoans
* RxJS http://reactivex.io/rxjs/manual/tutorial.html
* RxJS https://tech.pic-collage.com/a-gentle-introduction-to-reactive-programming-via-rxjs-52d801228763
* RxGo https://github.com/ReactiveX/RxGo (not sure if Go needs it (smile) )
* https://www.coursera.org/course/reactive
* http://reactivex.io/documentation
* http://blog.kontena.io/event-driven-microservices-with-rabbitmq-and-ruby/
* http://blog.cloud66.com/supercharge-rails-with-vuejs-and-actioncables/

# Samples:

* https://github.com/AleksanderBrzozowski/spring-reactive-pet-clinic
* https://github.com/ssouris/petclinic-spring5-reactive
* https://github.com/kgoralski/kotlin-reactive-playground


# Advantages  & disadvantages
Actually it is good for use cases described above.

"So let’s take a closer look at a few advantages

* Avoid the dreaded “callback hell”;
* It’s a lot simpler than regular threading;
* Has a standard mechanism for error recovery;
* Pretty straight forward and obvious way to compose asynchronous operations;
* Handling UI interactions/events is insanely easy;
* It offers the same “API” for database access, UI, computation, network access and everything you need it to be;
* It makes a lot easier to do complex threading, synchronising work in parallel and running some code when everything is done;
* Super easy way to talk to the UI thread;
* Makes concurrency almost hassle free;
* As soon as you understand the basics you can learn other operators as you need them, you don’t have to understand everything to start using it;
* Operators bring a lot of well tested code that can help you solve tasks;
* It helps make things more maintainable as you can add and remove blocks of code to a stream as needed;
* Doing things in a more functional way leads to readable declarative code that is easier to understand, test, and debug;
* There are some disadvantages though

Not everything is good

* The steep learning curve is not only because of the libraries, but also thinking reactively and using FRP to solve problems.
* It’s easy to not properly handle subscriptions and accidentally leak memory;
* Although being lightweight, RxJava still adds a good amount of methods towards the dex limit (with over 3500 methods);"
https://medium.com/@cesarmcferreira/why-you-should-be-doing-functional-reactive-programming-858bd9bb8001

# References

* http://reactivex.io/
* http://reactivex.io/documentation
* https://www.reactivemanifesto.org/
* https://gist.github.com/staltz/868e7e9bc2a7b8c1f754
* http://www.introtorx.com/content/v1.0.10621.0/01_WhyRx.html
* https://www.slideshare.net/epoberezkin/wtf-is-reactive-programming-75512905
* https://github.com/ReactiveX/RxJava/wiki/What's-different-in-2.0
* https://dzone.com/articles/spring-5-webflux-and-jdbc-to-block-or-not-to-block
* https://docs.spring.io/spring-framework/docs/5.0.0.M1/spring-framework-reference/html/web-reactive.html
* https://spring.io/blog/2016/11/28/going-reactive-with-spring-data
* https://kgoralski.github.io/post/rxjava-basics/
* http://www.vogella.com/tutorials/RxJava/article.html
* https://www.future-processing.pl/blog/reactivex-asynchronous-programming-done-right/
* https://github.com/ssouris/petclinic-spring5-reactive
* http://www.baeldung.com/vavr
* https://www.youtube.com/watch?v=LrPBHADuGuw
* https://developers.redhat.com/blog/2017/06/30/5-things-to-know-about-reactive-programming/
* https://blog.mindorks.com/a-complete-guide-to-learn-rxjava-b55c0cea3631
* https://stackify.com/when-to-use-asynchronous-programming/
* https://github.com/AleksanderBrzozowski/spring-reactive-pet-clinic
* https://www.kotlindevelopment.com/kotlin-webflux/
* https://dzone.com/articles/spring-boot-20-webflux-reactive-performance-test
* https://www.youtube.com/watch?v=LrPBHADuGuw
* https://www.slideshare.net/brendangregg/rxnetty-vs-tomcat-performance-results
* https://dzone.com/articles/spring-boot-20-webflux-reactive-performance-test
* https://stackify.com/reactive-spring-5/
* https://medium.com/@ggonchar/reactive-spring-5-and-application-design-impact-159f79678739
* https://spring.io/blog/2016/02/09/reactive-spring
* https://spring.io/blog/2016/06/07/notes-on-reactive-programming-part-i-the-reactive-landscape
* https://medium.com/@cesarmcferreira/why-you-should-be-doing-functional-reactive-programming-858bd9bb8001
* https://www.cocoawithlove.com/blog/reactive-programming-what-and-why.html
* https://medium.com/netflix-techblog/reactive-programming-at-netflix-b944d49874d2
* https://github.com/ReactiveX/RxJava/wiki/Additional-Reading
* https://vimeo.com/221255968
* https://www.infoq.com/articles/Servlet-and-Reactive-Stacks-Spring-Framework-5
* https://allegro.tech/2014/10/async-rest.html
* https://www.youtube.com/watch?v=weWSYIUdX6c


# Books
* http://introtorx.com/
* http://reactivex.io/tutorials.html#books
* Reactive Application Development https://www.manning.com/books/reactive-application-development
* Rx.NET in Action https://www.manning.com/books/rx-dot-net-in-action
* Reactive Programming with RxJava http://shop.oreilly.com/product/0636920042228.do
* https://www.gitbook.com/book/talanta/rx-book/details



# About Netty/Webflux (Java)
Spring Webflux enables using Netty with less effort. Not forcing you to use async/rx. The code can looks pretty much the same like Spring MVC. And use Rx when needed. Btw. Spring WebFlux is supported on Netty, Undertow, Tomcat, Jetty, and Servlet 3.1+ containers. 

"Netty is a non-blocking I/O client-server framework for the development of Java network applications such as protocol servers and clients. The asynchronous event-driven network application framework and tools are used to simplify network programming such as TCP and UDP socket servers.

WebFlux can run on Servlet containers with support for the Servlet 3.1 Non-Blocking IO API as well as on other async runtimes such as Netty and Undertow. Each runtime is adapted to a reactive ServerHttpRequest and ServerHttpResponse exposing the body of the request and response as Flux<DataBuffer>, rather than InputStream and OutputStream, with reactive backpressure. REST-style JSON and XML serialization and deserialization is supported on top as a Flux<Object>, and so is HTML view rendering and Server-Sent Events."

http://normanmaurer.me/presentations/2014-netflix-netty/slides.html - Why Netty?

https://www.techempower.com/benchmarks/#section=data-r15&hw=ph&test=json

http://normanmaurer.me/blog/2013/11/09/The-hidden-performance-costs-of-instantiating-Throwables/

https://docs.spring.io/spring/docs/5.0.0.BUILD-SNAPSHOT/spring-framework-reference/html/web-reactive.html

https://docs.spring.io/spring/docs/current/spring-framework-reference/web-reactive.html



https://www.infoq.com/articles/Servlet-and-Reactive-Stacks-Spring-Framework-5

The code of Webflux is very similar to MVC https://github.com/kgoralski/kotlin-reactive-playground



# Who is using it?

Reactive programming with RxJava has enabled Netflix developers to leverage server-side concurrency without the typical thread-safety and synchronization concerns.
