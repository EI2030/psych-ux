# UX case study - eink text editor

###### tags: `psych-ux` `ux` `case study` `productivity suite`

## 5 theorized UI design principles for an e-ink text-editor:

1. Paginate screens, don't scroll (we already knew that)

2. Because refreshing takes longer than LCD, the user can't easily spot an instantaneous change of the screen contents, and is liable to forget the exact layout of the screen when it flickers and some part of it changes. Thus, if it's not extremely obvious what changed, we should have some lasting indication of what just changed after a screen refresh. For instance, a column next to line numbering with a "*" on the lines that just changed.

3. This is a more general principle, but newbies aren't familiar with the exact behaviour of the program, so anything that's surprising (which could basically be anything) should be conveyed for a sec or two after it happens. I'm pretty sure this is why animation exist on LCD-screen UIs (e.g. a screen minimizes without warning and even though you weren't looking at it, the motion draws your eye after half a second and the 1-second animation means you still have half a second of watching the animation to understand it's moved to the taskbar).

4. Refreshing = you're blind for a couple of seconds and can't navigate or check stuff = sucks and should be minimized as much as possible. As in, minimize the number of partial refreshes and also avoid full-refreshes when a partial refresh would do. A few ideas for how to counter this:
    * a) if you're editing a line with text after the cursor, then instead of constantly reflowing the entire paragraph, perhaps either:
        * i) overlay the edit until the user stops  typing and then reflow the entire thing just once
        * ii) put the typing into a separate blank spot on screen then put an arrow to indicate where the text will be placed (perhaps if we have a full line's worth of vertical empty space between lines,  we can just have the typing displayed between the lines below with a ^.), or
    * b) if you're adding to a line and you need more space from the paragraph below you, perhaps a partial refresh could simply shrink the one paragraph below without needing to shrink any paragraphs *below the below*. Obviously, un-shrink the paragraph after a full reflow.
    
    * c) if you're deleting text, just use a strikethrough temporarily, perhaps? This might be an unnecessary delay that merely damages the immediacy of the action, especially if you've already highlighted the section. Worth testing idk.
    
    
5. Following on from 3 and 4b, if a *lot* of stuff moved around on the screen, then it would be helpful to explain what went where. Especially if your reflow involves both unshrinking a paragraph and reflowing the text below it. Ideas for making a full-screen refresh/reflow clearer:
    * a) Similar to the "asterisk column" idea from point 2, perhaps a line for each paragraph that moved going from where it was *before* the refresh to where it is *after*. Obviously we'd need to do a bunch of texting (with yet another effing text editor, because clearly the world needs more of those lol)
    * b) Perhaps make a full reflow a manual action bound to a button. This completely removes the chance of a "surprise refresh".
    * c) Instead of refreshing the whole screen at once, maybe refresh each 'step' individually so maybe it's clearer? As in, either:
        * i) refresh each e.g. 20% of the screen (split horizontal into bundles of lines)  one at a time, from top to bottom
            - ^here see partial refresh of eink screens
        * ii) do each logical reflow action separately - so, do a strikethrough then another strikethrough then unshrink a paragraph etc etc in the order the user right did it.
    
    * d) Maybe show a "minimap" of what a whole-screen reflow would look like, before it refreshes? As in, have a permanent minimap that updates more-or-less immediately. Would work well with the "manual refresh"  and the 5a.