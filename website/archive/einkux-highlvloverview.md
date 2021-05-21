# Eink UX - High Level Overview

[![hackmd-github-sync-badge](https://hackmd.io/Wf0a9-dSQxiSkA9DVsfgIw/badge)](https://hackmd.io/Wf0a9-dSQxiSkA9DVsfgIw)


This is a document to gather a high-level overview of what knowledge we should gather in regards to the UX of e-ink. Please contribute and add any questions you think relevant.

###### tags: `psych-ux` `ux` `high-level overview`  

<br/>
<br/>

## Open Questions - UX of e-ink

This section is for gathering questions that need to be answered. For any questions that are not listed, add another. Answers to these questions are intended to be listed in a seperate space.

<br />

### What effects does e-ink have on the user vs. traditional display tech?
* See psych-ux working group: https://pad.riseup.net/p/ZMmKmTWJ6IgjvPOz_8_q
* Eye strain? Readability? Connection to headache, etc? Ability to use for longer periods of time?
    * Our hypothesis: e-ink is better for eye-strain

* What use-cases is this applicable for? Which use-cases overlap with the use of the technology (e.g. not for watching video)
    * People with medical problems re: eye-strain headaches. Otherwise, it's not "applicable", it's just nicer. I think the core implication here is that we're ultimately pushing a premium product, as there's usually no app that an e-ink screen can run that e.g. an LCD can't do.
    * Battery life: can be mitigated by "optimising software" or by attaching a charger and/or getting a bigger battery. Or perhaps more practically, recharging the device more often. Outside of camping trips, I don't think this is realistically a problem; just a minor annoyance.
    * "Tech addiction"? (Check for research on color vs. b/w display usage)
        * Some Android versions have support for this already IIRC, it's just not enforced like B&W is on a B&W e-reader.
        * ^though depends on whether there is a difference between LCD in black + white vs eink in black + white
        * This needs more research, as there may also be a difference between vibrant color and muted color in terms of attractiveness, etc. My hypothesis would be that the impact is a combination of animation & movement, bright colors, and overall visual stimuli, which would be muted even on a color e-ink screen

    * Use at night & impact on sleep patterns?


<br />

### What are the top usability issues/benefits regarding e-ink
* What are the top UX issues reported for e-ink devices? Are these tied to the tech or the implementation?
    * e.g. low refresh rate & ghosting

* What are the top UX benefits reported for e-ink devices? Are these tied to the tech or the implementation?
    * e.g. Long battery life, low-glare screen
    * This sounds suspiciously similar to the "what effects does e-ink have on the user vs traditional display tech?" question.

* What design principles are particularly relevant when designing for e-ink? (Q: how specific should we be here?)
    * Visual: e.g. increased contrast, no use of shadow, minimalist design language
    * Interactive: e.g. minimize use of scrolling, prefer more on one screen(?) to minimize screen refresh
        * Minimise any sort of movement whatsoever. If you need to put something on the screen, keep it still. If you need to move something, teleport it directly to it's destination without any tweening.
        * When possible, paginate instead of scrolling (per above principle of teleportation)
        * See my stuff about text editors. I more-or-less used that to workshop (theoretical workshop? I didn't test any of it.) what would work for e-ink in general.
* What observed patterns and standards from traditional non-e-ink devices do not work well for e-ink? 
    * e.g. scrolling, touch-screen responsiveness (real vs. perceived), use of touch-screen keyboard, mouse movement

* What use-cases are most applicable to be combined with e-ink tech? Which not?
    * e.g. Not watching video
    * e.g. Reading a book, programming terminal, sales/trading desk in a bank(?),working with text

* What "dark" pattern design elements that promote over-/unhealthy-use of technology do not apply to e-ink devices? Which still do?

* What design principles are particularly relevant to the use cases(?)
    * E.g. minimising notifications/distracting stimuli if device is for productive work

<br />

## Hypotheses - UX of eink
These are essentially rewrites of the above questions, but imply our assumptions that we need to either prove or disprove. These should be listed in the form of a specific hypothesis that can be proven or disproven, but indicate our belief(s)

* e-ink screens are better for eye-strain and eye-health than LCD/traditional screens
* e-ink screens cannot fully replace LCD screens for all computer/phone tasks
* e-ink screens require different interaction paradigms/design principles, particularly for specific use-cases
* e-ink screens are particularly suited to certain task types 
    * (List of task types)
        * ...

* e-ink screens are particularly unsuited to certain task types
    * (List of task types)
        * ...
* e-ink screens promote more rationed usage of the applied technology as they inherently allow for less "addictive" design practices
    * (A note to this one -- this only applies to certain things: color, animation, video, etc, as being simpler and thus less visually appealing in certain ways. Addictive design practices can still be applicable (feedback loops, extrinsic motivation, behavioural economics)
    * as a strategy, we ought to design around use-cases that emphasize the strengths of the tech and not focus on use-cases where we need to improve the weaknesses - for instance, improving video playback (a weakness) so that e-ink can function as a general-purpose laptop.
All e-ink use-cases boil down to "slow-paced and doesn't have high image requirements" - e.g. "comics work while photographs perhaps don't", or "static text works while moving text doesn't"

<br />





# Use cases for our proposed e-ink device
This section is for gathering which use-cases we believe should be supported. Please consider also what user problem this is intended to solve.

A higher-level view of this can be taken using "jobs to be done" (JTBD) - we can also consider what the core "jobs" are that the device should solve. The tool of JTBD can be a bit tricky as there are very different levels to look at them from, thus I would suggest tackling this separately.

Note - this is something that I think we should involve the entire group in, however we can start and consider how best to gather input (e.g. through a survey, which would be simpler if we have already a set of inputs rather).

Anything specific here would clearly require custom UI for the device. I have no idea if that is at all possible for this project. Even if not, it is at least an interesting though experiment :)

<br/>


## Device goal
This would be to describe what the device is intended to do in general, its high-level goal. Likely this is too early, but feel free to provide suggestions.

### Goal suggestion 1 - robooneus (example):


*Core JTBD / functions:*

* Write - contents of all kinds
    * [Text editor case study](/YpI3eg2mTkSxtAb1aTw0Hw)
* Code
* E-mail
* Chat? (e.g. Zulip)

*Secondary JTBD / functions:*

* Read articles, books, written content
* View images
    * I see this as something that is a "necessary evil" in some cases, for example graphs and images in papers, textbooks, etc. Or in books, other things.


*Excluded JTBD / functions:*

* Watch videos


<br/>




## Design Principles and Considerations

### Interaction Design

### Visual feedback

### Visual clarity



