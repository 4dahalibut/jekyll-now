---
layout: post
title: Making healthcare in ML fair, and measures of how to do it
---

So [this article](https://science.sciencemag.org/content/sci/366/6464/447.full.pdf) has been making the rounds recently . The idea is that there are algorithms used to recommend patients for more intensive care which predict using the "label" of the future cost of the patient.  While using a label related to cost is easy because the data can be collected simply, and it is a simple numeric value, it embeds the history of black ppl getting less healthcare done, and the paper claims that this means that blacks have significantly higher amount of sickness conditioned on this risk score than white ppl. The question of whether "amount of sickness" is tied to their underlying metric of number of chronic conditions seems open to me, but opening up the conversation of the use of money as a proxy for other labels seems like a useful addition to the public dialogue.

I also liked the summary of three ways of measuring algorithmic bias:
* Accuracy: How well does the algorithm predict future cost related to the actual future cost, for blacks and for whites?
* Decision Parity: Are the same amount of blacks and whites recommended for intensive care, regardless of underlying conditions?
* Similarity of False Positive / False Negative rate by race - How often does the algorithm overshoot vs undershoot the real estimate across race?
It has been proven that achieving the second and third of these at the same time is impossible even approximately, except for in trivial situations such as perfect prediction rate, or if the real rate of the labels being a certain value is the same across groups. Even in the second case, the solution to solving the second and third of these fairness criteria at the same time is pretty hard. However, apparently it is possible to make a model have similar false positive and false negative rates across groups.
