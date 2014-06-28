Tasks
=======

A real-time experiment with Amber frontend and Pharo backend. The backend uses custom Zinc handlers and the command pattern, also [Mapless](sebastianconcept.github.io/Mapless) on [Mongo](http://www.mongodb.org/) for storage.

###Motivation
> "Real-time is coming in hot, so we better get ready for it" ~ [Sebastian](http://about.me/sebastianconcept)

*There is no sync.*

*There is no async.*

*There is no real-time...*


*Only perception.*

###Set up

1. clone this repo
2. execute ./load
3. wait :)

### Handy code

    Reactive stop.
    odb := 	MongoPool instance databaseAt: 'Reactive'.
    
    "Changing state..."

    http://localhost:21003/service/dev.html

For navigate the code:

1. In the backend use Pharo check the package named Reactive
2. In the frontend open the console and do: 

    smalltalk.Browser._open()


### Questions and Contributions

...are welcomed, send that push request and hopefully we can review it together.

###Direction?

1. This experiment ended
2. We've learned we can do a clean RESTful API with Zinc
3. We've learned we can do elegant command pattern work in the web and
4. Scale the observer pattern in a multiuser app in the web without much of a problem
5. Using a mini-Mapless in the frontend get us the latency-compensation feature
6. Using Mapless reactivity supported by Redis could give us horizontal scalability

###*Pharo Smalltalk
Getting a fresh Pharo Smalltalk image and its virtual machine is as easy as running in your terminal:
 
    wget -O- get.pharo.org/30+vm | bash

_______

MIT - License

2014 - [sebastian](http://about.me/sebastianconcept)

o/