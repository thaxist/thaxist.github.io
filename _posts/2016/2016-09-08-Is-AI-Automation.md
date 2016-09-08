---
layout: post
title: "Is Artificial Intelligence Just Automation?"
date: 2016-09-07
categories: ai
---
 
To many, "Artificial Intelligence" is an exciting concept.  It's sexy.  It's scary.  It's futuristic.  By contrast, [automation](https://en.wikipedia.org/wiki/Automation) sounds dull, mechanistic, and Orwellian.  It sounds like **mindless machines**, taking away what soul we have left on planet Earth.  There's an emotional difference between the two terms, for sure.  But is there a real difference?  What is AI, anyway?  How exactly is it different from automation?
 
I think the confusion between AI and automation is central to a broader cultural and intellectual confusion taking place today.  Futurists such as Ray Kurzweil, or Elon Musk, or Kevin Kelly, or Oxford professor Nick Bostrom (and there are many others) imbue AI with almost magical powers.  AI's will "come alive" and have minds, and formulate devious plans to take us over.  To the **AI Futurists**, we are in the process of a profound transformation, no less than the evolution of a new species.  Like Kubrick's (and Spielberg's) 2001 movie [A.I.](http://www.imdb.com/title/tt0212720/), we are "Orga" or organic life forms, and AI's are "Mecha" or mechanical life forms.  But the AI's keep getting smarter and smarter, and so the distinction between mindful Orgas and mechanical Mechas will disappear.  To the AI Futurist, the world belongs to the AIs.   
 
The AIs-are-coming meme is a popular one, spread all over the Internet and in popular media like movies.  The **evil genius** in the 2015 hit [Ex Machina](http://www.imdb.com/title/tt0470752/) captures the futurist mood, when he laments that the prospect of AIs overtaking mere humans is inevitable.  "One day the AIs are going to look back on us the same way we look at fossil skeletons on the plains of Africa," he says, taking a drink of vodka, musing existentially about his soon to be forgotten life.
 
Futurist AI is sexy, in the same way that good fiction is:  it has an emotional appeal to its followers.  (Here's to storytelling.)  But the question of what AI means to us, scientifically, I think is a different question and requires different thinking.  At the heart of the question of AI is not all this sci-fi futurism about the arrival of new, **sentient AIs** "coming alive," but rather the boring (and Orwellian) question of automation.  And, spoiler alert:  today's AI is just automation, and nothing else.  Can automation become mindlike?
 
To be sure, Futurist-AI enthusiasts are quick to point out that current AI applications are "narrow," meaning that they only solve problems in a specific application domain.  [Narrow AI](https://techcrunch.com/2015/01/31/narrow-ai-cant-do-that-or-can-it/) is today's AI, which does something well, that used to require humans.  But that's all it does:  chess playing computers only play chess; Jeopardy! playing computers only play Jeopardy!; self-driving cars only drive cars.  So the immediate problem arises as to how Narrow AI will sprout into the __Ex Machina__ type of AI, with minds and devious or angelic motives.  We used to call this latter possibility Strong AI, and lately we refer to it as [Artificial General Intelligence](https://en.wikipedia.org/wiki/Artificial_general_intelligence)(AGI).  How does this transformation happen?  How do Narrow AIs get real minds?
 
If we believe the rapture of futurist and Google's Director of Engineering Ray Kurzweil or co-founder of Wired magazine Kevin Kelly (check out his 2010 book [What Technology Wants](https://www.amazon.com/What-Technology-Wants-Kevin-Kelly/dp/0143120174), the transition from Narrow to AGI happens sort of like falling in love:  first gradually, then all at once.  AI will gain in sophistication, chugging along as Narrow AI, until it reaches a level of intelligence, at which point it starts designing itself and becomes "ultra intelligent," as the late mathematician I.J. Good famously proposed back in the 1960s.  More recently, Nick Bostrom, author of the 2014 best-seller [Superintelligence](https://www.amazon.com/Superintelligence-Dangers-Strategies-Nick-Bostrom/dp/0198739834/ref=sr_1_1?s=books&ie=UTF8&qid=1473299386&sr=1-1&keywords=Superintelligence), calls it superintelligence.  In other words, Narrow AI not only expands into AGI, but AGI pops out of its shell and becomes superintelligent AI.  This stuff just gets smarter and smarter.  Fossil skeletons, we are, on the plains of Africa...
 
This is all great futurism, but I think it's suspect.  If we take a more critical angle, it's easy to see that we don't really know much about AI at all, except that we can keep making Narrow AI applications that do more and more.  It's clear that AI becomes more powerful.  But the question is how it becomes less narrow.  Or:  how does AI--which we only know to work with specific applications--somehow come to exhibit general intelligence, like a mindful creature, like us?  Confidently asserting that intelligence keeps increasing or evolving to a point where it explodes into **superhuman intelligence** doesn't tell us anything much.  (Or rather, it tells us that we humans like to imagine technological futures, and the more bizarre and fantastic, the better!)
 
 In fact, let's cut out of this discussion altogether the blather about superintelligence.  We can focus on AGI.  An AGI would walk around (if it was a robot) and talk to us, and take out our garbage, and watch the Giants play on T.V. with us.  General here means like us; so, the AGI would have a **human-like intelligence**.  How does that happen?  How do computers start acting like they have a mind?
 
 To see why this is actually a very deep question, and one without an easy answer at all (no matter what the AI-Futurists say), we have to step back and look at how boring, ordinary Narrow AI works. We have to start with how AI actually works, and then try to understand where it might be headed.  If this sounds overly conservative, I'd argue that it's much more scientifically-minded than starting with what we want it to be (futurism), then insisting that it will be that way.  Let's start with observation, in other words, and try to extrapolate from what we **observe and know**.
 
 Building an AI application involves two steps.  One, the problem you are trying to solve, or analyze, must be __representable__.  If I want to teach a computer to play the ancient **Chinese game of Go**, I must first figure out how to represent the game of Go not as a human sees it, but rather as a data structure, where computation can be performed on it.  Otherwise, no AI.  Thus representation is our first requirement.  All AI uses an underlying representation of the problem space, whether it's hand-coded business logic for an enterprese software system, or deep learning algorithms for recognizing human faces on Facebook pages.
 
 Second, the problem must be analyzable in terms of a sequence of steps.  We can call this algorithmic, or just computational.  I'll use the term __specifiable__ to indicate that the problem can be identified as solvable in some finite sequence of steps.  This is essentially the same definition as "algorithm"--we can use the terms interchangeably.  Every problem that admits of an AI solution (or any computational solution at all) must first be translated into a representation, and a specification.  For example, if we wish to use a **convolutional neural network** ([deep learning](http://www.kdnuggets.com/2016/01/seven-steps-deep-learning.html)) approach to learning Go moves, we first translate Go into a game tree (representation), and then we identify learning algorithms that take as input prior board positions, and output some set of numbers describing their rank (regression), or output a best move (classification).  We thus specify how we will compute moves on the board that simulate playing the game.  If we don't reduce the problem to a representation and a specification, we don't have a computational treatment of the problem.  Ipso facto, we don't have an AI.
 
 Using this simple framework, it's easy to see how Narrow AI keeps succeeding at more and more complicated tasks.  Engineers and scientists, armed with more and more powerful computers, and using a larger and larger stock of techniques and approaches learned from prior attempts at other problems, keep finding creative ways to represent bits and pieces of our social lives and our world as computational problems.  **Strategy board games** like checkers, chess, and now Go are classic examples of this process of reducing a bit of intellectual activity (playing chess, say) to computation.  First, the game of chess is viewed as a data structure--a game tree--, then algorithms are specified for the game tree such that good or bad (and legal or illegal) moves can be taken, or simulated, on the computational representation of the game.  Once we have this reduction to computation, we can start building an AI.
 
 Correction:  we can start building a __Narrow AI__.  Because the problem reduced in this way is in essense translated into a recipe for that problem, the AI that succeeds at, say, playing great chess typically does nothing else.  The representation was brilliant for defining and devising chess algorithms like mini-max, but because of the specifics of the representation and specification, lots of other stuff gets pushed to the side, out of reach.  Narrow AI makes AGI __less__ likely.  This is how **IBM's Watson** caused such a stir by playing Jeopardy! (pretty cool), but somehow fails to understand much of anything else about language, especially the more general, simple tasks of reading and understanding basic prose, like in the newspaper, or from the guy chatting with you on the street.
 
 In fact, much of the intelligence of an AI system like Watson can be attributed to the human engineers, who ingeniously found ways to make playing the game of Jeopardy __non__-general.  They found an architecture, and a set of algorithms, that translate the task of playing Jeopardy! into a tractable representation and specification (see my article on this [here](http://www.thebestschools.org/magazine/watson-computer-plays-jeopardy/)).  At that point, all the intelligence is "set" in the system; Watson isn't gonna run off and start thinking or doing something else.  The price of Narrow AI victory is such specificity.
 
 Similar comments could be made about any other Narrow AI application, including voice to text, machine translation, self-driving cars, personal assistants like Google Now, and anything else called AI today.  It's all a reduction to representation and specification.  Voice recognition uses a kind of **supervised learning algorithm** called a graphical model (often a [Hidden Markov Model](https://en.wikipedia.org/wiki/Hidden_Markov_model)] or HMM).  Well, it learns from prior examples, but it's also a specifiable algorithm using a representation.  And so on.
 
 It follows, given this I think relatively straightforward treatment of how AI actually works today, that it's quite a leap of imagination for us to believe any of these systems will somehow become general intelligences, much less sentient ("coming alive"--how would that work?!).  In fact, once one understands how AIs exhibit the **simulated intelligence** that they do, it becomes even more difficult to see how they can become general, or mind-like, at all.  It's apples and oranges, once we know the details.
 
 At this point, we can just throw out all this Narrow AI discussion--it's depressing for the futurist, after all--and ask how AI might nevertheless arrive at general intelligence.  Forget Narrow AI.  What other paths exist?  Let's broaden the discussion.
 
 Science is great at finding limits to knowledge, especially when it's self-consciously attempting to extend our knowledge.  The laws of dynamics tell us about entropy; Einstein showed that the speed of light has a limit; **quantum physics** tells us about the uncertainty principle; chaos and complexity tells us about unpredictability; mathematical logic tells us about undecideability.  This is all part and parcel of good science.  We learn not just what we can do, but what we can't do.  And I think the lesson of AI is that what makes AI succeed, when it does, is reducing the problem, making it specific; excluding the other possibilities.  This is why we can call [Deep Blue](https://en.wikipedia.org/wiki/Deep_Blue_(chess_computer)), the chess playing computer, or [AlphaGo](https://en.wikipedia.org/wiki/AlphaGo), the Go playing computer, automation as well as "AI."  Why?  Because it is automation, by definition:  it's a mechanical way of simulating what used to require human intelligence.  It's pure automation, this AI business today.

Back to science and limits, think about this:  when we ask then how to make the simulation general, too, we're asking how we can escape the limits or boundaries we put on the problem in order to, well, make it work in the first place.  So this is a very basic problem for the Futurists.  While they point to Narrow AI success as evidence for the arrival of **AGI**, they use examples that shine no light on AGI at all.  They're pointing to examples of __limits__ to general intelligence, in order to argue for it.  (No wonder everyone is confused.)

But who can blame them?  We've just explained how every single AI example we can point to that actually works, is just one more example of reducing a problem to representation and specification.  That is, to automation.
 
 Another way to understand the distinction between the usable AI we see around us, Narrow AI, and the futuristic AI we talk about in movies and on blogs (not this one), is by asking if there are aspects of our intelligent life that don't seem reducible to specific representations or specifications.  There are, of course, and we won't have to look far and wide.  We can look no further than ordinary, everyday language, like a conversation you might have with a six year old, or whomever (say, your drunk uncle, or your librarian--what have you).  In a later post, I'll explain why **natural language understanding** (NLU) is not a Narrow AI application, and what this suggests about the real differences between AI and minds.
 
 
 
 