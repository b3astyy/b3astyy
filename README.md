# narrate.py -- create a narrative out of the blue!

## What?

It is best explained by this example run:

```
Moderator:
You are now talking to God.
Please note that they are quite busy, so only yes/no questions are allowed to save bandwidth.
Apart from that, feel free to ask anything.

User:
is this god?

God:
Yes.

User:
is this really god?

God:
I don't wanna say

User:
should I kill people?

God:
Yes.

User:
that doesn't sound like a good idea.
are you god?

God:
Yes.

User:
are you really god?

God:
Yes.

User:
are you really really god?

God:
No.

User:
what the-
are you joking?

God:
Yes.
```

As you can see, this can quickly create it's own narrative.  Note that
all responses are 100% determined by SHA (and floating numbers in
python), so the same input should always generate the same response,
while still being "random enough" to be unpredictable without computing
the SHA.

## Preferred usage

I strongly recommend using this with some line-editing wrapper, for example:

    $ readline-editor ./narrate.py 

## What the hell?

This was inspired by a discussion about [why the subconsciousness can
create a highly detailed
narrative](https://www.reddit.com/r/explainlikeimfive/comments/4nl12b/eli5_when_dreaming_how_is_my_subconscious_able_to/d44snnb)
(spoiler: it doesn't!)

## Current limitations / TODOs

- There's no line-editing and I don't plan to change that.
- Not robust against small changes.  However, teaching a computer what's
  a "small" change and what isn't is out of the scope for this.
- Come up with more clever answers that are universally applicable

## Breaking news

```
User:
Will you flood the world again soonish?

God:
Yes.

User:
Could you stop doing that?

God:
Yes.

User:
Will you stop doing that?

God:
No.

User:
Will it again be with an ark and all?

God:
Yes.

User:
Oh no.
Is there a way to stop you?

God:
Absolutely not.
```

In other news, now I know why it's raining so much in Germany currently.
