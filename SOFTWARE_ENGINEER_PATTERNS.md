## References

### How to manage/plan tasks? 

 
### [The best gitflow](https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow)

In even the smallest development projects, developers are often required to work on multiple components in parallel. Feature X, bug #102, a new UI for a sign-up form, etc.
Among many others issues, imagine these scenarios:

- Your client tells you that they don’t want feature X anymore.
- Or what if you find that feature Y — an experimental feature you have been working on — can’t be implemented?

How do you get code removed safely from your code base?

Using branches is the solution to these commonplace development problems.

Not convinced yet? you should read [it](https://www.webfx.com/blog/web-design/why-you-should-use-git/)

### Best practices to high quality code

- **Practice test driven develop**: code should have unit testing with at least 50% overall code coverage.
- **Team/Pair Programming**: code should be reviewed because it encourages discussion of code design 
- **Exception Handling**: code should handle exceptions to avoid retrieve errors to client
- **Keep It Simple Stupid**: simple code is elegant and can be harder to write but easier to maintain and understand
- **Use appropriate logging levels**: appropriate logging levels helps admins and developers deal with log messages appropriately