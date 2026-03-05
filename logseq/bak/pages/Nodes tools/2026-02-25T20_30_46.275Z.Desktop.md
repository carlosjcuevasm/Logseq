-
- Todas lo que importa y haces en la vida, es y/o puede ser un nodo, clasificable.
  Aquí un sistema para tomar control, tener una vida mas deseada. 
  Que todo lo que realmente importa, tenga excelente oportunidad de suceder.
  Ser mas completo, ser mas coherente, 
  ser mas tu, ser mas feliz.
- los anhelos más profundos de tu corazón puedan realizarse y quedarse contigo para siempre! 
  Puedes ser feliz. Siempre que mires tu exterior e interior puedas sentirte plenamente orgulloso de la persona que eres!
-
- *Every serious system has:* **A backlog of commitments** and **A way to advance some now**.
  collapsed:: true
	- Any system that _works_ must:
	  collapsed:: true
		- externalize memory
		- prioritize
		- limit scope
		- break work down
		- review and adjust
	- whether it’s called **GTD**, **Agile**, **Kanban**, or something developed independently in another culture, the **DNA converges**.
		- backlog exists
		- commitment windows exist
		- execution queues exist
		- review cycles exist
	- There really aren’t many other viable shapes.
	- Thus this my system here...
	- The win isn’t inventing a new shape; it’s **knowing why the shape exists**, so you can adapt it consciously instead of obeying it blindly.
- Model + Control System
- A great faming is goal or intent and  competency statement.
  A good “success looks like” statement is something you’d be proud—and safe—to say out loud in a professional setting or any.
	- why works:
		- Forces **transfer**, not memorization
		- Converts learning into **identity-level skill**
		- Makes progress falsifiable (“can I say this honestly yet?”)
	- example:
		- **Goal**: Learn graph science as a foundation for system design.
		- **Success look like:** I can reason about complex systems using dependency graphs, dataflow, and reactive principles, and explain design tradeoffs clearly
-
- [[Graphs]]
-
-
-
- ## **Life-operating system**
  id:: 697d200f-b7dd-4fe8-83db-663020ce8569
  for Provision / Expression / Recovery.
- The system strategy is fragmentar en base a prioridad y balance.
  collapsed:: true
	- What makes it _not_ just a task list is that **each layer narrows the pool differently**.
	- Steps
	  collapsed:: true
		- fragmenting time
		- pulling items from a pool
		- committing progressively (month → sprint → week → day)
- You'll realize each step owns it's proper item unit that enables it to be realized
  collapsed:: true
	- **Work Item notes** - This is the basic unit of work. This feature enable work breakdown or fragmentation.  You'll realize basic props almost to be mandatory. For instance,  for a sucessful  time workload planning for a sprint, weekly etc you'll need some type of work item estimation, hence time estimation. For cognitive load managmenet, you'll need a congnitive complexity. And so on for other things
- **Time-scaled control system**:
	- **Backlog** - All items you know about. Intentions, ideas, topics. Refined or not.  This is the inventory of nodes.
		- ( Kanban board one for easy handy)
		- [[Items Backlog]] ( a general one)
	- **Pack / Monthly planning** - Prioritization happens. What the main goals for the month are. Active builds and why them to anchor meaning
		- [[Monthly planning]]
	- **Sprint review and planning** - Is a commitment to items window . Respond to the monthly goals. Working items in packages, 2-week (or similar). Also Completed + % progress
		- [[Sprint planning]]
	- **Kanban. Work item tracker**  — Main tool for knowing what is committed to work on. Sprint scope. A state machine for items with overall view. Results form the sprint planning. Pending / Working / Done.
		- [[Kanban board]]
	-
	- **Weekly planning** — Weekly,  load management. This reflects sprint goals, now made a specific week intent.
		- TODO plantilla. Creo que esto es mas reflexion que otra cosa
	- **Daily agenda | daily view** — Daily organizer, what to do today. What to take in work items. Might just be Journals page.
		- {{journal}}
	- ---
	- **Reasoning:** Each step fragments the big goal
	  collapsed:: true
		- Monthly → sets direction and meaning
		  Sprint  → selects commitments
		  Kanban  → tracks state of commitments
		  Weekly  → balances load
		  Daily   → executes
	- ---
- Remember, is a life operating model. Thus, managing commitments under uncertainty.
- #### Fun facts
	- This is "Agile" methodology
	  collapsed:: true
		- | Scrum Concept | Your Life System |
		  | --- | --- |
		  | Product backlog | Nodes Backlog |
		  | Product vision | Provision / Expression / Recovery |
		  | Sprint goal | Monthly + Sprint planning |
		  | Sprint backlog | Kanban |
		  | Daily standup | Daily agenda (journal) |
		  | Sprint review | Sprint review + % |
		  | Sprint retrospective | Weekly planning reflection |
		  So yes — structurally, this **is Agile**.
		  Without forcing it, I just rediscovered Agile. Kanban as a tool made it extremly apparent.
		  It all started after the life as node system and how to organize work on it
	- Why this actually works
	  collapsed:: true
		- The system:
			- forces prioritization
			- fragmented workload by layers
			- makes commitment explicit
			- limits active work
	- If life is a node graph, use tools sharing that concept.
		- Probably a **low-level environment**
		  collapsed:: true
			- A **low-level environment** gives basics:
				- primitives (pages, blocks, links, tags)
				- composition instead of prescription
				- _no assumed workflow_
			- It does **not** assume pipelines:
				- what you’re building
				- why you’re building it
				- how work should flow
			- You assemble meaning yourself.
			- Environments give you _building blocks_.
			  Workflows give you _paths_
			- Logseq and Notion both fall into this category.
		- Logseq is a "everything is a node" approach.
			- It does all with "primitives"
				- It has only two **first-class** things: **Pages and Blocks**
				  That’s why it feels powerful instead of restrictive.
					- Pages and blocks are almost the same thing. 
					  A **page is a bock that got it's own file** to exist. Both can hold same capacity for content
					  This means a page has addressability outside Logseq. Is a top level block, etc
					  Pages feel “heavier” (navigation, namespaces, titles), Blocks feel “lighter” (thoughts, items, structure)
				- pages = nodes
				- links = relationships
				- templates = structure
				- kanban/query = views
			- Features like tags or properties etc are made using the primitives
				- They are essentially parsed, indexed metadata. You tell Logseq to "parse this words" because they would be used to discriminate things later.  Logseq cant parse all words unncessaryly, so you tell it "theses are discriminators". Be it tags or properties.By using the designated symbols, you let Logseq know those should be parsed.
					- Logseq is DOM + CSS thus, this tags or props become selectors in the css. Which means, customized views for end users. Deliberelty, they stay away from visual customization.
				- Tags: not a separate object. Tags are simply links to a page. So #Hello, is a link to a page Hello. Is a indexed parsable link, so it serves as a discriminator for queruies etc.
					- A tag itself is a self-contained node, is a page after all, as everything else.
					- How is this done
					  collapsed:: true
						- When you write:
						- ```
						  `This is interesting #fun-fact`
						  ```
						- Logseq does this:
							- Creates (or links to) a **page** called `fun-fact`
							- The current block becomes a **reference** to that page
						- So:
							- `#fun-fact` ≡ `[[fun-fact]]`
							- No difference semantically
						- You can open the `fun-fact` page and:
							- Define it
							- Write what “fun fact” means
							- Add related notes
							- See **all blocks/pages that reference it**
						-
				- Property: Simply indexed relations. As tags, they help discriminate, by providing the feature of one attribute having many options, say type, or love-level etc. **But they work different than tags**. **Properties are not nodes**.  They describe the block; they don’t connect it. Logseq parses them for discrimination but the properties themselves are not node objects
				  collapsed:: true
					- This allow for interesting features, like a labeling system
						- > complexity:: 1 
						  priority:: 3
						- Even if you never visit the `complexity` page, it still exists as a node and can be defined, queried, or extended later. Maybe you never go to the "complexity" page, but if you wish to see it, it does exist
					- A property collects many relations under one shared semantic meaning. In essence, is acts as a namespace. Is the concept of tag, just lifted one level up into a named  group of relations.
			- You can template stuff
			  collapsed:: true
				- **Templates** → copy/paste automation
				- **Placeholders** → visual hints only
				- **Macros** → rendering / computed views
				- **Nothing is “interactive” in core Logseq**
		- Tips for written documentation
		  collapsed:: true
			- Writing primitives
			  collapsed:: true
				- Use punctuation for flow.
				- Use line breaks for readability.
				- Use blocks for structure.
				- Use nesting for dependency.
			- Advice
			  collapsed:: true
				- Use sentences for flow and readability
				  Use blocks to expose structure and intent
				- Over-blocking destroys narrative, narrative fragmentation.
				  Under-blocking hides structure.
	- This is life, thus value some and not some
	  collapsed:: true
		- explicitly modeled:
			- Recovery
			- drain vs restore
			- load,
		- **didn’t** introduce:
			- velocity obsession
			- story points theater
			- daily guilt tracking
-
-
-