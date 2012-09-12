## What the sequences are representing and where they come from.My sequences are multi-channel sequences that represent the open source software development process. I have three channels: actor, activity, and artifact. The actor specifies *who* executes an action. The activity specifies *what* action is executed. Artifact specifies what the action is *related to*. For example a high-volume committer (actor) might commit (activity) a change to a requirements document (artifact). Hence, the channels are inherently connected to each other at each instance in time and unfold chronologically. Each activity has a timestamp.

I think that these are event sequences, however the events do not necessarily signify a change in state, but are rather activities with actors and artifacts attached to them.## The alphabet (list of symbols in the sequences).The alphabet consists of categories of actors, activities, and artifacts that are not ordered. The alphabet is under development, but essentially it looks like this:

### Actor

These are categories depending on what type of contributor the person who executes an action is:
* High-volume contributors
* Medium-volume contributors
* Low-volume contributors### Activities
These are common software development activities, as specified by the GitHub event stream:

* Create a new file
* Commit a change
* Comment on a commit or pull request
* Fork
* Pull Request
* Submit an issue (bug, feature request)

### ArtifactsI'm still working on this one, but it would include things such as:

* Specification document
* Wiki documentation
* Source code
* Binary files
* Testing code
* Deployment code## Size of Sequences
I'm looking at potentially huge datasets. At most I have sequenced 300 sequences of a maximum length of 60'000 events. This took 2 hours on the Case Western High Performance Computing Cluster.Because of the size of my sequences, graphical representations are not very interesting to me. Mostly I'm interested in ways of deriving statistics, clusters, and typical sequence structures.## The Kind of Knowledge You Expect to Extract From Your Sequences. 

I'm trying to identify typical sequence patterns that can be linked to covariates such as success, size of the community, code quality etc.