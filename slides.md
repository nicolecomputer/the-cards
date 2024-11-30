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

<!-- By being here, and listening, hero. You have been dealt an obstacle card of the computer. We all share this card. This machine is a box of wonder but it will also steal your heart and make your mind hard. Do not let it do this. Fight for your hummanity, your body, your community. You need to remember that you are a person first and a computer practioner second.-->

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
-->

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Community" imageUrl="/community.svg" rotationAngle="3" />
</template>

# Community

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Vitality" imageUrl="/vitality.svg" rotationAngle="-4" />
</template>

# The body

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Art" imageUrl="/art.svg" rotationAngle="7" />
</template>

# Art

---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Rest" imageUrl="/rest.svg" />
</template>

# Rest

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

<!-- You are loved, my hero. May your adventure be wonderous. Be good to each other.-->


