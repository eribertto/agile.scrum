After watching this video, you'll be able to describe sprint planning, explain
why having a sprint goal is important, describe how to run a sprint planning
meeting, assign estimates and labels to stories, produce a sprint plan. In the
scrum process, we've looked at product backlog and backlog refinement, and we're
now doing a sprint planning meeting, which will hopefully produce a sprint
backlog. Sprint planning is the meeting in which you determine what stories are
going to be in the next sprint, how much can we accomplish in the next two
weeks.  We do that by producing a sprint backlog. So, the sprint planning
meeting: Who should attend? Well, that should be the product owner, the scrum
master, and the development team. We don't invite stakeholders or anybody like
that to this meeting. It is just the core team.  The three roles in scrum: The
product owner, the scrum master, and the rest of the team. When I say
development team, I mean software engineers, testers, uh, operations folks. If
you're doing DevOps, uh, maybe business analysts. So, whoever is on the team
that is building the thing that you're delivering. A cross-functional team, not
just software engineers. So, we have to talk about goals here.  This is very,
very important. Each sprint should have a goal.  For some reason, it's hard for
some product owners to say what the goal of a sprint is.  They're thinking, I
need the whole thing done but they've got to think, what can I get done in the
next two weeks? And so, it's very important that the product owner articulate
the goal. And then, here are the stories in the product backlog that support the
goal so that everybody knows why they're doing the stories and how that story is
going to help us achieve whatever goal it is, whatever capability, whatever you
want to add to the product that we're building. And so, it's important for the
whole team to understand this. Sometimes you're in the middle of a sprint, um,
you know, and you have some questions about how to do something and you're like,
okay, what was the goal? You know, am I getting off on some tangent here, on
some other path? The goal was to deliver this capability.  Let me make sure I
don't over-code it, over-engineer it.  Let me make sure I meet the goal of
delivering whatever it is we decided to deliver to the customer. So, the
mechanics of sprint planning, what the development team is going to do, and,
this is a development team activity, they're going to take stories from the top
of the product backlog and they're going to move them into the sprint backlog,
and they're going to do this on and assign story points.  If you haven't had
story points, if you do have story points from the backlog refinement, they will
check to make sure they agree with those story points because they probably
didn't create them. So, the development team decides how big a story is. They're
the ones that have to commit to it, right?  So, they have to make sure they're
comfortable with the story points.  Sometimes they do a little something called
planning poker, uh, where they all, you know, hold up, I think, it's a three, I
think, it's a five, and they talk about why they think it's small or medium, and
then they all agree, yep, that's a medium story, I get it.  So, very important
to agree on how big these stories are and then they want to make sure that each
story contains enough information so that they can start working on it.  You
don't want to be asking questions in the middle of a sprint.  You want to be
able to take the next story off the backlog and know that everything in it is
there that you need to start working. And so, it's important that all the
developers understand, all the testers, all, everybody on the team understands
what that story is about in case they're the one that pulls it off the backlog.
And then, finally, you stop adding stories when you hit the team's velocity. So,
this begs the question, what is team velocity?  I’ve mentioned it a few times
now, right? Velocity is the number of story points that a team can execute in a
single sprint, right? So, you take all the story points in the sprint, and
sprint, and that becomes the team's velocity. This is critical because it's
going to change over time as estimates get more accurate. It will change as the
team gets more, uh, competent at implementing stories. It's going to change so
the velocity could change over time. Hopefully it will get better and better and
better, but here's the key piece: you cannot compare the velocity of two teams.
Velocity is a personal thing. Each team decides what's a medium, right? And so,
a medium for one team might be bigger than a medium for another team. So, it's
not fair to compare their velocity.  Also, some team might say, hey, two is a
medium, one is a small, right?  Three is a large. Another team might say five is
a medium, threes are small, eight is a large. Well, obviously, the team that
picks the bigger numbers is going to have the bigger velocity, but they may
actually be doing less work, so unless all the teams agree on what a medium
story is, and all the teams agree on what numbers to use, which they don't
always do because the teams are independent, you cannot compare the velocity of
two teams. Not fair unless everybody's using the same measurements. So, one of
the first things you want to do when you do sprint planning is create a
milestone. Now, in ZenHub, you can use a milestone, which is part of GitHub, but
ZenHub has just introduced something called sprints.  And so, sprints act like
the old milestones and you can use either.  I’m still using milestones because I
can still track them in other ways in GitHub.  The sprints are unique to ZenHub
but they have some cool automation where you can move stories from sprint to
sprint. So, you might want to look into that, but right now, I have my teams
creating milestones. So, you create the milestone, and you give it a title. I
usually keep the title short because they show up in drop down lists, right? So,
sprint one, colon, you know, deployed to cloud… just something really short so
we know what… sometimes the numbers are relevant, but we just know that sprint
is, uh, deployed to cloud. And then we want to give it a description and the
description should be the goal, right, so that everybody understands what are we
doing this sprint. Look at the description of the milestone, that goal, that's
what we're all here to do. So, make sure that we adhere to that goal and then
you give it a duration. And I like to have my sprints be two weeks.  Some teams
can do one week, I think it's a little short, but you really don't want to go
three, four, five weeks too many things can change.  I like to keep two-week
sprints. It's a nice cadence that's easy for most teams to do. So, let's look at
the user interface for creating a new milestone. So, one of the things we want
to do is we want to give it a title. So, I’ve called this sprint one colon
single counter, right? We just want to implement a single counter, that should
tell you right there the multiple counter store is not going to be in the
sprint, right? The sprint is just about the single counter and then in the
description, I like to put the goal. The goal is to get a single counter working
and deploy to the cloud, right? So, I’ve kind of stated this is what we're all
running for. We want to get it in the cloud, we want to get just a single
counter working, right? And this is what we're going to commit to our
stakeholders. And then I’ve got to give it some dates.  A start date and an end
date. And so I might say, yep, I’m going to start on Monday the 7th, and then
the following Friday the 18th is when we're going to be done with this two-week
sprint. And so, now I’m all ready to create that milestone. Just a title, a good
description, that gives you the goal and the start and end dates, so we'll
create a milestone.  So, now if we look at where we left our Kanban board, we
had some groomed stories in the product backlog. Some ungroomed stories in the
icebox, and we don't have to worry about anything but the product backlog and
the sprint backlog.  The goal here is to build a sprint backlog from the product
backlog.  So, if we look at it, we've got our stories. They don't have any story
points, so we're going to have to assign them. Notice at the top of the sprint
backlog, it says zero story points. The tool will track how many story points
you have in each one of the pipelines, and so, that's going to tell us when we
reach our team velocity.  So, let's look at the first story. So, I open the
first story and I want to assign it an estimate, so maybe we talk it over as a
team and the team says, this looks like a rather large story because it's, you
know, it's setting up the initial, you know, counter, the increment, and then
getting the values, there's a number of things in here.  Maybe they say, "This
is a large one. We're going to make it an eight." And then we assign it to the
sprint milestone of sprint one. So, now we know that this is in the sprint, and
it's got, uh, an estimate, uh, and so we'll close that one.  Now when it shows
up in the product backlog, it has an eight in the circle to show us that it's
eight story points. We still have our label and it's also been assigned to the
sprint, so now we'll move that one over into the sprint backlog and the sprint
backlog now shows us you've got eight story points in the sprint so far.  So,
let's look at the next one. We open it up, we talk about it as a team.  Is this
big? Is it small? Medium? Large?  What is it? Maybe the team decides, hey, this
is a medium, right, we know how to do this. This is something that we think is
kind of a medium story, get it done in a couple of days, less than a week, um,
and so that becomes a medium story. And so, the next thing we want to do is
assign it to the sprint. So, now we've got this story assigned to the sprint.
It's a medium story.  We go back to our Kanban board, we see that the story
points have been assigned and we drag and drop that one over into the sprint
backlog and now we're at 13 story points.  And we'll go look at the next story.
So, this is what you're doing during the sprint planning meeting, right? You're
looking at each one of these stories.  You're talking about it. This one's a
technical debt story, we talk about it with the team, the team decides this
one's also a medium, we assign it to the sprint milestone and then we save it
and that one shows up with all decorations and we drag and we drop that one
into, um, the sprint backlog. And so, you continue to do this until you hit your
velocity. So, let's say the team's velocity is 18 story points, um, and so we
stop at this point and say, hey, we've got enough things in our sprint plan, we
don't want to over-commit. The past has shown us that we can do about 18 story
points, and that's the beauty of story points, it's not wall clock time.  It's
like, you know, we could do a couple smalls, a medium, maybe a large, or maybe,
two mediums and a large, right? It's not the number of stories… every sprint…
it's given the estimates and given our past track record of implementing 18
story points or 20 story points per sprint, we don't want to exceed that
commitment in the next sprint.  In this video, you learned that it is the
product owner's responsibility to present the sprint goal, it is the development
team's responsibility to create a sprint plan, and a sprint plan is created by
moving stories from the product backlog into the sprint backlog until the team's
velocity is reached.