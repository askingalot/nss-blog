# What is an object anyway?

The word "object" gets used quite a lot in software development. It represents a concept that is important for every developer to understand. However, in my experience as a professional developer and as an instructor in the web development program of NSS, I've learned that it's not a very easy concept for beginners to grasp.

Outside of software development, it's common to think of an object as a physical thing. In fact, the first definition of [object](https://en.wiktionary.org/wiki/object) on Wiktionary.org says just that, "A thing that has physical existence". A clock radio, for instance, is an object - a real thing you can hold in your hand and interact with.

Software, of course, is not so concrete. In software development when we use the word "object", we mean something much _fuzzier_. You can't hold a software object in your hand. You can't feel it's weight, push its buttons, or set it on your nightstand. In a certain sense its not "real" in the same way a clock radio is. However, despite the many differences, a software object does have more in common with a clock radio than you might thing.

Let's look at some C# code.
```csharp
var clockRadioObject = new ClockRadio();
Console.WriteLine("Initial Time:");
Console.WriteLine(clockRadioObject.Time);
```
This gives us the following output.
```
Initial Time:
12:00 AM
```
The code above is analogous to plugging in a new clock radio and seeing the display blink midnight.

Just like with a "real" clock radio, we can set the time.
```csharp
clockRadioObject.Time = "2:03 PM";
```
In fact because software is so much more flexible than the pesky and limited, "real" world, we can just set the time directly without having to hold down some tiny, awkward button as numbers whiz by all the while hoping we don't pass the correct time ahd have to go around the clock again.

The above example shows us an important aspect of software objects: a software object _contains data_. Just like you can think of a real clock radio as having the current time, our `clockRadioObject` also has the current time. Even though the mechanisms work completely differently, the _concept_ is the same.

In addition to containing data, a software object often exposes a set of "operations" that can be performed. Each of these operations is composed of code that, when executed, will do something involving the object.

For example one of the things we can do with a clock radio is play the radio.
```csharp
clockRadioObject.Play();
```
Because this post is text, I'll humbly ask you to imagine with me the sound of music...
```
Lucy in the sky with diamonds
Lucy in the sky with diamonds
Lucy in the sky with diamonds, ahh
```
If imagining it is too much for you, I'll just leave this here for you to ~~enjoy~~ listen to. https://youtu.be/AB3uVARNhmM

Just like a clock radio contains the radio antenna, circuitry and speakers to play our favorite station, a software object contains the _code_ to perform operations.

## So What is an object? tl;dr
An object is a container of data and operations. Objects exist when our code is running and cease to exist when it stops.

