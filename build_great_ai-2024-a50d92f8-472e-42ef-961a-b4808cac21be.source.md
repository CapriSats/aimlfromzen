---
source_url: https://www.youtube.com/watch?v=U5J5RUOuMkI
source_file: build_great_ai-2024-a50d92f8-472e-42ef-961a-b4808cac21be.md
extractor: youtube
fetched_at: 2026-04-26T18:11:58.586816+00:00
char_count: 15740
title: "YouTube video U5J5RUOuMkI"
---

hey everyone it's Hugo B Anderson here
host of the data ML and AI podcast
Vanishing gradients I recorded an
episode recently with haml Hussein and
Dan Becka who I'm here with again hey
Dan hey thanks for having me absolutely
and so we record an episode uh about
many things including what you and haml
learned when teaching llms and fine
tuning to thousands of of students
there's a few things we chatted about
which made us want to do this demo which
I'd love to jump into in a second but
first for context maybe you could just
tell us a bit about yourself and what
you're up to at the moment yeah so I've
been a hobest data scientist for
probably 15 or 20 years and then worked
professionally in AI for started in in
about 2011 I finished second in a kago
competition with a $500,000 prize for
first place but no prize for second
place but ever since then I've been
working in AI that includes some time at
Google found out a startup ran a team
for for data robot building tools for
data scientists and then for the last
year or two have been doing independent
Consulting using llms and generative Ai
and then obviously teaching you and I
taught a deep learning
course probably in the mid 2010s for
data camp and then recently did this
course from Maven about fine tuning and
at the moment I'm teaching a course on
rag with Jason Lou the creator of
instructor awesome and a lot of other
educational
stuff as well I mean a lot of teaching
data science and analytics and machine
learning a data robot and building out
their platform for doing so and then
kaggle learn which you worked on at at
Google which you spearheaded which was
such a great
initiative yeah that's right so always
been excited to share AI with others so
what prompted us to decide to do a demo
along these lines what did you learn in
this course okay
so I think I've learned a couple things
people are very very excited about
Ai and you hear people talk about you
hear for instance Sam Alman talks about
Amor's law for everything that is every
aspect of our life is suddenly gonna
have this new trajectory of improving in
a exponential rate that we've never seen
before for anything except for maybe
microprocessors and when I taught this
course we had 2,000 people and everyone
was interested in llms in the abstract
and how larger model can I fit on a GPU
and how does that change with
quantization and very technical aspects
but very few people had ideas for
products they could build or use cases
and I think as much as we're all excited
about generative AI if we can't figure
out how to build useful products then
we're not going to get a moros off for
everything we're just going to get a lot
of optimization of a narrow set of use
cases so that made me very excited to
think more about useful products that
could be built then coming back to this
idea of a Mor is law for everything I
know that in my life in the lives of
people that I interact with a lot of the
things we want are physical and yet most
of the use cases that I've seen for llms
are optimizing the same things online
that we've been optimizing with data
science for a long time and not crossing
over from bits to atom so I've been very
excited about trying to do things that
help us help people create things real
physical tangible goods that will show
up in their lives and that they can
physically apply to solve problems so
that's the piece of software that is in
a very very early stage this is pre
Alpha this is sort of a side hobby
project I've just started on but is
something every time I use it I have fun
with it and I think it can
unleash the creativity and productivity
for people who want to build business
things well let's jump in and I love the
framing of from bits to Adams it reminds
me of don't know if you watch a lot of
The Simpsons but radioactive man who's
radio wolf Castle whose tagline slogan
was up and atam so let's let's do it
okay let's do it
here is the Prototype app and I'm a big
fan of yours let's make a household item
with your name engraved in it so let's
start with a cup with the name Hugo
engraved in in
it and I've always wanted one of
these we're going
to create a 3D model of an object
actually we're going to have a bunch of
different llms using different CAD
languages we're going to as result show
a bunch of different models of physical
objects spatial reasoning is still quite
challenging for most llms and as a
result many of these 3D models are not
going to be very good that's totally
okay we're going to build a bunch of
them and as a result if many of them are
not good we'll just ignore those and
then we are going to iterate within the
software the same way that if you using
CAD software you don't design everything
exactly right the first time you touch
your mouse instead you try things and
you go back and you move things around
so that's just part of the design
process and we will have the same design
process here so here you can see we've
got one the name Hugo is sort of
floating about so that's we want wanted
to try to try to 3D print that we've got
a number of different designs most of
them are not really exactly what I want
to 3D print but let me I'll just pick
one we wouldn't expect them to be with
the first prompt as well right that's
right let me I'm gonna take this one and
I'm gonna pick it and now we're g to
just iterate
so I'm G to say the name Hugo seems to
be loading on the inside of the cup have
it be
letters raised from the bottom inside of
the
cup and make the letters be pretty
tall and while this is running can you
tell us anything about the models you're
using or I don't want you to give away
any Trade Secrets or secret source as
well you know it's too early for me to
think of anything as trade secrets so
and let me also emphasize I would really
like to have people who have 3D printers
and don't know what to do with them
which I think describes 90% of people
who have 3D printers anyone who wants to
try this I'm not trying to monetize or
anything get in touch with me Dan at
buildg
gr. and I'd love to have people
experiment with this going back to your
question the models are just all the
mainstream models so that would be for
instance llama it's August 2024 so that
would be llama 3.1 GPT 40 Sonet 3.5 so
we're just trying all of them and then
for each of them we're trying them you
know Chain of Thought versus not Chain
of Thought they're different CAD
languages so different we're
experimenting with just uh a lot of
different versions but the models are
mainstream languages available through
apis so here we have this is already
looking better so you're using the base
models not you're not fine-tuning on CAD
prompts and and this type of stuff
that's right I think there's a future
where we do fine tuning and certainly a
future where we embed more examples we
have some examples in the prompt but we
have more examples in the prompt and you
can imagine doing rag to figure out what
examples you embed in the prompt so
there are lots of things that I intend
to do this is just a hobby side side
project that I started maybe a month or
maybe just even less than that ago and
so we're in the very early stages and
there's no fine-tuned model yet and just
one more question the output of the
model isn't this 3D image right it's
code that then use to render yeah so the
standard format that if you have a 3D
printer and you want to print something
the way that you import that into the
slicing software that's specific to your
printer is in a file it's format called
STL and if I click get STL then I will
download that file and now I can print
that and an hour from now if I want it
or I this a pretty small thing to print
probably 30 minutes from now I could
have that cup I could be holding it in
my hand I could be drinking from a Hugo
themed cup incredible and could you just
show us the code under get code by any
chance yeah so this is a relatively
simple object so as a result this code
is in a language called open escad and
we try uh a few different languages but
this I can tell by looking at it is open
escad code this is the open escad code
that creates the STL file or that object
which is the one that we would 3D print
and if we want we can make this actually
it's a quite small cup this is if I
printed it right now it'd be 8 by 8 by
12 cenm so I could make the twice as
large I could make the letters come up
three times as high so those are all
things I could do simply by asking
amazing so you what you want to see
another object love to yeah let's try I
have a a daughter who really likes dogs
so let's start with a dog and while
that's generating I saw something that
said upload image so I mean what my
intuition says is that you may be able
to use the multimodal aspects of such
models as well yeah a neighbor of mine
is a a I think that he would not be
offended if I said a small time inventor
one of the things that he invented is at
some campgrounds they have two different
types of plugs and they can't be used
simultaneously so he's got something
that cover the plugs with and then the
camp G can do that so that you can use
one of the plugs the other one is
blocked there's something that slides to
one and he said that if he wanted to use
this the thing he ideally would do is
sketch it on paper and then show us show
the image of his little sketch to the
model that's using the multimodal aspect
like you said and so this is all just a
way for however you want to input it
whether it is with text or whether it is
with images that you sketch out or I
could even you know show it a little
stuff dog and use that instead of
describing the dog as a way to get my
ideas into the
machine and coming back you can see like
some of these are actually quite bad
like these are detached that comes back
to lm's as of August 2024 being really
bad at just spatial awareness and then
also like if a human were to write this
code if they didn't get to see their
output they just had to do it straight
out we would do no I would know do no
better than this terrible option here
the first time around you actually kind
of see these are the legs but I would do
quite poorly you would need to iterate
fortunately we be faster are getting
many iterations simultaneously so you
can see here's one this is not so bad no
it's like a a chubby
Chihuahua yeah I'm not a Chihuahua fan
so I'm gonna say make the legs longer
you're gonna say make it a great or
something L boxy oh should we make it
make it
a Great
Dane okay let's see what happens
here very cool very interested in how
llama 3.1 as it's August 2024 Compares
for your needs to pinging vendor
IPR you know the funny thing is that
llama 3.1 comes in various
sizes the largest that I use I think
it's whatever 72 or 70 or 80 billion
parameters that is meant to be roughly
the same quality as GPT 40 mini both of
those are really not very good so both
of those are worse than GPT 40 or Sona
3.5 and I think that's not a surprise I
have a hunch that if I were to run the
400 billion parameter model that's the
one that's supposed to be competitive
with GPT 40 but I have not done done
that yet the for serving llama 3.1 I'm
using grock and I think that using grock
it happens to be free at the moment
hopefully they'll let me get a paid
account so I can use it more
aggressively um using Gro is a is a
fantastic experience and when you watch
this app have the models pop up you
always have one or two that pop up way
before the others that's because we're
using Rock that's with llama 3.1 on the
70 billion parameter model and it just
is much faster than the other models so
it pops in faster so the real advantage
of llama 3.1 if you can't use the really
big model is that because you can serve
it on grock you can serve it very
quickly
great so let's look at a couple of these
dogs
these we're GNA have to talk to the
model about our great dane these are
really not very great Dan like
but we can always iterate and for one or
two iteration I mean I iterate a lot
more to get way way less things what I
think they will be in
text yeah so I'm GNA just and at least
we're not hearing now oh I'm so sorry I
didn't do this you know of course I will
do this for you in
future yeah that's right and the you if
I if you were doing this with CAD
software no offense but I'm guessing you
haven't used CAD software so how long
would this take you I don't know a month
I've used some CAD software good
amount this would probably take me a few
hours even to get to the stage that this
is at right now and instead while we're
talking it's taken a couple minutes so
it's about a 60x speed up I think even
for someone who's good with CAD software
this is
still faster than it would they would be
at this point so in all honesty Dan
something I'm really I've got a bunch of
friends who are architects who I've
talked about you know the implications
of textto Tex models for the their line
of work but I I can't wait to show them
this video and just get their thoughts
on it and and riff with them on it I
think the upper bound and
complexity for what we can do with this
software is still lower than what can be
done with C software so I think for
someone who's making a building which is
obviously much more complex than a
plastic dog toy I think that they'll say
may I'll be interested to hear their
feedback I think that it's actually not
for them but for the home inventor who's
going to make something small I think it
actually is a a nice way to make
prototypes them out see yeah I mean even
thinking I don't know anything about
what I'm talking about but thinking
about Structural Engineering or
buildings or that you could imagine that
just generating templates could shave
10% save someone 10% of their
time yeah so one of the places that I
want to take this in the future is for
physical
objects if you want to design something
that is actually functional there's a
lot of calculations that you would
typically do one of the techniques is
finite element analysis so one of the
directions that I want to take this is
one where the LM can do tool calling and
as a result if I say I want a catapult
it doesn't just make me a catapult but I
can say I want a catapult and if I print
it with this type of plastic I want it
to to shoot a checker or meters and it
actually figures out what are the
parameters how long does the arm need to
be and so on in order to meet that
functional requirement and that doesn't
exist yet but I do that's one of the
directions that I'd really like to
explore incredible That's so exciting so
is there anything else you want to show
us here now I don't think so with my
call to action I've got the website
designbench doai so someone can either
email me or just log in there create
their own account you can do it take 10
seconds so I'd really encourage anyone
who sees this who's curious especially
if you have a 3D printer and haven't
used in a long time try this out and I'd
love to see if you find it interesting
and how I can improve it so that it's
useful to people fantastic and you said
Dan at build buildg
grate. yep or if you just want to try it
out without emailing me design bench. is
the one word designbench is the website
where this is being hosted awesome and
for those of you who bre this video
through the podcast episode thank you so
much for joining for those of you who
didn't I'm going to put a link to the
podcast episode below as well so please
check it out thanks once again Dan for
your your time and wisdom also everyone
just a super quick update it's been a
couple of days since I recorded with Dan
uh and as you can see here he's sent
through um some photos of
uh the Hugo inspired cup that he 3D
printed so thanks once again Dan um and
excited for to drink from this one day
