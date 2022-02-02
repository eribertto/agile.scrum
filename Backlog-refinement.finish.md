After watching this video, you'll be able to add details to make your story
sprint-ready, identify stories that are technical debt, and rank your product
backlog in preparation for sprint planning. So, the next thing I want to talk
about are the labels. Labels help us visualize the work. If we look at the
kanban board over here, you see all these nice pretty colors. Now, I don't get
too crazy with the colors. Too many colors, it becomes meaningless, but if I've
got a couple of colors that catch my eye, then I can see, is there too much of
that color on my board? And what does it mean to me? So, let's look at these
labels. The labels come standard in GitHub, and these are the standard GitHub
labels and colors. You can see I've got bugs, bugs are red. I like that. Red
means danger. You don't want a lot of bugs. Enhancements are the cyan color. Not
bad. Help wanted is in green. So, these are kind of good. I've got questions,
won't fix, things that are invalid, and they help me visualize things about each
one of the stories. But I like to add 1 label that, surprising to me is not
here, and that is technical debt down at the bottom, and I make that technical
debt, I make it yellow because yellow means caution. You don't want to have too
much technique debt. So, let's go back to my story and I look at it and say, you
know what? This is really adding value to the customer. This is the first thing
we're doing that's adding value, and I think it's an enhancement. So, I'm going
to assign the label of enhancement to this story, and then I'll save it. When I
save it, I go back to my product backlog and notice its appearance has changed
and it will change in ZenHub when you use the tool. You notice there's a little
circle that... There's an area at the bottom of it with a circle. That circle is
going to have the story points in it, so that'll have a number pretty soon. And
then I've got their little enhancement label and it's this, you know, light blue
or cyan colored enhancement label. So, now I could start seeing with colors how
we're doing on the kanban board. Let's go take the next one, the next highest
priority in the product backlog, and let's go groom that one. So, this one is as
a service provider. I need the service to persist so that I don't lose track of
the counter and so, what are some assumptions? Well, maybe we decide, you know
what, I think we're going to use a Redis database. It's this nice MEM cache
database. You know, we really don't need a relational database to keep track of
a counter. Developers might not know that. So, if you know it may be the
architect or the lead developer said, “Hey, you know, we ought to put in there,
so whoever picks this up knows, we're just going to use Redis and we're going to
store the counter as a name value pair in a MEM cache database.” So, anything
you know about it, there's always assumptions, document them in your stories and
then we have our acceptance criteria. Given I've incremented the counter two and
I restart the service, then the counter should still return to, right? So that
proves that we actually have persistence behind this. Now if I go think about
the label, I might say, you know what, that's an enhancement, right? This is,
this is something. It's better now because now you don't lose the counter. So,
I'm going to say that one is an enhancement. So, now when I go back to my kanban
board, you see that one has been modified and we'll go pick the next story
“deploy service to the cloud.” And when we open that, it's like, oh, all we have
is “deploy service to the cloud” because that one came from the new issues. So,
while we used the template when we created our initial stories, customers,
stakeholders. They're going to create more stories. They're going to wind up in
new issues. They're not going to have a lot of detail in them, so “deploy
service to the cloud.” So, let's go work on this one and refine it. So, as a
service provider I need the service to be deployed to the cloud so that it can
scale capacity with user demand, right, just so I know how important that is.
And maybe we have some assumptions, we're going to put it in the IBM Cloud and
maybe deploy it as a Cloud Foundry app. you know, whatever you want, you're
going to put it in Kubernetes and deploy it as a container. Give the developer
some hints on how you want to deploy this to the cloud. And then we've got our
acceptance criteria. Given I've deployed to the cloud and a customer goes to the
URL, our service will be available, right? This is all about availability, so
now what labels should we give to this one? I'm going to say this one is
technical debt because there's really no added value to the customer. Although
you can argue that higher availability is customer value, but the customer kind
of expects high availability, right? So, this is not an enhancement that the
customer might recognize, but if they would feel free to make an enhancement but
for the sake of argument, I'm just going to make it technical debt. So, that
begs the question, what is technical debt? Technical debt is anything you need
to do where the customer doesn't perceive that as value, right? It's not really
adding a feature to the product, but it's something you have to do. If you
didn't do it, maybe everything will fall apart and so you might say it's an
enhancement because the customer does get value out of things not blowing up,
but usually, it's anything you have to do that the customer has not perceived as
kind of a customer story where they're getting value out of it. Now, many people
understand that, you know, technical debt builds up over time, and they think
it's a bad thing, but sometimes it occurs naturally, right? Sometimes there are
vulnerabilities in the code that are external libraries that have to be patched
and that was not your fault. It was something totally out of your control, so it
does build up over time and it's important to pay that debt down. So, let's look
at some examples of what technical debt is. Maybe some code refactoring. So,
those are things where we took some shortcuts and now it's time to refactor the
code and the customer doesn't see a benefit from refactoring, but the
developers, because it's refactored, maybe they can add enhancements quicker.
So, you can always argue eventually they’ll benefit, but you know, if you
wouldn't put on your list of new features, “we refactor our code,” it's probably
technical debt. Setting up and maintaining environments. Customers don't care
about that. You need to test the environment. Any kind of environment, technical
debt. It has to be done, but you know the customer doesn't get a benefit.
Changing technology like databases. We decided to go from an SQL to an No SQL
customer doesn't see that it's all behind the scenes. It's kind of technical
debt, you know, not a bad thing. Maybe it's going to allow you to do things you
couldn't do before, but when you do those things you couldn't do before, those
are enhancements, but just swapping databases, technical debt. As I said, if
there are vulnerabilities in libraries, you've got to upgrade the libraries
you've got to retest the code, make sure nothing broke. Technical debt. So, it's
really, really important that you don't shy away from technical debt. Understand
what it is, give it a label. Make sure that you put a little bit of technical
debt in every one of your sprint plans so that you bring it down, but by having
this label you could see how many stories on the kanban board are yellow with
technical debt, how many are blue with new enhancements... So, now you can see
I've got this nice yellow label that shows me some of the stories in my backlog
are technical debt. We look at the last one as a System Administrator and the
ability to reset it a counter, so I could recount something. So, now let's add
some assumptions. Maybe the technical lead said, “Hey, you know, we ought to
tell the developer how to put this URL because it might be a little tricky, we
want it to be a post to counters with a counter name and then a slash reset and
that will reset the counter because there's multiple ways you could probably
reset the counter, right?” You could update it with a zero. You could do it a
lot of ways, but maybe that one because you want to protect it and only have
admins do it, you make it a separate endpoint that only admins get access to.
And then your acceptance criteria. Given the counter has advanced to five, when
I call reset on the service and I request the current counter, then I should see
zero return from the service. So, now we have a nice understanding of how should
this thing behave. We've agreed on the definition of done so that there's no
questions about it when we get to the sprint review and they demonstrate this,
and that's exactly what it does. No one can argue that that is what it was
supposed to do. So, now we'll assign a label, and I would say that's an
enhancement. Being able to reset counters is a new feature, so I'm going to go
with enhancement on that one. So, now back to our kanban board. We've got our
product backlog all refined and we've got labels so that we quickly see, hey,
we've got three stories that are enhancements, one story that's technical debt.
I've got this nice visual indicator and it's okay the ones in the icebox,
they're going to be later. We will refine those later, but the ones at the top
of the product backlog have these nice labels and then maybe we can put some
story points to them when we do the sprint planning for this go around. So,
let's look at some backlog refinement tips. You should be refining the backlog
every sprint. My sprints usually go from Monday to the following Friday and
about the Wednesday before the end of the sprint, I like to have a backlog
refinement meeting. So, every other week, I'm refining my backlog, getting it
ready for the sprint plan that I usually have on Monday mornings at the
beginning of the sprint, right? Because you do your sprint retrospective and
your sprint review on a Friday, everyone is exhausted, they go home and then I
do the Sprint planning first thing Monday morning, so I usually do this on a
Wednesday. Now, some people do it every week, and if you have a lot of
requirements coming in, you might want to do it every week. But it's important
that, at least once a sprint, you're refining this backlog to keep it healthy.
You want to have at least, I'd like to have two sprints worth of stories refined
in the backlog, right,? So, if by some miracle, right, they get done with all
the stories in a sprint, they need to pull more things from the backlog, they
could just pull them from the product backlog. But mostly I want to make sure
that I don't get cut short if something happens. You know, I've got enough
stories that are refined that maybe I can skip a refinement meeting one week
because of some delays or whatever. So, I'd like to have at least two sprints
worth kind of refined in that product backlog. And then the more time you spend
refining these stories, the less time you're going to spend doing sprint
planning. So, if you can add story points, we'll do it in the sprint plan, but
if you can't add some story points during the planning, the backlog refinement
meeting, then that's fine because it gives an idea of how big these stories are.
But the more you do, the more detail you add, you don't want to be typing up
stories during the sprint planning meeting. It'll make that planning meeting
take forever. So, trust me on this one. Get all that done during the backlog
refinement meeting. In this video, you learn that backlog refinement is used to
order the product backlog and make stories sprint-ready. Technical debt is any
story that does not add perceived value to the stakeholder, and the goal is to
get the backlog ready for the Sprint planning meeting.