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
* Code
* E-mail
* Chat? (e.g. Zulip)

*Secondary JTBD / functions:*

* Read articles, books, written content
* View images
    * I see this as something that is a "necessary evil" in some cases, for example graphs and images in papers, textbooks, etc. Or in books, other things.


*Excluded JTBD / functions:*

* Watch videos






#Design Principles and Considerations

#A hodgepodge list of theorized UI design principles for an e-ink text-editor (if you insert a point and change the numbering, please update the number references):
    1. Paginate screens, don't scroll (we already knew that)
    2. Because refreshing takes longer than LCD, the user can't easily spot an instantaneous change of the screen contents, and is liable to forget the exact layout of the screen when it flickers and some part of it changes. Thus, if it's not extremely obvious what changed, we should have some lasting indication of what just changed after a screen refresh. For instance, a column next to line numbering with a "*" on the lines that just changed.
    3. This is a more general principle, but newbies aren't familiar with the exact behaviour of the program, so anything that's surprising (which could basically be anything) should be conveyed for a sec or two after it happens. I'm pretty sure this is why animation exist on LCD-screen UIs (e.g. a screen minimizes without warning and even though you weren't looking at it, the motion draws your eye after half a second and the 1-second animation means you still have half a second of watching the animation to understand it's moved to the taskbar).
    4. Refreshing = you're blind for a couple of seconds and can't navigate or check stuff = sucks and should be minimized as much as possible. As in, minimize the number of partial refreshes and also avoid full-refreshes when a partial refresh would do. A few ideas for how to counter this:
        a) if you're editing a line with text after the cursor, then instead of constantly reflowing the entire paragraph, perhaps either:
            i) overlay the edit until the user stops  typing and then reflow the entire thing just once
            ii) put the typing into a separate blank spot on screen then put an arrow to indicate where the text will be placed (perhaps if we have a full line's worth of vertical empty space between lines,  we can just have the typing displayed between the lines below with a ^.), or
        b) if you're adding to a line and you need more space from the paragraph below you, perhaps a partial refresh could simply shrink the one paragraph below without needing to shrink any paragraphs *below the below*. Obviously, un-shrink the paragraph after a full reflow.
        c) if you're deleting text, just use a strikethrough temporarily, perhaps? This might be an unnecessary delay that merely damages the immediacy of the action, especially if you've already highlighted the section. Worth testing idk.
    5. Following on from 3 and 4b, if a *lot* of stuff moved around on the screen, then it would be helpful to explain what went where. Especially if your reflow involves both unshrinking a paragraph and reflowing the text below it. Ideas for making a full-screen refresh/reflow clearer:
        a) Similar to the "asterisk column" idea from point 2, perhaps a line for each paragraph that moved going from where it was *before* the refresh to where it is *after*. Obviously we'd need to do a bunch of texting (with yet another effing text editor, because clearly the world needs more of those lol)
        b) Perhaps make a full reflow a manual action bound to a button. This completely removes the chance of a "surprise refresh".
        c) Instead of refreshing the whole screen at once, maybe refresh each 'step' individually so maybe it's clearer? As in, either:
            i) refresh each e.g. 20% of the screen (split horizontal into bundles of lines)  one at a time, from top to bottom
            - ^here see partial refresh of eink screens
            ii) do each logical reflow action separately - so, do a strikethrough then another strikethrough then unshrink a paragraph etc etc in the order the user right did it.
        d) Maybe show a "minimap" of what a whole-screen reflow would look like, before it refreshes? As in, have a permanent minimap that updates more-or-less immediately. Would work well with the "manual refresh"  and the 5a.

##Interaction Design

##Visual feedback

##Visual clarity



