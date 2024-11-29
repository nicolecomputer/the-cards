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
---

<Cards />

<!-- I want to tell you a story -->

---
layout: CurtainCenter
---

<Card :animated="true" />

<!-- This is the story of you (flip card) and of me and of what it means to be alive and doing your best -->


---
layout: TableCenter
---

<FlowingCards />

<!-- You get delt cards -->
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

---
layout: TableCenter
---

<ThreeUp>
  <CardFront title="Time of peace" kind="light" imageUrl="/light-blank.svg" :animated="false" />
  <v-click>
    <CardFront title="Strong Family" kind="light" imageUrl="/light-blank.svg" :animated="false" />
  </v-click>
  <v-click>
    <CardFront title="Health" kind="light" imageUrl="/light-blank.svg" :animated="false" />
  </v-click>
</ThreeUp>


---
layout: TableCenter
---

<ThreeUp>
  <CardFront title="Relationship Ending" kind="obstacle" imageUrl="/obstacle-blank.svg" :animated="false" />
  <v-click>
    <CardFront title="Career Changes" kind="obstacle" imageUrl="/obstacle-blank.svg" :animated="false" />
  </v-click>
  <v-click>
    <CardFront title="Identity Crisis" kind="obstacle" imageUrl="/obstacle-blank.svg" :animated="false" />
  </v-click>
</ThreeUp>



---
layout: TableCenter
---

<TheComputer />

---
layout: TableCenter
---

<p>Nothing you learn can <span class="cancel-wish">nullify</span> your dark cards.</p>

<p>And you <span class="cancel-wish">cannot stop</span> obstacles.</p>

<v-click>
<p class="im-sorry">I'm so sorry. I wish it were different.</p>
</v-click>

---
layout: TableCenter
---

<FiveCards />

<!---
With that said, I want to tell you about some of the light cards that I've learned, that help me.
-->


---
layout: CardAndText
---

<template v-slot:card>
  <CardFront title="Nature" imageUrl="/nature.svg" />
</template>

- Blah
- Bleeehhhhh
- Anothe blah

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

---
layout: TableCenter
---

<h1 class="loved">You are loved.</h1>

<Nametag />



