[MUSIC] After watching this video, you'll be able to define a product backlog,
describe how to assemble a product backlog, and convert requirements into
stories. So if we look back at the steps in the scrum process, in this module
we're just going to concern ourselves with the product backlog. How do we build
a product backlog? So what is a product backlog? A product backlog is all the
unimplemented stories, right? Stories that are not in a sprint, they're not
being worked on, they're waiting to be worked on. Usually we back, we rank this
in ranked order. Now, if they've got a long product backlog, the ones at the top
will be ranked a little more accurate than the ones down at the bottom and
that's okay. You only have to rank maybe the next sprint or two and then the
rest of them could be relatively unranked but the top of the backlog should be
ranked in order of business important. What's the next most important thing that
we need to get into a sprint? And then the stories at the top should have more
detail than the stories at the bottom, right? So as we work on this backlog and
we work on the stories, we want to get the ones at the top sprint ready, having
all the details they need and the ones at the bottom again, they're a little bit
fuzzier. We're going to work on them later, we'll add more details later. So,
we're going to go through an example and in this example we're going to give you
some sample requirements for the service that we're building.  So, what are we
building? We're going to build a hit counter, we're going to be a service that
counts things, so I could give the counter a name and then every time I
increment it 1, 2, 3, 4, and then I say, "How many of those do I have?" And it
gives me back the number 4, so it's just a little counting service that we use
to count things, hits to a page, count whatever you want. So it's a counting
service. Now, we want it to allow multiple counters eventually, so having
multiple counters that we can count multiple things is one of the requirements
that we have. Also the counters need to persist across restarts. So this just
can't be an in memory counter. It's going to need some kind of persistence, some
kind of database so that when the system restarts and comes back up it remembers
all the counters. And then we have a requirement that says, "You know, I
probably need to be able to reset a counter once in a while back to zero." So I
could start counting those things again and so resetting a counter is another
requirement that the customer has given us. So if we look at the kanban board in
ZenHub, you'll see these columns, they're called pipelines for new issues,
icebox, product backlog, sprint backlog, in progress, Q&A, review Q&A and done.
And so for this exercise we don't have to worry about anything but new issues.
Let's talk about creating new stories.  We've got new issues and it's empty and
so we're going to start creating the first story: Needed service for counting
things. So let's go back to our story template, remember as some role, I need
some function, so that I gained some benefit. Let's apply this to that first
story, need a service for counting things, well, maybe this is for the user.
Right as a user, I need a service that has a counter so that I can keep track of
how many times something has been done. So now we know who it's for, what is it,
and what is the value that they get after it and at this stage that's about all
I know about the story. And so I will put this story into the new issues, I'll
create a new issue for this story and so now it turns into a regular story.
Let's look at the next requirement: Must allow multiple counters. Again, we go
and look at "who is this for?" Probably still for the user. As a user, I need to
have multiple counters so that I can keep track of several counts at once.
Again, we know who it for, we know what they need, we know how valuable it is to
them so as we rank the backlog, we could say, "How valuable is that they can
keep track of several at once? Maybe in the beginning not, maybe let's just get
one working," right? So this is all the information you need to know in order to
rank this backlog later on. So that becomes a story in new issues. Let's look at
the next requirement, persist counters across restarts, so who is this for?
Well, maybe this one's for the service provider, right? Maybe the service
provider would be embarrassed if the service gets rebooted and they lose all the
counters. So maybe this one's for the service provider, I need a service to
persist the last known count so that users don't lose track of their counts
after the service is restarted and we can evaluate how important that is. That's
our third story and now let's look at the 4th requirement: Counters can be
reset. So we go through it again, this one might be for a system administrator.
Maybe we say, "Hey, only the sys admin can reset a counter." Maybe we don't let
users reset the counters. So, I need the ability to reset the counter so that I
can redo counting from the start. The important part here is that you're saying
who it's for. Specifying the role makes everyone clear who's going to benefit
from this. "I need," says what is it they really need and the, "so that" says,
"What is the business value that they're going to get out of it?" So now I've
got my fourth story in the backlog. Now let's move on to prioritizing the
backlog. Now that I've got them in new issues. I want to decide should I put
them in the icebox or should I put them in the product backlog? What do I do
with these? Remember I said I like to use new issues as my inbox, so now that we
got these four things in the inbox, let me go do something with them. Let me
prioritize that backlog. So I'll take the first one and say, "You know what?
That's kind of fundamental." Right? We need to get the service running, so that
was going to go right to the top of the product backlog. Then I look at the next
one and I read it, right, I need to have multiple counters. And I might say,
"You know what? Multiple counters, we'll handle that later. That's something
we're going to do in the future, I'm not going to bite it off right now,." Then
I look at I need the service to persist restarts. I say, "It's probably
something right after I get it working. I probably want to put a database behind
it." So when I do my minimum viable product, it might not have any persistence
behind it. And then next it will have persistence. And then I look at the last
one in the new issues as an administrator and say, "Yeah I might want to be able
to reset the counter right after I persist it in the database. So that I could
start counting all over again. And so what I've done is I've taken these new
requirements that came in from the customer which were just one liners and I
wrote them in the story syntax. I use the story template to say, "As a user I
need, right, as some role 'I need' so that I get some value and then I move them
into the backlog in some kind of priority order that I think I might want to
execute them. In this video you learned that a product backlog is a ranked list
of all unimplemented stories. Stories high ranked in the backlog should have
more detail than those that are lower, and creating stories using the "As a,  I
need, So that" template to ensure everyone understands who it benefits and the
business value it provides.