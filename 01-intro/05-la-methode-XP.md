# La méthode [XP][XP]
>Extreme programming (XP) is a software development methodology which is intended to improve software quality and responsiveness to changing customer requirements. As a type of agile software development, it advocates frequent "releases" in short development cycles, which is intended to improve productivity and introduce checkpoints at which new customer requirements can be adopted.

# Les activités 
1. Coding
2. Testing
3. Listening
4. Designing

## Coding
>The advocates of XP argue that the only truly important product of the system development process is code - software instructions that a computer can interpret. Without code, there is no working product.
Coding can also be used to figure out the most suitable solution. Coding can also help to communicate thoughts about programming problems. A programmer dealing with a complex programming problem, or finding it hard to explain the solution to fellow programmers, might code it in a simplified manner and use the code to demonstrate what he or she means. Code, say the proponents of this position, is always clear and concise and cannot be interpreted in more than one way. Other programmers can give feedback on this code by also coding their thoughts.

## Testing
>Extreme programming's approach is that if a little testing can eliminate a few flaws, a lot of testing can eliminate many more flaws.
Unit tests determine whether a given feature works as intended. A programmer writes as many automated tests as they can think of that might "break" the code; if all tests run successfully, then the coding is complete. Every piece of code that is written is tested before moving on to the next feature.
Acceptance tests verify that the requirements as understood by the programmers satisfy the customer's actual requirements.
System-wide integration testing was encouraged, initially, as a daily end-of-day activity, for early detection of incompatible interfaces, to reconnect before the separate sections diverged widely from coherent functionality. However, system-wide integration testing has been reduced, to weekly, or less often, depending on the stability of the overall interfaces in the system.

## Listening
>Programmers must listen to what the customers need the system to do, what "business logic" is needed. They must understand these needs well enough to give the customer feedback about the technical aspects of how the problem might be solved, or cannot be solved. Communication between the customer and programmer is further addressed in the planning game.

## Designing
>From the point of view of simplicity, of course one could say that system development doesn't need more than coding, testing and listening. If those activities are performed well, the result should always be a system that works. In practice, this will not work. One can come a long way without designing but at a given time one will get stuck. The system becomes too complex and the dependencies within the system cease to be clear. One can avoid this by creating a design structure that organizes the logic in the system. Good design will avoid lots of dependencies within a system; this means that changing one part of the system will not affect other parts of the system.

# Les pratiques d'XP
## Fine-scale feedback
* Pair programming
* Planning game
* Test-driven development
* Whole team

## Continuous process
* Continuous integration
* Refactoring or design improvement
* Small releases

## Shared understanding
* Coding standards
* Collective code ownership
* Simple design
* System metaphor

## Programmer welfare
* Sustainable pace

## Coding
* The customer is always available
* Code the unit test first
* Only one pair integrates code at a time
* Leave optimization until last
* No overtime

## Testing
* All code must have unit tests
* All code must pass all unit tests before it can be released.
* When a bug is found tests are created before the bug is addressed (a bug is not an error in logic, it is a test that was not written)
* Acceptance tests are run often and the results are published
 
Suite : [le build pipeline](../02-outils/00-le-build-pipeline.md)

 [XP]:(https://en.wikipedia.org/wiki/Extreme_programming)
