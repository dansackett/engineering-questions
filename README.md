# Engineering Questions

When working in the software engineering field there are so many questions that
you can ask up front to save time down the line when scoping out a new project.
There are also so many things to consider before shipping a product. Some of
these that I have run into are captured here as a checklist to remind myself
where my questions should be taking me.

## Questions about Edge Cases

- [ ] What's the empty state?
- [ ] What happens if there's only one?
- [ ] What happens when there are a thousand?
- [ ] What if times are in the distant future / past
- [ ] What happens if there are weird timezones?
- [ ] What happens when the request fails?
- [ ] What happens when the request is loading?
- [ ] What happens if the string is very long?
- [ ] Are there accesibility implications?
- [ ] How does it look on mobile? In landscape view?
- [ ] What happens when the user is logged out?

## Questions about Solutions

- [ ] Is there anything else like this in the product?
- [ ] Can I pull data to support a particular solution?
- [ ] Can I make a skeleton solution before working with a designer?
- [ ] Is there anything like this in other products?
- [ ] What would be the most consistent with the spirit of the rest of this page / product?

## Questions about Errors

- [ ] Do you handle errors gracefully? At all?
- [ ] Do you know why an error is occuring?
- [ ] Do you have error logging setup?
- [ ] Do you write regression tests to ensure errors do not return?

## Questions about Refactoring

- [ ] Is this function doing too much?
- [ ] Is this import being used anywhere else?
- [ ] Can these pieces be moved into a clearer module?
- [ ] Are you doing too much type checking?
- [ ] Are you doing too many conditional checks?
- [ ] Does this function make sense? Signature?
- [ ] Can the state of this class be shared among subclasses?
- [ ] Is the code orthogonal such that changing it will not change other parts of the system?

## Questions about using Dependencies

- [ ] How large is the dependency tree for your project?
- [ ] Does the third-party dependency you're considering have dependencies?
- [ ] Is the external API documented?
- [ ] Are you using the internal API? What if it changes?
- [ ] Are you using many features of the dependency or only a subset? Does it make sense to write the subset yourself?
- [ ] Are your dependencies easy to install for contributors to your project?

## Questions about Databases

- [ ] Do most of your queries run without JOINs?
- [ ] Could you benefit from denormalizing a column on a table?
- [ ] Do you have a way of discovering slow queries?

## Questions about Performance

- [ ] How large is the generated bundle of code? (mostly modern JS appropriate)
- [ ] Does an expensive task need to be run in realtime? Can it be asynchronous?
- [ ] Do you user ALL of the data from a request or can you limit the fields?
