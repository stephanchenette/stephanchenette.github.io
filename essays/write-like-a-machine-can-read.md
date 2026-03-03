---
layout: default
title: Write Like a Machine Can Read
permalink: /write-like-a-machine-can-read/
essay: true
---

# Write Like a Machine Can Read

*March 2026*

For the last several years I've been obsessively organizing my notes. Obsidian vaults, Notion databases, tagging systems, folder hierarchies, daily templates. I spent more time than I'd like to admit getting the structure right. And it was right. For me.

The problem is that I now have a second reader.

I run a constellation of AI agents that help me manage my life and work. They check my calendar, process my meeting notes, surface tasks I've forgotten, draft messages in my voice. They're good at this. But every time one of them tries to read my carefully organized Obsidian vault, I watch it struggle with the same thing: my notes were never written for it.

This isn't a minor inconvenience. It's a fundamental design problem that almost nobody is talking about clearly. We've spent a decade building personal knowledge systems optimized for one audience, ourselves, and now we have a second audience that reads completely differently, and we're trying to serve both with the same files.


Here's what I mean. When I write a meeting note, I use shorthand. I reference people by first name. I use → arrows for action items. I bold things that matter to me visually. I nest toggles. I have a color system. All of this makes the note instantly scannable when I open it a week later. I can glance at it and reconstruct the entire meeting in seconds.

An LLM cannot glance. It doesn't benefit from bold text or color or spatial layout. What it needs is something much more boring: clear, unambiguous text with explicit metadata. It needs to know that "Sarah" is Sarah Chen from the product team, not Sarah my neighbor. It needs the action items tagged in a way it can parse, not styled in a way that catches my eye. It needs dates in ISO format, not "next Tuesday."

These are two fundamentally different consumption patterns, and we've been pretending they're the same.


The realization hit me when I added a file watcher to my Obsidian vault. Every time a meeting note gets saved, an AI agent picks it up, reads it, extracts action items, and adds tasks to my daily note. Simple enough. But I kept finding it was misclassifying things, missing context, and creating duplicate tasks. Not because the AI was dumb, but because my notes were optimized for a human who already had the context. The AI had to guess, and it guessed wrong often enough to be annoying.

So I started adding frontmatter. YAML headers with structured fields: meeting type, attendees as wiki links, company names, tags. Ugly to look at, but suddenly my agents could reliably tell the difference between a customer call and an internal standup without reading the whole note and inferring.

And here's the thing that surprised me: the frontmatter made the notes better for me too. Not because I read YAML for fun, but because the discipline of filling in those fields forced me to be precise about what just happened. Who was actually there? What company? What type of meeting was this really? I started making fewer sloppy notes.


This echoes something Nate Lee said in a recent video about building "agent-readable" knowledge systems. He made the observation that the internet is forking. There's the human web with fonts and layouts, and the emerging agent web with APIs and structured data. And he argues that your personal notes are forking in exactly the same way.

He's right about the fork. But I think he undersells the harder problem, which is that most of us don't want two separate systems. We don't want a pretty Obsidian vault for ourselves and a Postgres database for our agents. We want one set of notes that serves both audiences. The question is whether that's possible without making the notes worse for either one.

I think it is, but it requires a shift in how we think about writing for ourselves.


The shift is this: treat your notes like an API with a nice frontend.

The underlying data should be structured, explicit, and machine-parseable. The surface presentation can be whatever makes you productive. Your colors, your shorthand, your spatial layout. But the structure underneath has to be legible to something that doesn't have your context.

In practice this means a few things. It means frontmatter matters. It means naming conventions matter. It means when you reference a person, you use a consistent format your agents can resolve. It means your folder structure should encode information, not just organize visually. It means your templates should generate both the human-friendly layout and the machine-friendly metadata in one action.

None of this is technically hard. What's hard is the habit change. For years, the only question I asked when organizing my notes was "can I find this later?" Now the question is "can I find this later, and can a machine find it too, and can it understand what it found?"


There's a deeper point here that I keep coming back to. Toby Lütke, the Shopify CEO, said something provocative recently. He thinks a lot of corporate politics amounts to "bad human context engineering." People are unclear about what they mean, what they want, and what they decided, and the ambiguity creates space for dysfunction.

I think there's a personal version of this. A lot of the friction in our personal knowledge systems is just bad personal context engineering. The notes we can never find. The tasks that fall through the cracks. The decisions we remake because we forgot we already made them. We write things in a way that feels sufficient in the moment but is actually ambiguous. We rely on our own memory to fill in the gaps.

AI agents can't fill in those gaps. They take what you wrote literally. And the beautiful irony is that writing clearly enough for an AI to understand forces you to write clearly enough that your future self will understand too. Your future self is a lot more like an AI than you think. Limited context. No memory of the emotional state you were in. Just the text on the page.

Optimizing for machines turns out to be optimizing for your own forgetfulness.


I'm not suggesting you turn your journal into JSON. The human experience of writing and reviewing notes matters. There's a reason people love Obsidian's graph view, or Notion's gallery layouts, or even just the satisfaction of a well-organized folder tree. These are features for humans, and they should stay.

But underneath the human-friendly surface, there needs to be a machine-friendly skeleton. Structured metadata in the frontmatter. Consistent naming patterns. Explicit references instead of ambiguous shorthand. Templates that generate both at once so you don't have to think about it.

The people who figure this out are going to have a compounding advantage. The ones who build personal knowledge systems that serve both audiences without degrading the experience for either. Every note they write gets better for them and simultaneously makes their AI agents more capable. Every new tool they try can immediately access their full context. They stop re-explaining themselves to every new chat window, every new model, every new agent.

The people who don't will keep maintaining two separate systems, or more likely they'll keep a beautiful human system that their AI can barely read, and they'll wonder why AI still feels like a party trick.


We're in a weird transitional moment. The tools haven't caught up to this problem yet. Obsidian doesn't have a "make this agent-readable" button. Notion's AI features are bolted on, not foundational. Most knowledge management apps are still designed as if the only reader is a human with a mouse.

That will change. But you don't have to wait for the tools. You can start now by changing how you write. Add the frontmatter. Be explicit about who and what. Use consistent formats. Think of every note as something that two very different readers will need to understand.

It's a small change in habit that unlocks an entirely different relationship with AI. And it turns out, it makes you a clearer thinker too.
