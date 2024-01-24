# Cedar Public Issue tracker

This is the public GitHub issue tracker for CedarEDA. Issues are tracked using
GitHub issues (see the Issues tab above). We are interested in any bug reports,
feature requests or particular benchmarks. However, please note that this
issue tracker is intended for Open Hardware users of Cedar. If you are a
commerical Cedar customer, please use your JuliaHub support mechanism for
any issues. In particular, all issues filed here are publicly visible.

## Frequently Filed Issues (aka Known Issues)

Below is a list of known general issues that we are aware of and working on.
While you are always welcome to file an issue, if your issue falls into one
of the categories below, there is no need to file an issue as we're already
working on it. However, if the issue is a performance issue and you have
a particular additional benchmark that exhibits the issue, you are still
welcome to file it so that we can validate that the issue is resolved on
all benchmarks as we work on a fix.

1. Code caching is not yet available in the released version of Cedar. The simulator will generate custom code, highly specialized, for every device in the circuit at the start of every simulation request (although each such request may run many simulations, e.g. for parameter sweeps). This may result in long delays before the start of compilation. In addition, the compilation delay for larger circuits may be prohibitive.

