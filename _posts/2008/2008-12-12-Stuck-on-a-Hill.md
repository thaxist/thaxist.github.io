---
layout: post
title: "Stuck on a Hill"
date: 2008-12-12
categories: theory science.ai science
---

In artificial neural network (ANN) research, there's a well known problem of
local minima (or maxima). I've worked a bit with ANNs but much more with a
(superior) learning algorithm, Support Vector Machines (SVMs). Unlike the
latter, ANNs require heuristics to "converge" on an optimal solution given some
very large decision surface. The heuristics, to simplify a bit, are intended to
get the algorithm to converge on a global, not local, solution. Local solutions
are unwanted because they can appear to be global (good) solutions, given some
snapshot of the decision surface, but in fact are very bad solutions when one
"zooms out" to see the larger picture. This phenomenon is perhaps best
illustrated with geographical imagery. If I am walking up and down hills, en
route to a very large mountain, a local maxima might be the top of a foothill.
But it would hardly be a global maxima, like the top of the mountain. The point
is that ANNs can converge on the foothills, telling us that it's the mountain.

ANNs notoriously suffer from this limitation, but the "blindness problem" is
endemic to all statistical learning algorithms, including SVMs (though, at least
in theory, you can get an optimal solution with an SVM). Using such algorithms
to learn from past experience (i.e., training data), you generate an
approximation function for the underlying distribution you're trying to model.
You see the function as worth the time it took to gather training data, select
the features, and train, if it approximates pretty well the underlying target
distribution you're interested in. You can tell if it pretty well approximates
the underlying distribution if it keeps getting things right, and you don't have
to keep making excuses for it (say, by saying that "it's complicated").

Anyway, we can view ANNs, SVMs, and other statistical learners as essentially
inductive systems, in the sense that, given a set of prior examples, they learn
a rule (classifier) that allows us to predict something about new, unseen
examples. They generalize, in the sense that unseen examples that match a
profile (learned from the training data), even if not an exact fit, may still be
classified correctly. It's not a simple one-to-one match. Hence, _generalize_ .

The problem with the generalization performance of all such systems is two-fold.
One, they're limited by the set of features that were chosen (a person selects
features that are relevant, like "is followed with 'inc.'" for classifying
organization mentions in free text). Two, even given optimal feature selection,
the generalization performance of inductive systems is always hostage to the
information in the training data. We collect examples to use to train the
system, and, in the end, we hope that the training data was adequate to model
the true distribution (the thing we really want to predict). Problem is,
whatever hasn't occurred yet in this true distribution, can't possibly be
collected from past examples, and so the entire approach is hostage to the fact
that things change in real-life environments, and the larger "pattern" of the
true distribution as it unfolds in time may not be captured in the training
data. Whenever this happens, the approximation function does not model the true
distribution. Bummer.

Now, a feature in particular of such inductive systems (we can substitute
"supervised statistical learning sytems" if it sounds more fancy) is this local
minima or maxima worry, which I introduced with regard to ANNs, but which is
really just a handy way of introducing the general problem of generalizing from
past cases to future ones writ large. And it is a problem. Consider _time
sequence prediction_ (as opposed to, say, _sequence classification_ such as
the well-known document classification task in IR research). In time sequence
prediction, the goal is take a sequence of elements at time t, and predict the
next element at time t+1. Applying this multiple times you can predict a large
sequence of elements through some time n. 

And this is where the inductive problem comes in, because if the data you're
using to predict the next elements came from some set of prior elements, it's
possible that the prior elements (your training data), gave you a model that
will get you stuck on a foothill, or, will see the top of a small hill as a
bottom valley, and so on. You can't be sure, because _the future behavior of
the true distribution_ you don't have. And this is why, in the end,
induction&mdash;however fancy it gets dressed up in mathematical
clothing&mdash;not only can be wrong, in theory, but often is, in practice. 

We can't see into the future, unfortunately. If we could, we could fix the
inductive problem by simply adding in the additional information about the true
distribution that we're missing in our training data. But in that case, of
course, we'd hardly need the
approximation.