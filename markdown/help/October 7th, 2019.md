- 13:18 -- 13:21 [[Conor]]
    - Wrote up a bit on "Creating headers"
   {{embed: ((qDoJ5qCJd))}}
- 13:21 -- 13:42
    - [[Conor]] put in start of our [[Privacy Policy]]
- 20:19
    - Notes on [[Michael Nielsen]] and [[Andy Matuschak]]'s [[Essay]] [[How can we develop transformative tools for thought?]]
        - source:: https://numinous.productions/ttft/ 
        - first impressions::
            - I'm a bit disappointed that the whole first part of the essay is dealing with memory and education.
                - There is definitely something significant about building a better textbook -- which is what [[Quantum Country]] is
                    - it is totally correct to have a piece which is giving you long form material have a problem set, and spaced-repetition style tutorial built into it.
                    - To me this feels like taking what works about school (you read something and are then tested on it), and then optimize that by presenting the tests immediately upon reading, and then following an optimum forgetting curve.
                    - Yes -- if we had more material online like this, we would definitely have better knowledge transfer from teachers to their students
                    - Yes -- many complex thoughts do require that you have the fundamental concepts down in order to do any sort of interesting novel work with them
                    - But somehow this feels like learning, which is differant than thinking
            - Ok, so parts of this essay are sort of infuriating to me right now
                - Particularly "$$\color{red}24.$$ Of course, a designer who spoke to an expert on, say, Babylonian mathematics, might well have come across some of these ideas. We'll ignore that, since it depends on the oddity that many excellent prior ideas about numeral systems had been displaced in Roman culture.)" in relation to ""__The typical modern design practice__" would not cause you to discover any deep insights about the field"
                - This just seems insane thing to ignore if your claim is that immersing yourself in the field is insufficient to generate the relevant insights -- since immersing yourself in the field -- as I see it, would ensure you eventually found someone who knew something about Babylon
                    - I'm also taking for granted that 
                        - the situation where Roman culture had displaced good Bablyonian ideas isn't unique.  
                        - We've now displaced good ideas from the 60s 70s and 80s
                            - reason::
                                - "This seems like a more reasonable critique of the current design community -- specifically related to [[Bret Victor]]'s talk where he slams software for not paying attention to the good ideas from the ancestors 

see [[The Future of Programming]] {{youtube: https://www.youtube.com/watch?v=8pTEmbeENF4}}"
                - I mean -- maybe someone like IDEO who is doing a 1 year project is going to fail this way -- but what the hell is the person doing by "you'd interview domain experts (in this case, mathematicians), " "and read any relevant literature. " if not trying to reach a deep enough understanding of the field to have the relevant insights for solving their design problem
                - I'm going to hope that there is some stuff later that presents an alternative to 
                - Perhaps what they're saying is that iff you only focused on "In short, you'd do what people in the design community refer to as immersing themselves in the target field." you wouldn't have a wide enough definition of the field, you wouldn't be able to find anyone who knew anything about how they did things in Bablyon, or if you did you wouldn't be interested in the approaches that they were taking
                    - This seems like a more reasonable critique of the current design community -- specifically related to [[Bret Victor]]'s talk where he slams software for not paying attention to the good ideas from the ancestors 

see [[The Future of Programming]] {{youtube: https://www.youtube.com/watch?v=8pTEmbeENF4}}
            - I might have been a little to hard on this "Ok, so parts of this essay are sort of infuriating to me right now"
                - Particularly thinking about it in Relation to [[Roam]]
                    - Yes, for the past few years we've been doing something a bit more like "__The typical modern design practice__" -- due to a funding model where we could only get paid to build things that users in the AI Research community were asking for -- and yes, that was extremely frustrating because we definitely were trying to explore fundamental ideas that hadn't been manifested in any previous tool
                        - However -- doing this did put a lot of pressure on us to feature match the existing tools -- which were necessary to get adoption, and to even begin to introduce users to the new concepts in Roam
                    - The better insights came from things like learning about [[Zettelkasten]], or [[Tiago Forte]]'s explanations related ideas with [[Intermediate Packets]]
                        - There was also a sort of aesthetic itch to be able to build these sort of knowledge graphs, so that we could go off in tangents, but then be able to concisely organize a set of complex interrelated claims and questions
                - Key Questions::
                    - What are the [[Deep Insights]] in [[Roam]]?
                        - It does feel tough to say, because it does feel like many of the deepest insight's we've had we haven't been able to implement yet -- partially because some of the problems are still unsolved 
                            - "One of the key things we figured out I think, was to not try to write a programming language that would actually say much about the Meaning of that statement ""Bob Marley" is "The Pope" of "Reggae"""
                            - Also, many of the deep insights currently are barely expressed in the UI -- they'll only really come out in future features we have in development
                                - specifically thinking about the way we want to combine [[Associative Data Model]] with [[Graph Databases]] and [[Event Logs]]
                                - Or the models of version control and sharing that are inspired by [[Federated Wiki]]
                    - Where did the [[Deep Insights]] in [[Roam]] come from?
                        - [[Douglas Hofstadter]]'s [[Analogy as the Core of Cognition]] and the larger book [[Surfaces and Essences]]
                            - Open Question::
                                - Do things like [[Word Vectors]] from ML capture any of the things that are expressed in analogy?
                                - How would you stress test or expand an analogy with a tool like [[Roam]]?
                                    - Well, you could be a hell of a lot more specific than is available in just text
                                        - The example given in [[Surfaces and Essences]]
                                            - "Bob Marley" is "The Pope" of "Reggae"
                                                - Bob Marley
                                                - The Pope
                                                - Reggae
                                    - One of the key things we figured out I think, was to not try to write a programming language that would actually say much about the Meaning of that statement ""Bob Marley" is "The Pope" of "Reggae""
                                        - To really dive into that -- if you wanted to try and evaluate whether it was true -- you'd have to figure out some things about the relationship between the pope and the catholic church -- or perhaps the pope to others outside the catholic church (or maybe you actually mean to God) -- and then you'd say something like does "Bob Marley" have the same sort of relationship to "Reggae" as the pope does to any of the things you might be comparing him to
                                            - In the english sentence, there is a shit-ton of ambiguity about what the speaker actually means by that statement
                                                - Even when they write it, even if they then tried to explain it, they  definitely aren't going to be able to capture all the possible interpretations of what that statement could mean. 
                                                - So, the thing we adopted instead was something like [[Block Mentions]] which just allow you to target particular "nodes" which are just lines of text in the knowledge graph
                        - [[The Universal Design Pattern]] by [[Steve Yegge]] which draws on Doug's work from [[Godel Escher Bach]]
                        - [[Clojure]] -- specificially [[Rich Hickey]]'s talk on [[Design Composition and Performance]]
                        - 
            - The further I get into the essay though, the more I'm troubled by their use of the term [[Tools for Thought]] to describe the [[Mnemonic Content]] they're talking about building!
                - The whole thing is about Pedagogy!
                - it's all about transferring existing stores of knowlege!
                - Not about the creativity of Remixing Ideas in order to generate new ones
                - Not about the process of actually relating the new idea to other things you've learned
                - Not about the process of solving problems
                - Yes - For damn sure, we need better educational content -- but the idea that a better tool for ensuring lossless transfer of a set of ideas from one person to another through media - interactive or otherwise -- is so fucking different from what I think anyone like [[Doug Engelbart]] or [[Howard Rheingold]] meant when they talked about [[Tools for Thought]]
                    - [[Book: Tools for Thought]]
            - The stuff that [[Ivan Sutherland]] was doing with [[Sketchpad]] wasn't about educational content, it was about direct manipulation in order to solve harder problems
            - These guys should know better than to do this
                - Haven't they read
                    - [[Augmenting the Human Intellect: A Conceptual Framework]]
            - The last few sections of the document seem to be the most interesting -- but they're buried with too much demo of a tool that is more about education than about problem solving and original thinking
                - Transmission is a part of the problem -- learning the things you need to know is a crucial part of [[getting into a position to think]]
                    - "his observations revealed that about 85% of his "thinking" time was actually spent "[[getting into a position to think]], to make a decision, to learn something I needed to know. Much more time went into finding or obtaining information than into digesting it.""
                    - "Licklider's analysis of his research behavior showed that most of his [[task]]s were clerical or mechanical: "searching, calculating, plotting, determining the logical or dynamic consequences of a set of assumptions or hypotheses, preparing the way for a decision or an insight. Moreover, my choices of what to attempt or not to attempt were determined to an embarrassingly great extent by considerations of clerical feasibility, not intellectual capacity." #important "
                    - 
        - Tweet Storm::
            - Extremely frustrated with the latest  essay from [[Michael Nielsen]] and [[Andy Matuschak]] on Tools for Thought https://numinous.productions/ttft/#memory-systems

But.. it could be because MY models are wrong... so sharing em here

thread
{{count}}
            - First a caveat -- I really respect both of the authors

Michael wrote one of the best books I've read on collective intelligence, which was a huge inspiration for my work {{count}}
            - Andy has shared some fantastic ideas in the few times I've talked with him
            - he's also given me the best grilling on twitter I've yet had {{count}}
            - I also care really deeply about the problem space -- I've been working  on designing Tools for Thought for the past 6 years. More if you count my first startup (a collective intelligence experiment for local govts) or time at Huffpost Labs {{count}}
            - I went as far as living in a van for a year and moving to India for two so I could cut down on rent, avoid taking a "real job", and focus on reading and prototyping {{count}}
            - Since I've gotten so much out of both their work, and they titled the essay precisely on my life goal, I had very high expectations for this piece
            - I should also stress -- it's not exactly a bad essay, it just, in my current opinion, gives dangerously bad examples without context for why they fit into the category
            - Before I go into why, I'll start with an argument for why I'm wrong, and it might be the correct title
            - After a quick nod to Alan Kay, Ivan Sutherland, and [[Doug Engelbart]] -- the vast majority of the essay is about pedagogical technology.  {{count}}
            - They talk about essays or videos delivered online that embed spaced repetition tests inline to more effectively transfer the core ideas in a discipline (like Quantum Physics) to a student/reader/viewer

Case study being quantumcountry.com
 {{count}}
            - The claim they are making seems to be: you can't think about certain domains if you don't understand the core ideas in them - so the highest leverage tool for thought is a tool that helps you get those core ideas into your long term memory {{count}}
            - That at least is what I expect people to take away if they stop reading half-way through, or skim the essay, or think that the examples they give are the ones that symbolize the term they're using {{count}}
            - The claim isn't crazy either
            - The other examples they give for tools for thought are 
            - They also say explicitly that they can not - by definition give an example of what future tools for thought will be like -- because if you could communicate the idea in words, it wouldn't be transcending words
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fv8%2Fhelp%2FrMSpJiRTqM?alt=media&token=26304daf-a694-43b7-9c8e-3c7a867f3be2)
            - When I think about "Tools for Thought" I think about [[Doug Engelbart]]'s 1962 paper on Augmenting the Human Intellect -- specifically the hLAM-T model
            - Augmenting Intelligence means -- for Engelbart & myself

Making sense of what's happening in your environment

Better identification of what problems to focus on

Solving problems faster

Solving problems you couldn't have solved before {{count}}
            - Before Engelbart, all the focus in CS was on automation -- getting AI to replace human work.


            - Doug said this wasn't the real grail -- what was needed was Augmentation -- he had the first idea of a knowledge worker, who would work WITH computers to do things that neither could do alone {{count}}
            - He saw radar screens, and imagined a computer monitor, where a "knowledge worker" could interact directly with the computer -- instead of through punchcards {{count}}
            - His idea was, if we don't improve our capacity to make sense of the world, form and spread better models, and act on them -- then the increasing leverage we get over the world would lead to increasing destruction -- and we're all damned {{count}}
            - 
            - His paper set up a whole new paradigm -- was inspiration for J
            - 
