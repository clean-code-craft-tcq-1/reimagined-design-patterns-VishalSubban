# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.


**Observer:**

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**
Imagine you need to update screen information of each of the users who are getting an update from you.
Cricbuzz is a live example.
Cricbuzz needs to update the cricket score information of all the user applications.
Cricbuzz server is a Subject and all the users using cricbuzz app to view score in their mobile are observers.
When the score information is updated in the server (subject), it is updated automatically to all its clients (observers).

**how the pattern works, what the basic idea of the pattern is**
This idea works with following objects. 
1. Subject
2. Observer
As mentioned above, when subject is modified, all its dependent objects (observers) are notified automatically.

**what the main advantage and what the main disadvantage is of using this pattern**
**Advantage:**
Observers can be added or removed at any time
Data transfer from observer to clients is effective
**Disadvantage:**
No control over how many observers are attached and the flow over transferring data to observers.


**State:**

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**
Imagine the working example of a computer
You power on a computer and the state handling is as follows
1. Boot up or Pre-Run
2. Main processor Run
3. Display processor Run
4. Sleep 
5. Wake up
6. Shutdown

In Pre-run, the drivers in the computer will be powered up and initialized.
In Main processor run, the processor will be up and ready for usage
In Display processor run, the display drivers will be powered up, initialized and ready for usage
In sleep state, most of the drivers will be powered down and only few drivers will be up and running for power consumption and performance
In wake up state, all drivers will be powered up and initialized and ready for usage
In shutdown, all the drivers will be powered down and the processors will be powered off

**how the pattern works, what the basic idea of the pattern is**
The functionality of the software or system changes based on the state changes
what the main advantage and what the main disadvantage is of using this pattern

**Advantage:**
Easier to add states for additional behavior
Reduces conditional complexity

**Disadvantage:**
Large amount of code needed for state machine


**Builder:**

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**
Imagine the working example of McDonalds
Consider the meal as the end product. Meal comprises of veg-burger, fries, coke and ice cream which are actually type of burger, type of side, type of drink and type of dessert.

When customer (client) order a meal (end product), the attender(director) directs the chef(builder) to cook(build) the order.

**how the pattern works, what the basic idea of the pattern is**
This idea works as complex object is built as a step by step approach. The builder class builds the final object step by step

**what the main advantage and what the main disadvantage is of using this pattern**

**Advantage:**
Less complex logic in object building processor
Parameters to the constructors are reduced
Better control over construction process
**Disadvantage:**
More lines of code


**Proxy:**

**what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example**
Imagine that you want to use your money deposited in your bank account.
You can withdraw cash and make use of it. Or you can use your debit card or cheque to make use of it.
Here, the debit card or the cheque acts as a proxy to your money in the bank.

**how the pattern works, what the basic idea of the pattern is**
Proxy pattern is used when we need to create a wrapper to cover the main object’s complexity from the client.

**what the main advantage and what the main disadvantage is of using this pattern**
**Advantage:**
Security
Avoids duplication of objects

**Disadvantage:**
Response from service might be delayed
code  may be more complicated as we introduce lot of new classes.
