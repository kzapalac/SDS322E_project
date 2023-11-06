Can a Learning Orientation Reduce In-Group Bias?
================
Kaylee Billstone, Paulina Brown, Jaqueline Marroquin, Christian Ozuna,
Kirsten Richards, and Kennedy Zapalac
2023-10-02

# Project Overview

**What is in-group bias and why does it matter?**

In-group bias is the preferential treatment of people with whom you
share a common identity, such as gender, race, or culture. In-group bias
can be harmful when it leads to unfair outcomes, such as when a
perfectly qualified job candidate is not hired because of their race.
Current research is focused on reducing in-group bias to mitigate its
harmful effects.(Wang et al. 2015)

**Our aims:**

Along this line, we are investigating if in-group bias can be influenced
by priming people with a learning versus performance orientation. A
learning orientation is other-focused (trying to get to know another
person), whereas as performance orientation is self-focused (trying to
make a good impression). Other studies have demonstrated that in-group
bias is influenced by the priming received, so we expect the priming our
participants received will affect their in-group bias (Bettencourt,
Charlton, and Kernahan 1997). Specifically, we will:

1.  Determine how perspective taking, empathetic concern, and altruism
    is different among in-group versus out-group members. Do our
    participant’s display an in-group bias such that they have an easier
    time understanding, express more empathy for, and exhibit altruistic
    behavior toward in-group members?
2.  Determine if the priming received (learning versus performance)
    influenced perspective taking, empathetic concern, and altruism
    towards out-group members.

A few other aims we could pursue later:

1.  How does trait-level orientation influence the effectiveness of the
    priming received in reducing in-group bias?
2.  Investigate whether there are gender-related differences in the
    effectiveness of the learning orientation prime in reducing in-group
    bias.
3.  Perform textual analysis on the participants’ responses to the
    person going through a hard time. We could extract additional
    variables, which could be used to understand in-group bias. For
    example, can we use the sentiment expressed to predict how
    empathetic someone rated themselves as? Could we predict if someone
    had received a learning or performance orientation prime based on
    their language? Or does someone’s trait-level orientation strongly
    influence their language usage?

**Our dataset:**

Our dataset can be accessed
[here](https://github.com/kzapalac/SDS322E_project/blob/main/LP_Dictator.csv).
You can also reference the survey outline
[here](https://github.com/kzapalac/SDS322E_project/blob/main/LP_Dictator.pdf)
to understand the dataset better.

The sample includes white adults who identified as male or female, and
the survey was conducted entirely online. Participants were asked to
write a paragraph about themselves, and they received a learning or
performance prime. Next, they read about a gender-matched in-group or
out-group member (e.g., white or black stranger) going through a hard
time. Then, the participants wrote a letter of support to this person,
filled out a 5-item questionnaire about how easy it was to take the
other person’s perspective, a 1-item measure about how much empathetic
concern they felt for the person, and play a one-shot dictate game.
Trait-level learning and performance orientation was also assessed.
There were two quality measures, which may reduce the size of the
dataset, including an attention check and asking whether or not their
responses should be included.

Overall, there are:

- 2 independent variables: in-group/out-group stranger and
  learning/performance orientation

- 3 dependent variables: perspective taking, empathetic concern,
  altruism (via dictator game)

- 2 potential covariates: trait level learning/performance orientation,
  gender

# Exploratory Data Analysis

### In-Group vs. Out-Group Empathetic Concern, Altruism, and Perspective Taking

![](readme_files/figure-gfm/empathetic%20concern-1.png)<!-- -->![](readme_files/figure-gfm/empathetic%20concern-2.png)<!-- -->

| inOrOut |   n |     mean |       sd |        se | lower_ci | upper_ci |
|:--------|----:|---------:|---------:|----------:|---------:|---------:|
| in      |  65 | 5.246154 | 1.500320 | 0.1860919 | 4.881414 | 5.610894 |
| out     |  59 | 5.372881 | 1.230339 | 0.1601765 | 5.058935 | 5.686827 |

**Description of graph:** The graphs above display participants’
self-rated empathetic concern for an in-group versus out-group stranger.
Participants were able to rate their empathetic concern on a scale from
1 (none) to 7 (an extreme amount). In the box plot, we can see that the
median response for empathy was slightly greater for users who received
an in-group response or an out-group response, but overall the
empathetic concern expressed across both groups is fairly high. The
in-group had a larger range of empathy levels felt than the out-group.
In the bar graph, we can see that the mean level of empathy for in-group
and out-group responses are almost the same. The summary table tells us
that the mean empathy level for the in-group is 5.25 (+/- 0.365) and the
mean empathy level for the out-group is 5.35 (+/- 0.304). Although
participants exhibit very slightly more empathetic concern for out-group
strangers within this sample, this difference likely isn’t significant
since the error bars overlap. There is a chance that the reason we do
not see a difference in empathy for in and out groups is because of the
way that participants were primed. We explore this more below.

**Hypothesis based on graph:** Whether a participant received an
in-group or out-group response had little to no impact on the level of
empathy they felt for the person they read about.

![](readme_files/figure-gfm/altruism-1.png)<!-- -->![](readme_files/figure-gfm/altruism-2.png)<!-- -->

| inOrOut |   n | median |     mean |       sd |        se | lower_ci | upper_ci |
|:--------|----:|-------:|---------:|---------:|----------:|---------:|---------:|
| in      |  65 |      0 | 5.215385 | 7.861084 | 0.9750474 | 3.304292 | 7.126478 |
| out     |  59 |      5 | 6.745763 | 8.146489 | 1.0605825 | 4.667021 | 8.824504 |

**Description of graph:** As part of an altruism test, participants were
compensated with 25 cents for participating in this study, but they were
able to share this money with the stranger they read about. The violin
graph depicted above displays the results of this altruism test. The
in-group is on the left and out-group is on the right within this plot.
Regardless of whether it was an in-group or out-group stranger, most
participants chose to keep the majority of the money for themselves,
represented by the wider distribution at lower values. Participants in
the out-group may have been a little more giving since the distribution
is more spread out. To examine this difference further, we created a bar
plot representing the average money given with error bars. It seems that
people in the out-group condition were slightly more giving on average
in this sample, but this difference may not be represented in the
population since the error bars overlap.

**Hypothesis based on graph:** We hypothesize that there is little to no
in-group bias present in regards to the participants exhibiting
altruistic behavior toward in-group members. People seem no less likely
to give money to an out-group member than they do to an in-group member.
In fact, they may have been slightly more likely to give to give to an
out-group member than an in-group member. This is demonstrated by the
wider distribution at higher values for the violin plot and the greater
mean for the out-group in the bar plot. Perhaps in-group bias is being
obscured in this sample because the learning prime reduced in-group bias
for a portion of the sample.

![](readme_files/figure-gfm/perspective%20taking-1.png)<!-- -->![](readme_files/figure-gfm/perspective%20taking-2.png)<!-- -->![](readme_files/figure-gfm/perspective%20taking-3.png)<!-- -->

| inOrOut |   n |     mean |        sd |        se | lower_ci | upper_ci |
|:--------|----:|---------:|----------:|----------:|---------:|---------:|
| in      |  65 | 5.880000 | 1.1284946 | 0.1399725 | 5.605654 | 6.154346 |
| out     |  59 | 5.752542 | 0.9793305 | 0.1274980 | 5.502646 | 6.002438 |

**Description of graph:** Participants expressed how easy it was to
understand the perspective of the stranger whose paragraph they read.
They answered 5 questions, and these questions were averaged to obtain
each participant’s average ease of perspective taking. Higher scores
represent better perspective taking. In the violin plot, it looks like
participants in the in-group condition had a slightly easier time take
the perspective because the distribution is wider at the highest values.
The boxplot displays the same thing, but we just wanted to explore the
data in a few ways. Since there didn’t seem to be a clear difference
between the in-group and out-group conditions in the distribution plots,
we created a bar plot to more easily detect a difference. In the
boxplot, it does appear that participants within this sample had a
slightly easier time on average understanding an in-group stranger, but
this difference doesn’t appear to be significant since the error bars
overlap.

**Hypothesis based on graph:** We hypothesize that there isn’t a
difference between people’s understanding of in-group and out-group
strangers because there isn’t a clear difference in the distributions
depicted in the violin plot or in the means in the bar plot. Perhaps the
learning prime was successful, so it’s obscuring the difference in
perspective taking for in-group and out-group strangers.

**Overall, there doesn’t seem to be a difference in people’s empathetic
concern, altruism, or perspective taking for in-group vs. out-group
strangers within this sample, which is counter intuitive given the
well-demonstrated existence of in-group bias. The learning prime may
have been successful in reducing in-group bias, obscuring the difference
unless we separate by both conditions (in-group vs. out-group and
learning vs. performance priming). We explore this below.**

### Influence of Priming on Out-Group Perspective Taking, Empathetic Concern, and Altruism

![](readme_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->![](readme_files/figure-gfm/unnamed-chunk-1-2.png)<!-- -->![](readme_files/figure-gfm/unnamed-chunk-1-3.png)<!-- -->

| inOrOut | priming_received |   n |     mean |       sd |        se | lower_ci | upper_ci |
|:--------|:-----------------|----:|---------:|---------:|----------:|---------:|---------:|
| in      | learning         |  35 | 5.685714 | 1.078437 | 0.1822890 | 5.328428 | 6.043001 |
| in      | performance      |  30 | 4.733333 | 1.760355 | 0.3213954 | 4.103398 | 5.363268 |
| out     | learning         |  28 | 5.535714 | 1.070899 | 0.2023810 | 5.139048 | 5.932381 |
| out     | performance      |  31 | 5.225807 | 1.359158 | 0.2441121 | 4.747347 | 5.704266 |

**Description of graph:** We created the violin plot and the box plot to
examine the distributions, but the following description focuses on the
bar plot. Within the study’s in-group, participants who were primed with
a “learning orientation” exhibited a mean empathetic concern score of
5.69, whereas those who received the “performance orientation” priming
displayed a slightly lower mean score of 4.73. In the “learning
orientation” in-group, the empathetic concern scores exhibited
relatively low variability, as evidenced by the narrower confidence
interval (5.33 to 6.04) and a smaller standard deviation (1.08). This
suggests a more consistent range of scores within this group.
Conversely, the “performance orientation” in-group displayed higher
variability, with a wider confidence interval (4.10 to 5.36) and a
larger standard deviation (1.76). These statistics indicate greater
diversity in empathetic concern scores within this group, signifying
less consistency compared to the “learning orientation” group.
Furthermore, the error bars do not overlap, meaning that we can safely
assume a true difference exists between the empathy expressed for
in-group participants depending on the priming they received.

In contrast, for the out-group, individuals subjected to the “learning
orientation” priming had an average empathetic concern score of 5.48,
while those exposed to the “performance orientation” priming yielded a
mean empathetic concern score of 5.23. In the “learning orientation”
out-group, the empathetic concern scores showed moderate variability, as
indicated by the confidence interval (5.10 to 5.87) and standard
deviation (1.09). Meanwhile, in the “performance orientation” out-group,
there was also variability, with a confidence interval (4.75 to 5.70)
and a slightly higher standard deviation (1.36). This implies a range of
scores with some differences within this group, reflecting a moderate
level of variability. Unlike the in-group condition, the error bars do
overlap in out-group graph. This indicates that the observed difference
in empathetic concern dependent on the priming received is not
significant. There may not be a difference in the empathetic concern
expressed for out-group strangers when a different priming is received
for some reason.

Lastly, there doesn’t seem to be a significant difference between the
empathetic concern expressed by in-group or out-group participants who
received the same priming. For example, the mean empathy for in-group
participants who received the learning orientation was 5.69 (+/- 0.357)
whereas the mean for out-group participants who received the learning
orientation was 5.48 (+/- 0.397). Since the error bars overlapped, this
was not a significant difference. The same is true for in-group and
out-group participants who received the performance orientation because
their error bars overlap.

**Hypothesis based on graph:** Based on the graphs above, we hypothesize
that only in-group participants (not out-group) primed with a learning
orientation will express more empathetic concern than those primed with
a performance orientation. Although participants who received the
learning orientation trended towards expressing more empathetic concern
in the in-group and out-group condition, the error bars indicate that
the difference was only significant for participants in the in-group
condition.

![](readme_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->![](readme_files/figure-gfm/unnamed-chunk-2-2.png)<!-- -->![](readme_files/figure-gfm/unnamed-chunk-2-3.png)<!-- -->

| inOrOut | priming_received |   n |     mean |       sd |       se | lower_ci |  upper_ci |
|:--------|:-----------------|----:|---------:|---------:|---------:|---------:|----------:|
| in      | learning         |  35 | 5.171429 | 8.074964 | 1.364918 | 2.496189 |  7.846668 |
| in      | performance      |  30 | 5.266667 | 7.741217 | 1.413346 | 2.496508 |  8.036826 |
| out     | learning         |  28 | 5.750000 | 5.898054 | 1.114627 | 3.565330 |  7.934670 |
| out     | performance      |  31 | 7.645161 | 9.758922 | 1.752754 | 4.209763 | 11.080559 |

**Description of graph:** The violin and boxplot are visualizations of
Altruism distributions found between people that were chosen for
In-Groups vs Out-Groups that received either learning or performance
priming. The barplot shown is the average level of Altruism found
between the same testing groups. To examine the barplot further, four
means of Altruism levels were observed. Those who were in the In-Group
and received learning priming had a mean of 5.17 points with a standard
error of 1.36. However, those in the In-Group but with performance
priming were observed to have a mean Altruism score of 5.27 with a
standard error of 1.41. Similarly, for the Out-group, the learning
priming group received a mean Altruism score of 5.55 and standard error
of 1.09. Like the In-Group, the Out-group of people who received
performance priming had a higher Altruism average than those in the
learning priming group with an average of 7.65 and standard error of
1.75. In the In-Group and Out-Group, each group that received
performance priming had higher means than those in learning priming
groups.

Due to error bar overlap for the In-Group, this is not a significant
variance between learning and performance priming groups. Similarly,
there is no significant difference in altruism for out-group participans
who received a different priming because the error bars overlap. In
fact, all of the error bars overlap, so there is no difference in
altruism for any combination of in-group and out-group with learning or
performance priming.

**Hypothesis based on graph:** Based on the graphs above, we hypothesize
that there is no difference in altruism for any combination of in-group
and out-group with learning or performance orientation.

![](readme_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->![](readme_files/figure-gfm/unnamed-chunk-3-2.png)<!-- -->![](readme_files/figure-gfm/unnamed-chunk-3-3.png)<!-- -->

| inOrOut | priming_received |   n |     mean |        sd |        se | lower_ci | upper_ci |
|:--------|:-----------------|----:|---------:|----------:|----------:|---------:|---------:|
| in      | learning         |  35 | 5.971429 | 1.0325786 | 0.1745376 | 5.629335 | 6.313522 |
| in      | performance      |  30 | 5.773333 | 1.2403930 | 0.2264637 | 5.329464 | 6.217202 |
| out     | learning         |  28 | 5.835714 | 0.8486217 | 0.1603744 | 5.521380 | 6.150048 |
| out     | performance      |  31 | 5.677419 | 1.0926145 | 0.1962394 | 5.292790 | 6.062049 |

**Description of graph:** In the violin plot and boxplot above, we
wanted to see the distribution for the ease of perspective taking for
people that were chosen for In-Groups compared to Out- groups based on
the priming that each participant received. The distributions look
fairly similar across the in-group and out-group participants, although
perhaps there is a bit more spread for the in-group participants. Then
within in-group and out-group conditions, the priming received doesn’t
seem to have influenced perspective taking very much either. Perhaps
there is slightly more spread for people who received a performance
priming both within the in-group and out-group condition, but there is
no clear difference once again.

To better visualize the difference between each of the conditions, we
plotted the means with error bars. Within the In-Group participants,
those who received the learning prime had a mean of around 5.97, which
was slightly higher than the mean of those who received the performance
prime, which was around 5.77. In the Learning Prime In-Group, the upper
confidence interval was about 6.313 and the lower confidence was about
5.629, with a difference of about 0.684. This means that there was
slightly less variability in perspective taking scores for the Learning
Prime In-Group, as the Performance Prime In- Group had a upper
confidence interval of about 6.217 and the lower confidence was about
5.329, with a difference of about 0.888. This would also mean that more
people in the Learning Prime In-Group chose almost the same scores than
people in the Performance Prime In-Group. Since the error bars overlap,
the difference observed between the perspective taking of people in the
in-group across the 2 orientations was likely not significant.

Within the Out-Group participants, those who received the learning prime
had a mean of around 5.79, which was slightly higher than the mean of
those who received the performance prime, which was around 5.67. In the
Learning Prime Out-Group, the upper confidence interval was about 6.097
and the lower confidence was about 5.489, with a difference of about
0.608. This means that there was also slightly less variability in
perspective taking scores for the Learning Prime Out-Group, as the
Performance Prime Out-Group had a upper confidence interval of about
6.055 and the lower confidence was about 5.299, with a difference of
about 0.756. This would also mean that more people in the Learning Prime
Out-Group chose almost the same scores than people in the Performance
Prime Out-Group.

In the error-bar plot, the error bars for all of the groups overlap,
with the Learning Prime In-Group and Performance Prime In-Group
overlapping each other, and the Learning Prime Out-Group and Performance
Prime Out-Group overlapping each other as well. This means that there is
likely no significant difference in perspective taking scores between
In-Groups and Out-Groups based on the priming that each participant
received.

**Hypothesis based on graph:** Based on the graphs above, we hypothesize
that both in-Group and out-group participants do not show much of a
difference in perspective taking regardless of their priming received,
as there were little to no differences in the plots. An in-group bias
does not appear to exist within our sample since the plots are
relatively the same across in-group and out-groups. However, the lack of
in-group bias is likely not due to the effectiveness of the learning
orientation because there don’t appear to be significant differences
between the learning and performance orientation groups within the
in-group or out-group condition.

**There doesn’t seem to be much in-group bias in our sample, but we
can’t attribute this lack of bias to the learning priming. For the most
part, similar empathy, altruism, and perspective taking was exhibited
across people who received different priming and read about the same
kind of stranger (in-group or out-group).**

# References

<div id="refs" class="references csl-bib-body hanging-indent">

<div id="ref-bettencourt1997" class="csl-entry">

Bettencourt, B.Ann, Kelly Charlton, and Cyndi Kernahan. 1997. “Numerical
Representation of Groups in Cooperative Settings: Social Orientation
Effects on Ingroup Bias.” *Journal of Experimental Social Psychology* 33
(6): 630–59. <https://doi.org/10.1006/jesp.1997.1334>.

</div>

<div id="ref-wang2015" class="csl-entry">

Wang, Chenbo, Bing Wu, Yi Liu, Xinhuai Wu, and Shihui Han. 2015.
“Challenging Emotional Prejudice by Changing Self-Concept: Priming
Independent Self-Construal Reduces Racial in-Group Bias in Neural
Responses to Other’s Pain.” *Social Cognitive and Affective
Neuroscience* 10 (9): 1195–1201. <https://doi.org/10.1093/scan/nsv005>.

</div>

</div>
