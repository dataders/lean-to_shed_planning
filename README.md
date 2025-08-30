# handy dad in the machine

[current iteration of the plan](outputs/comprehensive-plan.md)

## background

I've never built a lean-to roof before, but as a father of two, I am in desparate need of both
- storage for
  - vague gestures at everything 
  - an emergent ebike obsession
- an excuse to
  - buy more powertools
  - have time to myself and work on project that's nominally for the benefit of the family

While I could call my own father, or bug my very handy neighbor. Why shouldn't an LLM help me do this?

We are now in the era of the handy dad acheiving singularity. He is in the machine. His capacity to use the computer and internal has increased enormously. His emotional availability is unchanged.

I find myself alone for Labor day weekend, which is a perfect opportunity to make progress on this project.

Now, I'm halfway through the first of only two full days I'll have to myself for the foreseeable future.

It totally makes sense to prioritize documenting my AI-assited journey to planning and building this lean-to roof, right? This isn't a side quest at all, right right?

Help me Handy Clanker Dad!

## the journey

### before today

I've been dreaming of a lean-to shed for two years now. I borrowed post hole diggers ahead of a long weekend 9 months ago.

<img width="200" alt="evidence" src="images/request.png" />

After procuring the post-hole diggers, I did nothing for 8 months until last month at which point I finally dug and poured 3 concrete piers with brackets for 4X4 posts.

Fun! But now I'm somewhat overwhelmed with all the new terminalolgy so I'm leaning hard into what I am good at: Googling and vibe-coding. Here goes nothing

### today (pre Claude)

Below is [`spec_v0.md`](inputs/spec_v0.md), the prompt I began with originally and asked of ChatGPT5. 



> i need plans, materials, and instructions for a lean-to roof i'm planning on building against the pre-existing shed in my backyard.
> 
> some relevant info:
> - the ledger board height will be about 7.5 above the ground
> - the roof will be a single slope
> - the roof will be 16 feet long
> - distance between the shed and the posts will be about 6 feet
> - i've already made concrete piers for the posts with 4x4 simpson strong ties
> - there are 3 piers spaced 8 feet apart

The results didn't feel comprehensive, so I modified the prompt to be this instead

> what information is missing from the below information that a contractor would need to know in order to write up plans and a materials list for a lean-to roof i'd like to have built against the pre-existing shed in my backyard?

A productive dialogue ensued in which I was able to manually refine my list of bullet points which became [`spec_v1.md`](inputs/spec_v1.md)


> i need plans, materials, and instructions for a lean-to roof i'm planning on building against the pre-existing shed in my backyard.
> 
> some relevant info:
> - roofing material the i plan to use corrugated steel panels
> - target pitch: 2:12
> - the ledger board height will be about 7.5 above the ground
> - distance between the shed and the posts will be about 6 feet
> - the roof will hang 6 inches past the beam on the down side of the roof
> - there will be no overhang on the sides of the roof 
> - 9 2x6 rafters 24" on center
> - 2x4 purlines at 24" on center
> - horizontal projection (run) of roof is 6.5 feet
> - the roof will be a single slope
> - the roof will be 16 feet long
> - there will be 3 4x4 posts spaced 8 feet apart supporting the roof opposite the shed wall
> - i've already made concrete piers for the posts with 4x4 simpson strong ties
> - drip edges
>   - eaves (low end) D-style
>   - top (shed wall end) L-style
> - Synthetic underlayment

### prep for Claude

To bring Claude into the mix, I stand on the shoulders of giants and steal heavily from one @dbeatty10 made for an internal project of ours. The things I like that I'm cribbing:
1. `Workflow Improvement Protocol`: automatically trigger workflow to refine the worflow and documentation after every prompt
2. a `CHAT_LOG.md` to preserve our conversation

I'm also introducing the concept of an `outputs/` directory into which I put the current state of my specification, that I'd like to iterate on with Claude.

Right now it's just a single markdown file, but I can foresee if being a number of files like:
- a diagram
- materials list
- shopping list for Lowes
- instructions

