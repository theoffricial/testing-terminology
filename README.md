# Why Testing Terminology?

- It is negligible what programming languages or technologies one is using, The terminology is about having a shared set of conceptual terms that one can communicate with others and although it is technically, both parties will understand clearly each other on the higher level discussion, and it is applies while testing code as well.
- A technical modeling of the different types of testing objects possible, will help any developer to understand clearly what testing possibilities he/she will face sooner or later.

## TestDouble - Unit Testing Terminology

Test Double is a generic term for any case where you replace a production object for testing purposes.

There are various kinds of double:

- **`Dummy`** objects are passed around but never actually used. Usually they are just used to fill parameter lists.
- **`Fake`** objects actually have working implementations, but usually take some shortcut which makes them not suitable for production (an InMemoryTestDatabase is a good example).
- **`Stubs`** provide canned answers to calls made during the test, usually not responding at all to anything outside what's programmed in for the test.
- **`Spies`** are stubs that also record some information based on how they were called. One form of this might be an email service that records how many messages it was sent.
- **`Mocks`** are pre-programmed with expectations which form a specification of the calls they are expected to receive. They can throw an exception if they receive a call they don't expect and are checked during verification to ensure they got all the calls they were expecting.

## Examples

[TBD]()

Inspired by [Martin Fowler](https://martinfowler.com) blog.
