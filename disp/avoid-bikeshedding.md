# How Disp will avoid Bikeshedding
[Bikeshedding](https://thedecisionlab.com/biases/bikeshedding) is a problem that many projects (specifically programming languages) have where a disproportionate amount of time is spent discussing irrelevant or preferential aspects of the feature. Instead of just implementing the feature, it gets stalled due to unnecessary disagreement on unimportant aspects (such as syntax). This is unnecessary, and here is how disp will fix it:

When trying to figure out what syntax, keywords or defaults to use for the language, if there is not an obvious consensus, multiple potential implementations will be merged into the compiler under optional flags for programmers to experiment with them. The different syntactical representations of the feature must be equivalent in the abstract syntax tree that disp files are saved as.

To figure out which one should be used by default, use [persistent voting](https://hopefulpathway.blainehansen.me/persistent-voting) to get the most-liked version. Persistent voting is nice because the feature representation can even be changed after a default has been agreed upon if the community so wishes.