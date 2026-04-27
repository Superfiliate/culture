# Product-Minded Engineering Playbook

**Status:** Draft outline

## Table of contents

1. Why this playbook exists
2. What product-minded engineering means here
3. Core principles
4. When to use this playbook
5. Working model
   - Before we build
   - During execution
   - After launch
6. Roles and expectations
   - Engineers
   - Squad Leaders
   - Godfathers
   - Engineering Managers
   - PMs and Designers
7. Lean spec template
8. Planning review checklist
9. Review trigger matrix
10. Spec clinics and planning reviews
11. Examples library
12. Adoption plan
13. Signs this is working

## 1. Why this playbook exists

Product-minded engineering starts from motivation. Engineers are drawn to this work for many reasons — the challenge of a hard problem, the elegance of a clean system, the craft of shipping something that works well. Product-minded engineers share all of that, but their center of gravity is the customer problem and the impact of solving it. Quality, performance, and architecture still matter deeply, and product-minded engineers hold a high bar on them, because those are what let us deliver better outcomes for customers and keep shipping as the product evolves.

At Superfiliate, we intentionally build a team of product-minded engineers. In a startup, we want everyone — including engineers — to be connected to the customer, the problem, and the business impact of their work. That mindset creates teams that move faster, make better trade-offs, and build systems that are easier to change, because change is part of serving customers well.

This playbook exists to make that mindset explicit. It documents the principles, expectations, and practices behind product-minded engineering at Superfiliate, so people can learn it, apply it, and use it as a shared reference across teams.

## 2. What product-minded engineering means here

Product-minded engineering means the work extends beyond code and execution. We seek the why behind what we build. We want to understand which problem we are solving, why it matters, and why now. That context is not optional. It is part of the job, and a core source of motivation. Product-minded engineers actively participate in problem framing, ask questions early, and help the team get sharper on the real problem before jumping to solutions.

It also means staying close to the business. We try to understand our customers, how they operate, the market we are in, and the trade-offs the company is making. We participate in brainstorms and product discussions, because product context is not owned only by Product or leadership. We use that context to suggest simpler solutions, challenge unnecessary complexity, and make better decisions.

It also means the work is not done when the code is merged. A product is only delivered when it reaches customers and we learn whether it actually solved the problem. A well-designed system or a clean data pipeline is not enough on its own if nobody uses what we built or if it fails to create value. That is why we care about adoption, feedback, data, and outcomes, and why we treat learning from launch as part of the job.

This mindset does not lower the engineering bar. It raises it. Product-minded engineering requires high standards in code quality, maintainability, observability, reliability, and performance, because we are playing the long game. Our customers' needs will keep evolving, so we need systems that are easy to change, issues that are easy to detect, and products that feel fast and dependable to use. Product and customer value are the north star behind these decisions.

## 3. Core principles

Product-minded engineering keeps engineers in builder mode. When people have context, trust, and room to move, the work becomes more energizing and the product gets better. It is hard to compete with people who are having fun, and building this way is genuinely fun. These principles are what make that possible.

- **Start with the why.** We seek context before we seek solutions. We want to understand the problem, why it matters, why now, and what success looks like before we start building.
- **Know your game.** We stay close to customers, the market, and the business. We understand how our customers operate, what pressures they face, and how Superfiliate wins, so our engineering decisions are grounded in reality.
- **Solve the problem, not just the request.** We do not treat our job as implementing requirements exactly as written. We help the team find the simplest and most effective way to solve the real problem.
- **Ask for forgiveness, not permission.** We do not create approval loops for low-risk, reversible decisions. When something is hard to reverse or affects other teams, we pause and align. Otherwise, we use judgment, communicate early, and move.
- **Overcommunicate to create autonomy.** Autonomy only works when people make their thinking visible. We share context, trade-offs, decisions, and risks early so others are not surprised and momentum does not depend on constant check-ins.
- **Optimize for learning and impact.** Shipping is not the finish line. We care about whether customers use what we built, whether it solved the problem, and what we learned from the result.
- **Quality sustains speed.** Code quality, observability, reliability, performance, and maintainability are not separate from product work. They are what allow us to keep shipping quickly, respond to change, and serve customers well over time.

## 4. When to use this playbook

This playbook is not a step-by-step guide for how our process works. It is intentionally process-agnostic. It is a guide for how we want engineers to think, behave, and stay motivated at Superfiliate. We expect every new engineer to read it at least once, and we believe it is useful for anyone in Engineering or Product who wants to understand the mindset behind how we operate.

It is most useful in moments that require alignment and judgment: when someone is joining the team, when a new project is starting, when trade-offs need to be made, or when a team feels like it is drifting into execution without enough context. In those moments, this playbook helps bring the conversation back to the same foundation: customer value, ownership, speed of learning, and high engineering standards.

Like our tech vision, this is closer to a manifesto than an operating manual. It is not meant to define every step of the process. It is meant to give us a shared philosophy we can come back to whenever we need to reset, realign, or remind ourselves why we work this way.

## 5. Working model

Product-minded engineering is not only about how we think. It changes how we work across the full lifecycle of a project: before we build, during execution, and after launch. This is not a rigid process. It is the default operating model we want engineers to follow.

### Before we build

Before we build, our job is not only to code and deliver what was asked. It is to find and solve problems in the best way possible. That starts by connecting with the why behind the work. Understanding the problem is not owned by any one team, but everyone; it is part of how strong engineers create value. It brings us closer to the customer, helps us contribute better ideas earlier, and gives us the context to make better technical and product decisions.

An engineer reaches their full impact when they are deeply involved in the problem, not only in the implementation. With real context, we can shape scope, challenge assumptions, and find a better path forward. That usually leads to simpler solutions, better trade-offs, and systems that are easier to evolve.

When we skip this and jump straight into implementation, we can add debt, lock ourselves into the wrong constraints, or miss the real problem entirely. We have seen this happen, and we have also seen the difference it makes when engineers invest early in understanding. In early 2026, Nicholas and Morgana were working on a difficult billing project that needed to support two providers in a part of the product that already had significant technical debt. Instead of jumping straight into implementation, they interviewed key stakeholders across Sales and Customer Success to understand the real pain points in the current billing model. That work helped them see a better path: a new billing architecture for new customers, keeping the old one as legacy. A better technical plan became possible because they invested early in understanding the real problem.

The same happened in the first Meta Ads projects. Leo and Ale were entering a completely new domain, with little internal knowledge and a challenging external API. They did not limit the work to technical exploration. They talked to ad buyers and marketers, including people outside the company, and studied competitor products to understand how those users actually work and how the APIs were being used in practice. This kind of research is one of the clearest ways engineers go above and beyond. It brings us closer to the problem, increases our ownership, and improves the quality of what we build. In this case, it gave them much better domain understanding, helped them navigate API limitations, and played an important role in us shipping a full Meta Ads suite with real ownership over the feature.

Once we understand the problem, a good habit is to look for the simplest version of a valuable solution. The goal is not to overthink the implementation. It is to focus on the smallest thing that can create meaningful value and teach us something. Quick prototypes are great tools here, because they help us validate direction with stakeholders and designers before we go too far. Breaking the work into smaller deliverables and weekly goals helps for the same reason: it gives the team visibility, creates a real sense of progress, and makes it easier to learn and adjust early.

We do not always map every risk, unknown, and dependency perfectly in advance, but we do care a lot about identifying irreversible decisions as early as possible. That is one of the reasons engineers should be involved early in problem definition. If one path creates major constraints, expensive mistakes, or hard-to-undo decisions later, we want to surface that while there is still time to choose differently.

Finally, before we build, we align on what success looks like. Our team is data-driven, and that is a big part of how we measure whether the work is actually succeeding. That may mean a business goal, a customer outcome, access to a specific capability, or a technical milestone that unlocks the project. What matters is that the team knows where it is trying to go, how it will know whether it got there, and which signals will tell us if we are on the right track.

### During execution

During execution, the goal is to ship the agreed solution to the customer without losing sight of the problem behind it. Product-minded engineers do not disappear into implementation and follow the original plan without reassessing. They keep solving the problem in real time. As reality gets clearer, new constraints appear, trade-offs change, and some decisions need to be made before a full alignment loop can happen. This is where ownership matters the most.

One important part of this is proactive communication. It means sharing the information that helps the team stay aligned: what changed, what is blocked, which trade-offs are being made, and where a decision may need support from others. Our culture already says this clearly: say it like you mean it. That means being honest, direct, and timely about what matters. If scope is drifting, if priorities changed, if something feels off, or if a decision needs support, we say it early. We do this with empathy and good intent, but we do not let vague communication create silent misalignment.

At the same time, we protect focus time. We are engineers, and execution is still mostly technical work. We need uninterrupted time to think, build, test, and ship well. That is why we keep our communication intentional, keep only the meetings that are truly useful, and protect enough deep-work time for real execution.

When ownership is high, engineers can use their judgment on behalf of the project. We saw this clearly in Communications. Carol and Salomao had already been involved in discovery and execution for multiple iterations, so when the PM and the designer were away for a few weeks, the squad did not stall. Carol designed the approach she believed was right for some features, Salomao already had a clear vision of what the sprint needed to achieve, and the team kept moving. When Dani came back, they aligned on what could be improved and refined it together. That speed was only possible because the engineers had enough context and enough ownership to make good decisions without waiting for every handoff.

We ship in slices. Breaking work into smaller deliverables creates checkpoints for the team to stop and ask again: are we still working on the most important thing right now? This matters because it is easy to get pulled into the unknown and lose track of what the project actually needs. Shipping in slices limits how far we can drift, helps us review progress earlier, and gives us more chances to adjust before too much time is spent in the wrong direction.

One of the reasons we ship in slices is to expose bad plans early. Rework is not always bad, but there are two very different kinds of it. One comes from misalignment: we say we are building something, but the team is not actually aligned on what it should do or why it matters. We ship it, it misses the value, and everyone gets frustrated. This is the kind of rework we want to avoid, and the right answer is usually to stop, realign, and change the plan early. The other kind of rework comes from learning. The team is aligned, we make a deliberate bet, we ship something, and we learn that it does not solve the problem as well as we expected. That is acceptable. That is how learning works. Reworking after a real hypothesis is very different from reworking because of avoidable misalignment.

During execution, quality still matters. We do not drop the engineering bar. Testing, observability, maintainability, and clear code are part of the standard, because they are what keep the codebase flexible enough for us to add, remove, and change things quickly. We do not over-optimize for performance or complexity before it is necessary, but we also do not treat quality as optional. The goal is to keep raising the standards of the codebase so we can preserve future speed while solving the customer problem in front of us.

### After launch

After launch, the work is not done. Launch is the beginning of learning.

When we say launch, we do not necessarily mean a public marketing launch. For Product and Engineering, something is launched as soon as customers can use it for real. That is when the product meets reality and we can start learning from actual behavior, not assumptions.

We try to start that learning as early as possible. We do not wait for the sprint to end if a slice is already good enough to be tested. Internal stakeholders and market experts can help us get signal faster, but customers are still the source of truth. They are the ones who tell us whether we actually created value.

This is where being data-driven becomes concrete. We want instrumentation, dashboards, usage metrics, performance signals, bug reports, and direct feedback loops that show us what is really happening. Fernanda's work on Product Instrumentation is a good example of this mindset: map the right events early so new projects can be measured from the start. Squads building Metabase dashboards to understand adoption and usage patterns are another.

After launch, we validate whether the work solved the problem. If it did, we build on it. If it did not, we fix it, adjust it, or change direction based on what we learned. And if we find issues while the squad is still active, we do not wait passively for the sprint to end. We align with Product, solve what matters in real time, and protect the customer experience.

This is also where Engineering and Product come back together most clearly. We share what worked, what failed, and what we should do next. We ship, we measure, and we learn. That is how we avoid confusing delivery with impact.

## 6. Roles and expectations

Ownership is one of the most important parts of making product-minded engineering work in practice. Everyone involved in a squad contributes to the product workflow, but not everyone carries the same kind of ownership. Some roles are closer to discovery, some are closer to delivery, and some exist to create leverage, unblock decisions, or grow the people doing the work.

Clear ownership helps the squad move faster because people know who to defer to for decisions, who should be consulted, and who is accountable for moving each part of the work forward. It reduces ambiguity, prevents unnecessary approval loops, and makes it easier to keep momentum without losing quality or alignment.

### Engineers

Engineers are the role with the strongest ownership over building the agreed scope. They are not only ticket-takers or implementers; they are expected to understand the problem, participate in shaping the solution, ask questions, challenge assumptions, and stay connected to the customer outcome.

Product, Design, Squad Leaders, and Godfathers can help shape, unblock, and refine the work, but engineers carry day-to-day ownership over implementation quality, progress, and delivery.

Engineers are expected to:

- Understand the why behind the work before building.
- Participate in problem framing, trade-off discussions, and scope decisions.
- Build the agreed scope with quality, maintainability, observability, and performance in mind.
- Communicate blockers, risks, and changes early.
- Ask for clarification when requirements, UX, or success criteria are unclear.
- Help validate the work after launch through bugs, usage, feedback, and data.

### Squad Leaders

The Squad Leader is an engineer with broader ownership over the squad's delivery. They lead execution from inside the work, not from above it. This role combines technical execution, product context, communication, and lightweight project management.

The Squad Leader helps the squad move from scope to shipped product. They stay hands-on, help break down the work, write or refine stories, coordinate QA, communicate progress, and make sure Product and Design are aligned before release.

Squad Leaders are expected to:

- Lead execution while staying close to the code.
- Help break scope into clear, shippable pieces.
- Pair with engineers and unblock day-to-day implementation.
- Keep Product and Design informed about progress, trade-offs, QA, and release timing.
- Help write or refine stories so the team knows what needs to be built.
- Own the squad's delivery rhythm and make sure risks are visible early.
- Protect both momentum and quality.

### Godfathers

The Godfather oversees one or two squads in the same product context. They are not usually responsible for day-to-day execution, but they carry strong ownership of the squad's deliverables and context around the work. Their role is to create technical leverage: unblock engineers, review important PRs, challenge weak plans, help with architecture, and make sure the squad is making sound technical decisions.

Because Godfathers have broader context, they are also important connectors. They help bring the broader product and technical vision into the squad, bridge communication with other stakeholders, and make sure local decisions fit the direction of the company and the codebase.

The Godfather should be involved enough to understand the product workflow and delivery risks, but not so involved that every decision depends on them.

Godfathers are expected to:

- Stay close enough to the squad context to give useful guidance.
- Review important PRs and technical decisions.
- Unblock engineers and Squad Leaders when they hit complexity or ambiguity.
- Help identify architectural risks, technical debt, and hard-to-reverse decisions.
- Raise the engineering bar without slowing the squad unnecessarily.
- Own the technical health and delivery confidence of the squads they support.
- Coach engineers through decisions instead of centralizing all authority.

### Engineering Managers

Engineering Managers are primarily responsible for the growth of engineers. Their focus is development plans, career growth, feedback, performance, motivation, and making sure engineers are growing into the level of ownership expected from the team.

They are not the main execution owner for squad delivery. They should understand the work well enough to coach effectively and spot patterns, but their main responsibility is the person, not the project.

Engineering Managers are expected to:

- Support engineers' growth, career development, and performance.
- Help engineers build stronger product judgment, communication, and ownership.
- Give feedback regularly and clearly.
- Identify growth gaps in technical skills, product thinking, collaboration, or execution.
- Partner with Squad Leaders and Godfathers to understand how engineers are performing in real work.
- Create development plans that help engineers increase their impact.
- Protect a high bar for engineering culture and expectations.

### PMs and Designers

PMs and Designers are essential to product-minded engineering. They bring depth on the customer problem, product direction, user experience, and the definition of success. Their work gives the squad the clarity it needs to make good decisions and build something that actually solves the problem.

In this model, they are not alone in translating product thinking into execution. Squad Leaders help with story-writing, QA, release communication, and alignment. Engineers participate earlier and more actively than in a traditional handoff model.

PMs and Designers are expected to:

- Bring customer, business, and product context into the squad.
- Partner with engineers early, before the solution is fully locked.
- Define the user experience and success criteria clearly.
- Collaborate with Squad Leaders on stories, QA, and release readiness.
- Stay available during execution as trade-offs and edge cases appear.
- Help validate whether the shipped work solved the problem.
