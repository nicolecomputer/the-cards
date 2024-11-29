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

# The Cards

---
layout: TableCenter
---

# Dark Cards

Probably all on one table

---
layout: TableCenter
---

# Light Cards

Probably all on one table


---
layout: TableCenter
---

# Obstacles

Probably all on one table



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
  <LightCard title="Nature" imageUrl="/nature.svg" />
</template>

- Blah
- Bleeehhhhh
- Anothe blah

---
layout: CardAndText
---

<template v-slot:card>
  <LightCard title="Community" imageUrl="/community.svg" rotationAngle="3" />
</template>

# Community

---
layout: CardAndText
---

<template v-slot:card>
  <LightCard title="Vitality" imageUrl="/community.svg" rotationAngle="-4" />
</template>

# The body

---
layout: CardAndText
---

<template v-slot:card>
  <LightCard title="Art" imageUrl="/community.svg" rotationAngle="7" />
</template>

# Art

---
layout: CardAndText
---

<template v-slot:card>
  <LightCard title="Rest" imageUrl="/community.svg" />
</template>

# Rest

---
layout: TableCenter
---

# Momento Homo

---
layout: TableCenter
---

<h1 class="loved">You are loved</h1>

<Nametag />



