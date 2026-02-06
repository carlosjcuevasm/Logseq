- {{renderer :kanban_651a3832-a06f-4dee-8c77-bc15908765e8}}
- ## Work Items #v.kanban
	- Pending
		- A work item
		- another one
		- {{query (and [[work-item]] (task TODO LATER) (not (page Templates)))}}
		  query-table:: false
		-
	- Working
		- [[prueba work item]]
		  #defenses
		- {{query (and [[work-item]] (task NOW DOING "IN-PROGRESS"))}}
	- Done
		- {{query (and [[work-item]] (task DONE))}}
-
-
- ## All
  collapsed:: true
	- TODO
	  :LOGBOOK:
	  CLOCK: [2026-02-06 Fri 00:24:49]
	  :END:
		- {{query (task NOW LATER TODO DOING "IN-PROGRESS" WAIT WAITING)}}
		  collapsed:: true
	- :LOGBOOK:
	  CLOCK: [2026-02-06 Fri 00:25:25]
	  :END:
-
-
-
- TODO hola
-
-
-
- ## TODO WorkPack
  type:: work-item,work-pack
  collapsed:: true
  :LOGBOOK:
  CLOCK: [2026-02-06 Fri 02:29:45]--[2026-02-06 Fri 02:30:06] =>  00:00:21
  CLOCK: [2026-02-06 Fri 02:30:10]--[2026-02-06 Fri 02:30:12] =>  00:00:02
  :END:
  #work-item #work-pack
	- **Intent:**
	- **Priority:**
	- **Topics:**
	- **Type:** work-pack
-
-
- TODO hola
  :LOGBOOK:
  CLOCK: [2026-02-05 Thu 23:42:30]--[2026-02-05 Thu 23:42:31] =>  00:00:01
  CLOCK: [2026-02-05 Thu 23:42:31]--[2026-02-05 Thu 23:42:31] =>  00:00:00
  CLOCK: [2026-02-05 Thu 23:42:34]--[2026-02-05 Thu 23:42:34] =>  00:00:00
  CLOCK: [2026-02-05 Thu 23:42:35]--[2026-02-05 Thu 23:42:35] =>  00:00:00
  :END:
- id:: 69811683-c7cf-496d-8288-55b92b8d0483
- ## WorkItem 1
  type:: work-item
  status:: pending
  collapsed:: true
	- **Notes:**
	- **Attributes:**
	  collapsed:: true
		- **Topics relation:**
		- **Work pack:**
		- **Priority:**
		- **Time Est (hrs):**
		- **Cognitive Load:**
		- **Success (this sprint):**
		- **Sprint:**
		-
-
- ## WorkItem 2
  type:: work-item
  status:: working
  #v.self-border
	- **Notes:**
	- **Attributes:**
	  collapsed:: true
		- **Topics relation:**
		- **Work pack:**
		- **Priority:**
		- **Time Est (hrs):**
		- **Cognitive Load:**
		- **Success (this sprint):**
		- **Sprint:**
		-
-
-
- ## WorkItem 3 
  type:: work-item
  status:: pending
  #v.self-border
	- **Notes:**
	- **Attributes:**
	  collapsed:: true
		- **Topics relation:**
		- **Work pack:**
		- **Priority:**
		- **Time Est (hrs):**
		- **Cognitive Load:**
		- **Success (this sprint):**
		- **Sprint:**
		-
-
- ## TODO WorkItem
  collapsed:: true
  :LOGBOOK:
  CLOCK: [2026-02-05 Thu 23:03:00]--[2026-02-05 Thu 23:03:01] =>  00:00:01
  CLOCK: [2026-02-05 Thu 23:03:02]--[2026-02-05 Thu 23:03:03] =>  00:00:01
  CLOCK: [2026-02-05 Thu 23:03:04]--[2026-02-05 Thu 23:03:05] =>  00:00:01
  CLOCK: [2026-02-05 Thu 23:03:10]--[2026-02-05 Thu 23:03:12] =>  00:00:02
  CLOCK: [2026-02-05 Thu 23:03:14]--[2026-02-05 Thu 23:03:14] =>  00:00:00
  CLOCK: [2026-02-05 Thu 23:03:15]--[2026-02-05 Thu 23:03:15] =>  00:00:00
  CLOCK: [2026-02-05 Thu 23:03:16]--[2026-02-05 Thu 23:03:16] =>  00:00:00
  CLOCK: [2026-02-05 Thu 23:03:17]--[2026-02-05 Thu 23:03:17] =>  00:00:00
  CLOCK: [2026-02-05 Thu 23:03:37]--[2026-02-05 Thu 23:03:39] =>  00:00:02
  CLOCK: [2026-02-05 Thu 23:04:53]--[2026-02-05 Thu 23:04:58] =>  00:00:05
  CLOCK: [2026-02-06 Fri 02:54:47]--[2026-02-06 Fri 02:54:49] =>  00:00:02
  :END:
  #work-item
	- **Notes:**
	- **Topics relation:**
	- **Work pack:**
	- **Priority:**
	- **Time Est (hrs):**
	- **Cognitive Load:**
	- **Success (this sprint):**
	- **Sprint:**
	- **Status**:
-
- Pending
	- {{query (and (property type work-item)(property status pending))}}
	- {{query (and (property type work-item)
	               (property status pending))}}
- Working
	- {{query (and (property type work-item)
	               (property Status working))}}
- Done
	- {{query (and (property type work-item)
	               (property Status done))}}
-
-
- # Items Backlog
	- ## name
	  collapsed:: true
		- **Intent:**
		- **Priority:**
		- **Topics:**
		- **Type:** work-pack