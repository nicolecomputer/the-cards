---
theme: seriph
title: The cards
info: |
  Let's talk about your cards

# apply unocss classes to the current slide
class: text-center
drawings:
  persist: false
transition: fade
overviewSnapshots: true

colorSchema: dark
layout: TableCenter
clicks: 1
---

<Cards />

<!-- I want to tell you a story (flip, count to two) -->

---
layout: CurtainCenter
clicks: 1
transition: none
---

<TheHero />

<!-- This is the story of you (flip card). The hero. It is the story of me as well and what it means to be alive and doing your best -->


---
layout: TableCenter
---

<FlowingCards />

<!-- In life we are dealt cards. We do not ask for these cards. Some of them are dealt at birth some, later in life. -->
---
layout: TableCenter
---

<ThreeUp>
  <CardFront title="Chronic Depression" kind="dark" imageUrl="/dark-perfectionism.svg" :animated="false" />
  <v-click>
    <CardFront title="Perfectionism" kind="dark" imageUrl="/dark-depression.svg" :animated="false" />
  </v-click>
  <v-click>
    <CardFront title="Nuerodiversity" kind="dark" imageUrl="/dark-nuerodiversity.svg" :animated="false" />
  </v-click>
</ThreeUp>

<!--Some are dark cards. Like chronic depression (click), perfectionism (click), and nuerodiversity. These cards will be with us our whole life and you must make them your friends. Take them to tea. Get to know them.-->

---
layout: TableCenter
---

<ThreeUp>
  <CardFront title="Time of peace" kind="light" imageUrl="/light-peace.svg" :animated="false" />
  <v-click>
    <CardFront title="Strong Family" kind="light" imageUrl="/light-family.svg" :animated="false" />
  </v-click>
  <v-click>
    <CardFront title="Health" kind="light" imageUrl="/light-health.svg" :animated="false" />
  </v-click>
</ThreeUp>

<!-- Some cards are light cards. You may have been born into a time of peace and prosperity. (click) You may have a strong family. (click) You may have your health. These are blessings. These too you did not earn. They are the grace of the universe. Treasure them. -->


---
layout: TableCenter
---

<ThreeUp>
  <CardFront title="Relationship Ending" kind="obstacle" imageUrl="/obstacle-heartbreak.svg" :animated="false" />
  <v-click>
    <CardFront title="Career Changes" kind="obstacle" imageUrl="/obstacle-job-loss.svg" :animated="false" />
  </v-click>
  <v-click>
    <CardFront title="Identity Crisis" kind="obstacle" imageUrl="/obstacle-identity.svg" :animated="false" />
  </v-click>
</ThreeUp>

<!-- As you live through life you will be dealt obstacles. They will appear when it's most inconvient. You will need to do your best. Relationships will end.  (click) Careers will change, sometimes suddenly. (click) And you will have moments of identity crisis. You will overcome these obstacles. -->



---
layout: TableCenter
---

<TheComputer />

<!-- By being here, and listening, You have been dealt an obstacle card of the computer. We all share this card. This machine is a box of wonder but it will also steal your heart and make your mind hard. Do not let it do this. Fight for your hummanity, your body, your community. You need to remember that you are a person first and a computer practioner second.-->

---
layout: TableCenter
---

<p>Nothing you learn can <span class="cancel-wish">nullify</span> your dark cards.</p>

<p>And you <span class="cancel-wish">cannot stop</span> obstacles.</p>

<v-click>
<p class="im-sorry">I'm so sorry. I wish it were different.</p>
</v-click>

<!-- These are your cards. You must bear them, love them work with them. You cannot wish away your dark cards. You cannot stop obstacles. You will age. The people you love will change. (click) I wish it were different. I'm so sorry.-->

---
layout: TableCenter
---

<FiveCards />

<!---
You will have aid. You may not always know the light cards that are available to you. But I want to tell you about some that dear to me.
-->


---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Nature" imageUrl="/nature.svg" />
</template>

- Read a book somewhere peaceful
- Camp outside
- Walk somewhere that makes you feel alive

<!-- Nature reminds us that we are part of something bigger. It reminds us that there are season to
being alive. It teaches us to slow and to feel. Being in Nature doesn't have to be complicated. Take a book and read somewhere you find
peaceful. Listen to the way the world sounds. Spend a night camping outside with the magic of a fire. Car camping counts. Walk in
the solemnity of a forest or deep in a city park. What birds are those? What's the name of that plant?

Nature helps break the spell of the computer. It is not rigid, it flows. Answers can be right and wrong at the same time. It's answer is
always "it depends".

You can not have an inauthentic experience in nature. Relax into what is there in that moment. You'll feel better.
-->

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Community" imageUrl="/community.svg" rotationAngle="3" />
</template>

# Community

- Start with hello
- Really listen to the stories
- Find community in play, creativity, shared experiences, shared curiosities

<!--Community will save your life. Again and again. Your community will remind you that you are not alone, that your feelings
are wonderous and yours and also familiar. Whoever you are, not matter how lonely, community beckons to you. Start with hello.
Find the people who make you feel alive and grounded in the fullness of yourself. Ask about their adventures, really listen.
Give of yourself with no expectation other than knowing and being known. You may have a dark card of social anxiety, I know
I do. Try to be patient, feel your feet on the ground, the air in your lungs.

Community exists in so many forms from people you play video games with, solve crosswords with, mail postcards to, program
with and so much.

Even computers long for community. They connect over huge distances. But the protocols are rigid. Remember to give and flex in
your community.
-->

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Vitality" imageUrl="/vitality.svg" rotationAngle="-4" />
</template>

- Your body craves plays
- Running, swimming, frisbee, dance!
- A happier longer life

<!-- Your body craves play. Somewhere inside of you you probably already know this. It wants to run
and move and jump. It wants to twirl a pen between fingers just because it's cool. Find these feeling
and nurture them. Being in your body can be a group thing in team sports or even just going for a walk
together. For many of us, though, we might be drawn to solitary activities.

For me running is a practice that makes me feel more alive. At first my mind will be loud with stories
but as I get into a run things quiet and I am feeling my feet hit the ground.

If movement is hard for you here are two perspectives that might help: think of it like medicine at first.
You take your dose, your life improves. Or maybe look for the "hill climbing". Can you run 1 kilometer?
What about 2? And see where it goes.

Being in your body is almost the computer's opposite. You think and feel with the whole of you. Especially
after a long day of programming there's probably a part of you craving this.
-->

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Art" imageUrl="/art.svg" rotationAngle="7" />
</template>

- Start with paper and an analogue
- Art is writing, scribbling, folding the paper
- Not for impressing others

<!--
Art gives your mind a break form rigid thinking.

The world is so big and so full and it can, at times seem full of dark cards. Making is an act of rebellion.
Making says I exist, I matter. I am full of feeling and wonder. Art may feel awkward at first. You might not be
good at it or it might be a long forogtten form of play. Your hands, your mind, and spirit crave this kind of play.
Remember when you were excited to draw the forms or home, family, cards, trees. That spark is still alive in you.

The art you make is for you. Start with a sheet of paper and an analog tool. Your hand will know what to do. Do you
want to write stories? Draw scribbles? Faces? Words? Plans? This is a part of you talking to yourself. Listen.

You are not making art to impress others. This is a catharsis. This is a messy part of you that wants to be heard.
-->

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Rest" imageUrl="/rest.svg" />
</template>

- More than just a good night's sleep
- Go for a walk with no technology
- Consider a duvet day

<!-- This is perhaps the hardest of the light cards that I know. You must rest. Rest is not just sleeping at night,
although your needs and craves that. It also means fallow periods. It means time where nothing is expected of you
either by yourself or by others. You are tending to the fullness of yourself and investing in the future. I promise
you are not lazy for needing rest, recovery and space.

One form of rest that I find helpful is the "duvet day". On a duvet day I make an effort to stay in pajamas, I hang
around the couch or the bed. I read. I listen to music. I don't check my fitness rings or worry about what I have
created or done that day. I allow myself rest. You might find your version of duvet day be it sabbath, no-technology
at the dinner table, or trips to places where there's no cell reception.

The computer and technology never ceases and always wants. It sends push notifications, runs cron jobs, and grows
bigger every moment. You are not a computer.
 -->

---
layout: TableCenter
---

<h1 class="warning">
Momento Homo
</h1>

<!-- Remember that you are a person. You are filled with wonder and universes and magic. And you are also full of feeling. You will need rest. You will have sick days. You will have wonderous days. Remember that you are a person and you are allowed all of it.-->

---
layout: TableCenter
---

<h1 class="loved">You are loved.</h1>

<Nametag />

<!-- You are loved. May your adventure be wonderous. Be good to each other.-->


