After watching this video, you'll be able to describe what a Kanban board is,
explain what each pipeline is used for, and summarize the workflow across a
Kanban board. So there are lots of Agile planning tools out there. But one thing
you need to understand is that a tool won't make you agile, you really have to
have the Agile mindset to become agile. Tools will support your Agile process,
but you have to have the process first. I've seen a lot of people who haven't
had training try to make a Kanban board look like a Gantt chart. Those are two
different things, two different ways of doing project management. So it's really
important that you understand this. And there are lots and lots and lots of
Agile planning tools. Most of them do the same thing, but some of them are a
little more complicated than others. I just need epics and stories to describe
my plans. Some of them go into tasks and subtasks. And I don't want, that's
micromanaging in my estimation, right? Just epics and stories are fine. And so I
like to use a tool called Zen hub. And we're going to use ZenHub for this
course. So what is Zen Hub? Well, it's a plugin to GitHub. It's one of the
reasons I like it. My developers stay in GitHub and they use this Zen Hub
plugin. What Zen Hub does is it allows you to add project management tools, a
Kanban board, to manage your projects while you remain in GitHub. So that's
pretty important to me. The other is, is that Zen hub is customizable. It starts
out with a set of columns, which are called pipelines, in your Kanban board, but
you can customize them to be anything you like. You can make it as complex or as
simple. I like to keep them simple. So why do we use it? Well, one of the main
reasons is because it uses GitHub issues. It's not another tool with another
thing that I have to go off and edit. That's one of the problems I find is if
you're using too many tools, and a developer has to go someplace else to update
the status, that status is going to be out of date 100% of the time. Because as
soon as they updated, they're going to go on and do something else, and it's not
going to be reflected in the status. So that's the reason I like ZenHub. It
provides an easy way to understand what is going on. I've got my Kanban board in
GitHub. And if anybody asked me, "How's the project going? Management wants to
know where are you?" They can open up the ZenHub Kanban board, they can see all
the issues that are still in sprint, haven't been worked on. All the issues that
are currently being worked on, and who's working on them, and all of the issues
that we already have done. So very, very important to get a quick status of
where we are in a project.  And, as I said, it maintains an up-to-date, one
version of the truth, developers work on stories and GitHub all day long. The
issues in GitHub, which are stories. Those issues are the things that they open
and close, and they don't have to go someplace else to update the status. The
status is kept right in their favorite tool, GitHub. So it allows developers to
go one place to get things done, and not have to update multiple tools. So what
is a Kanban board? We've been talking about Kanban boards here. Very simply put,
there's things that you need to do, things that you're doing, and things that
you've already gotten done. It doesn't have to be any more complicated than
that. People make it very, very complicated. But it's kind of you know, what I
got to get done, what am I working on now, and what have I already done. And you
move things across the Kanban board, in order to show the progress that you're
making, so it's a very visual way of seeing exactly where you are at any point
in time. Now, here's a real Kanban board. And as you could see, it's got the
product backlog. And it's got what's on deck and it's got what's doing and what
we have done. So it's kept it very simple, but this is a real Kanban board. It's
not a tool. It's not some electronic thing. It's a physical whiteboard with a
bunch of sticky notes. So in true Kanban fashion of having a billboard note, a
note that moves along the supply chain moves along the management, the
manufacturing chain, that's what they do. You take a sticky note, and you write
the story on it. And then you move the sticky note across the whiteboard across
those columns. I mean, that's as simple as a Kanban board needs to be. So let's
talk about the default pipelines or columns that are in ZenHub. It starts with
new issues. New issues is like your inbox. When anybody opens up an issue. It
defaults to going into the new issues column. And so I don't like to leave it
there too long. When I when I do my backlog refinement and I work on my Kanban
board, I usually do new issue triage first and say this is something that just
came in, where should it go? And I move it to another pipeline, or I reject it,
but I don't keep it in the new issue so that when another one comes in, I know,
oh, that must be really new because I just cleaned that out kind of like your
inbox for emails. Then there's the icebox. This is unique to ZenHub, but I kind
of like it. The icebox is cold storage. It is where you put things that are
going to be, you're going to work on long term. So if I'm not going to get to
something for a while, I'll throw it in the icebox. So I don't forget about it.
But then it is not in my other pipelines that I'm actively working on so that
they don't get too cluttered up. After the icebox is the product backlog. The
product backlog is everything you ever want to do forever in your product that
you haven't done yet. Right. It doesn't contain things you're doing.  It
contains all the things you haven't put in a sprint that you want to work out at
some time in the future. And again, in order to keep that product backlog not
too cluttered things that are long term future, I like to move into the icebox.
That brings us to the sprint backlog. The sprint backlog is what we're going to
do in the next two weeks. So I've taken things from the product backlog and move
them to the sprint backlog to make a sprint plan. Now the developers don't have
to worry about any of these other pipelines, they just concentrate on the sprint
backlog, because that is the work we're going to do in the next sprint. Then
once we start working on things we move them to in-progress. So I know that when
I see those cards, those stories in the in progress column, I know that somebody
is working on them as they assign them to themselves, their little avatar shows
up. So I can see exactly who is working on what and what is being worked on as
we speak. Once the work is complete, then a developer usually create a pull
request to go pull their work back into the base branch. And so those go into
review QA, you can also set up GitHub and ZenHub so that it automatically
creates pull requests in that review QA column. And so that so that developers
know, when they see something show up there, that they need to go look at it and
help another developer out and review their story and make sure that they get,
it meets the criteria needed to go merge it into the rest of the code. And then
finally, there's the done column. After we're all done, we've merged our code
back, then we move the story to the done column. So done means the developer is
done. It doesn't mean that it's been accepted by the product owner. That is
something that happens during the sprint review. But it does mean that the
developer is done with that story. They go back to the sprint backlog, pulling
the story into in-progress, assign it to themselves and keep working. So the
flow goes from left to right. New stories come in on the left and a done
increment winds up going out on the right. In this video, you learn that a
Kanban board is a way of tracking planned items needed to be done, items in
progress, and items completed. A Kanban board is made of multiple pipelines.
Work moves from left to right as it is completed.