---
layout: post
title: The Solvable Problem and the Real Problem
---

This election cycle, I tried to get a job at one of the companies that receive the donations you give to your preferred candidate, that try to convince those Other People to vote like you do. I failed to secure one of these jobs. I made it decently far in a few interview loops but ended up with bupkis. For this essay, I am concentrating on the interview loop that was the shortest; you could also refer to it as a "single interview".

I am speaking of my interview with the chief something at Anne Lewis Strategies, joined by a senior something else at their parent company, InfoGroup. They were looking for a Machine Learning Engineer to design a tad of Machine Learning Automation.

The task that they described to me with giddy smiles was for me to use Machine Learning to pick out the words that would go into the spam emails that would make the people who clicked on those spam emails give campaigns the most money.

"Doesn't that seem kind of manipulative??" I said. At this point, the interview was over, but we were still talking because there’s some momentum inherent to conversations. They obviously disagreed with this sentiment, and we mulled that disagreement over for a few more minutes before ending the interview early.

This episode had already moved from my "talk about in conversations regularly" part of my brain downwards and inwards to the "only thought of when directly referenced" part of my brain when I met a fellow Boston-for-now in a sick Anne Lewis Strategies Patagonia fleece while we were both out canvassing in Maine. It got me thinking more about this episode.

To me, their job request was not just manipulative, it didn't seem like something Machine Learning could solve. If you were to prepare a dataset to solve this problem, you'd have people, specifically digital communications associates like my Patagonia friend, generate thousands of differently worded emails. You’d send them all out to your voter lists, and then you’d measure the click-through donations per email. You would take all that info, and have your algorithm attempt to predict the total amount of donations given based on the features of the words in the email, such as sentiment, phrases, subject line, or word choice. I'll refer to this as the Naive Problem.

The Naive Problem IS something machine learning can solve. The issue is that this problem is more than a stone’s throw from the goal Anne Lewis is targeting. Anne Lewis employs her Strategies to try to win elections, not (optimize payment quantities per email sent).

There are two big leaps to cross to get from The Naive Problem over to the problem of using email to help win elections. I shall explain them to you now.

First, there is Goodhart’s Law. This law states that

"When a measure becomes a target, it ceases to be a good measure"

The easiest parable for this law is that when I was studying for the SAT, which is a measure trying to predict roughly the amount schools will make back in alumni donations by letting me attend their undergraduate program, of course, what I optimized for is answering correctly specific questions known to be asked on the SAT, and so what colleges actually optimized for instead were, the kids that were so trodden down by the public school system that they felt the need to sacrifice an important period of their social growth for a name on their resume, like me.

Anywho, Goodharts law pops up everywhere, like how when companies optimize for quarterly shareholder value, they’re not optimizing for the long term health of a company. It also pops up when it comes to sweets, where humans think that the sweeter a food is, the better it is to eat, which was fine when we were picking berries off trees to tell us what was ripe, but the hyper-optimization by Coca Cola gave everybody the beetus.

How does it apply to my machine learning problem? Well, getting good amounts of donations for each email Jaime Harrison sends out is fine as a vague heuristic, but when you ask a stupid algorithm to optimize it, you get things like "HELP PLEASE FUCKING READ This EMAIL". Which given our problem formulation may well be optimal, but is probably doing more harm than good for Jaime.

Why specifically isn't it good for Jaime? The answer is due to the second concept I will present in this post, and the last. Its name is Second-Order Effects.

My parable for this one involves Netflix, who recently came under fire for canceling too many shows before they had their plots resolved, such as The OA. Their stupid algorithm had told them that to keep The OA show running, they would lose money. That’s probably true. The path from there to their goal of being an Iconic Company involves

1. Reluctance of viewers to take a risk watching a show that hasn't completed yet

2. Users defecting out of anger their favorite show was canceled early

3. TV critics who review shows being turned off and influencing their audience away from the platform.

4. The best and brightest directors taking their content to somebody who might give their show a fair shot at completion next time.

Netflix's model might have accounted for 1 and 2, but you can't use machine learning to target 3 or 4. It's just not in the data, and so you can’t be data-driven and win this fight.

So, this whole cycle, Jaime Harrison probably annoyed the shit out of you with his spammy emails, because the person they hired instead of me told them he or she probably he could solve their problem, and maybe now when you think of Jaime Harrison the man, you think of the grossness of the emails with his name on them filling up your inbox, and not his progressive-lite policies.
