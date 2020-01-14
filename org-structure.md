One of the things I've been starting to think about is organizational structure.  In particular, what is the boundary between "us" and "them".  

# "Us" versus "Them"

There are some aspects of all companies that I'm 90% certain are related to the tribalism of humans.  I've seen them in enough of the employee surveys across organizations and companies to believe they're universal.  Let's lay a few of them out there.

## Our team is easy to work with.  Other teams are a nightmare to work with.

This is incredibly important, because the only difference is perspective.  The other teams are saying the same thing about your team, unless you work **really** hard to change this.  Additionally, it means that the teams you view as difficult to work with, don't see themselves that way.  Why not?  That's a great question, and I don't have an answer, but the first step is recognizing the realities.  

## If <insert team in a different org> just reported into our org, we could fix this.

This is going to be the fundamental question that leads to the rest of this document.  I've spent some time thinking about it, and realized that if you did that with every problem organization, pretty soon your org would be so large, that you've re-created the same silos.  Think about it for a minute. Everyone is part of one company.  You all meet at the CEO/Board, so why do all large companies have this problem?  So I got to thinking about what is that inflection point.  No matter how much you like the leader of your organization, when does the organization size make it so that they can't have a cohesive "it's all us" culture?

Then I remember Dunbar's Number.

# Dunbar's Number

The [Wikipedia page](https://en.wikipedia.org/wiki/Dunbar%27s_number) exists for a reason, but I'll just quickly summarize.  [Robin Dunbar](https://en.wikipedia.org/wiki/Robin_Dunbar) looked at human and primate brains to determine what was the range or social groups that could be maintained.  At a 95% confidence interval, it was between 100 and 230, with a mean of 148, which is rounded to 150.

Now 150 is interesting because, independent of Dunbar's Number, there are [other examples](https://www.weforum.org/agenda/2016/12/the-weird-thing-that-happens-when-companies-get-bigger-than-150-people) of companies hitting this number and seeing dramatic changes in how the company operates. 

There is some discussion on whether or not this number is different in non-survival groups, but there seem to be enough independent confirmations that it's at least a credible hypothesis.

# Assertion: An "Us" organization is capped at ~150 people

If this is the case, then what are the other organizational constraints?  Given that we're talking about software development, one constraint is going to be the size of our development teams.  Agile is the current way of the world, so what is an ideal scrum team?  Well, that's a team that develops all of it's commitments on time with nice burndown charts, but that isn't what I meant.  There is pretty strong consensus that it has between 3 and 9 members.  Separate from the scrum size, the consensus is that the best team sizes are between 5 and 8.  I actually think you can be a bit on the higher side (up to 10) if you have great line managers, but 8 is probably a good upper goal.

Now, with all of this, teams no greater than 8, and a maximum organization size of 150 we can now figure out the number of layers this organization could have.  5^3 is 125 and 8^3 is 512.  Going the other way, the cube root of 150 is ~5.3, which means that the largest effective "Us" organization is three layers of management deep.  Every line manager has ~5, and every level above that has 5.  That puts that layer at an org size of 25 individual contributors and 30 total (25 IC + 5 managers).  The layer above that also has 5, and that puts it at 125 IC and 155 total (30 * 5 + 5).

![Idealized org chart](Images/org-chart.png)

# The difference between structure and responsibilities 

Now, until this point I've been talking about this as strictly a math problem, but I think the real world should probably get included eventually.  

The reality is that organizations and teams exist in order to deliver business outcomes.  The idea that a manager only manages directly, and the next level up only manages indirectly, and that organizations will be constantly rebalanced [B-tree](https://en.wikipedia.org/wiki/B-tree) is fantasy.  But, what is important is to recognize that if you understand the upper-bounds you now have a framework for maximizing your organizational potential and achieve better results with less "political" churn.

# The role of leadership and personal relationships

I do think that there are ways that these limits can be expanded, but I don't think it can be systemized/scaled.  If you have a particularly effective leader, or you have personal relationships that cross Dunbar boundaries, then the chances of reducing "Us vs Them" as well as increasing org size to the upper bounds are possible.  But, that relies on individual personalities and relationships and I just don't know how you can create those.  You can foster it, and it's why "team building" and "leadership offsites" are useful.  However, in my experience true close relationships and leadership like this are rare, so you shouldn't plan on it.

# Conflict between Conway's Law

[Conway's Law](https://en.wikipedia.org/wiki/Conway%27s_law) (roughly) says that organizations will design systems that match their organizational structures.  I think experience will show that this is true for our Dunbar limit as well.  Organizations will decide to build tools within their org because they will argue they have unique requirements, or this other tool doesn't do quite what they want, or ... any number of excuses.

So, where is the conflict?  

One way that organizations attempt to increase their effectiveness is through centralization and co-location.  Which is all good, but then creates brittle software at scale.  I'll cover that more in my [Normal Accidents](normal-accidents.md) page, when I get around to creating it.  


## Additional Reading

* [Dunbar, Altruistic Punishment, and Meta-Moderation](http://www.lifewithalacrity.com/2005/03/dunbar_altruist.html)
* [The Dunbar Number as a Limit to Group Sizes](http://www.lifewithalacrity.com/2004/03/the_dunbar_numb.html)
* [Dunbar Number & Group Cohesion](http://www.lifewithalacrity.com/2005/10/dunbar_group_co.html)
* [What Dunbar’s Number means in business today](https://www.wework.com/ideas/dunbars-number-means-business-today)
* [The magic number: this is what happens when companies hit a certain number of employees](https://www.weforum.org/agenda/2016/12/the-weird-thing-that-happens-when-companies-get-bigger-than-150-people)
* [Organization Design: Fashion or Fit?](https://hbr.org/1981/01/organization-design-fashion-or-fit)
* [Do You Have a Well-Designed Organization?](https://hbr.org/2002/03/do-you-have-a-well-designed-organization)
* [Structural Determinants of Organizational Effectiveness](https://ibimapublishing.com/articles/JOMS/2014/273364/)
* [An Elegant Puzzle: Systems of Engineering Management](https://www.amazon.com/Elegant-Puzzle-Systems-Engineering-Management/dp/1732265186)
