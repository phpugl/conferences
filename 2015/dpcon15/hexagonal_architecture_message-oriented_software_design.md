Matthias Noback - "Hexagonal archicture - message-oriented software design"
###########################################################################

Commands, events, queries - three types of messages that travel through your application. Some originate from the web, 
some from the command-line. Your application sends some of them to a database, or a message queue. What is the ideal
infrastructure for an application to support this on-going stream of messages? What kind of architectural design fits 
best?

This talk provides answers to these questions: we take the *hexagonal* approach to software architecture. We look at 
messages, how they cross boundaries and how you can make steady communication lines between your application and other 
systems, like web browsers, terminals, databases and message queues. You will learn how to separate the technical 
aspects of these connections from the core behavior of your application by implementing design patterns like the 
*command bus*, and design principles like *dependency inversion*.

Sources
=======

 * Talk <http://www.slideshare.net/matthiasnoback/hexagonal-architecture-messageoriented-software-design>
 * Blog <http://php-and-symfony.matthiasnoback.nl/>
 * Twitter <https://twitter.com/matthiasnoback>
 * Github <https://github.com/matthiasnoback>

Notes
=====

 * Framework will encapsulate you from the rest. Hard to follow messages.
 * Encapsulation vs. Abstraction
 * Domain-Driven

 * Core should be a polygon with borders that only messages could pass.
   
                  /--------------------------------------\
                 /                /------\                \
     outer world | infrastructure | core | infrastructure | outer world
                 \                \------/                /
                  \--------------------------------------/
    
     message --|-->


 * Each edge/border is a port to the core.
   
   * HTTP --|--> Controller / Request / Response --|--> Command / CommandHandler
   * CommandHandler / RepositoryInterface --|--> Repository / QueryBuilder --|--> Db / Sql query

