# make-ambiguous

## description

a Chrome extension that looks at the "People also asked..." section on google search pages, judges the polarity/"loadedness" of the question, generates a neutral replacement, and displays that instead.

### the 'why', or the origin story

I was looking up 'Quintana Roo', hoping to see hits on both the place and the bike brand when searching just those two words (which there were), but then I noticed that the "People also ask" questions were: "What is the capital city of Quintana Roo?" "What is a Quintana?" "What is the population of Quintana Roo?" and "How poor is Quintana Roo?". I may be misguided, but to me, three of these are objectie questions and one of these is a "loaded" or pre-filtered or predisposed question. AFAIK, "poor" is not the name of the objective measure that the answer to that question presents itself in. The asker of that question is really looking for "The GDP of Quintana Roo" or "the global rank of the GDP of Quintana Roo", or both pieces of information together. Thus, the inspiration to create a plug in that visually replaces such loaded questions with their neutral equivalent on these pages.

## Current tasks

* determine when a URL is a google search (3)
* access the "People Also Ask" section if exists, and does nothing if not. (3)
* determine which, if any, questions in the PAA section are "loaded" (6)
* generate a complete and neutral replacement question (7)
* display this question in place of original (1)

I have rated these tasks in estimated difficulty on a scale from 1 (easiest) to 10 (hardest).

## Some useful resources

https://developer.chrome.com/extensions/overview
http://www.darbyhayesconsulting.com/scraping-people-also-asked/ 

## Some challenges/notes
As may have already been obvious to some of you, "loaded" questions are hard to distinguish. For instance, when looking up "Santa Cruz", we get the following PAAs:


**People also ask**
Is it expensive to live in Santa Cruz?
Is Santa Cruz safe?
Why is it called Santa Cruz?
Who bought out Santa Cruz?
What is the brand Santa Cruz?
Who owns specialized bike?


which ones are "loaded" questions? I find 1 and 2 to potentially fit my former definition of "loaded", even though it's hard to come up with a neutral yet concise replacement question. The first is easy enough, e.g. "What is the cost of living in Santa Cruz, compared to other similarly sized cities". But "Is Santa Cruz safe" is complicated.
