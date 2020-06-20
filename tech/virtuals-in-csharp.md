# Virtual methods in C#

By default I dislike virtual methods (and also non-sealed classes) in C# for the following reasons:

- Extensibility should always be an explicit decision. Non-explicit extensibility in my experience leads to unmaintainable code.
- I generally prefer composition over inheritance because it is the much more flexible approach for adding functionality.
- If methods in a class depend on each other making those methods virtual can lead to unexpected problems when people break implicit assumptions in their derived classes.

## Further reading

- Related [Stack Overflow question](https://stackoverflow.com/questions/14451325/should-i-mark-all-methods-virtual) with a good mix of opinions in the answers. I strongly agree with [Eric Lipperts answer](https://stackoverflow.com/a/14451437/31985). 
