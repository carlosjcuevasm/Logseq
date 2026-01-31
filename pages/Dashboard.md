-
	- Code
	  {{query (and (task TODO) (tag code))}}
	- Cook
	  collapsed:: true
	  {{query (and (task TODO) (tag cook))}}
	- Home
	  collapsed:: true
	  {{query (and (task TODO) (tag home))}}
	- Other
	  {{query (and (task TODO)
	               (not (tag code))
	               (not (tag cook))
	               (not (tag home)))}}