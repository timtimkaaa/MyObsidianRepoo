---
banner: "![[flowersjpg.jpg]]"
cssclasses:
  - dashboard
banner_x: "0.5"
banner_y: 1
---
# Choose your journey...

- 📝 Notes
	- Knowledge: `$=dv.pages('"All/Knowledge"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`  
	<br>
	- Mind: `$=dv.pages('"All/Mind"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link` 
	<br>
	- Drinks: `$=dv.pages('"All/Food and drinks/Drinks"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link` 
	<br>
- 🚑 First aid toolkit:
	- [[Reasons to live and not consume rn]]
	#
	-  [[Checklist of things to feel happy right now]]
	#
- 📖 Studying
`$=dv.list(dv.pages('"All/Studying"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
	
- 📲 UX
	- [[UX to learn]]
	<br>
	
	- [[ToDo]]
	<br>
	
	- [[UX Portfolio]]
<br>
- 🎨 Art
	- [[Art !deas]]
	<br>
	- [[Art Gallery]]
<br>
- 🧾 Latest art reviews
`$=dv.list(dv.pages('"All/Art/Reviews"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- Stuff
	- [[Attitudes]]
	- [[Structuring my mind]]
	- [[Emotions]]

# Other stuff

- 📮 Inbox: 
`$=dv.list(dv.pages('"All/Inbox"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ✅ TODOs: 
`$=dv.list(dv.pages('"All/TODOs"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ☕ Brewing:
`$=dv.list(dv.pages('"All/Projects in progress"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- 🗃️ Oldest knoledge updates: 
	`$=dv.list(dv.pages('"All/Knowledge"').sort(f=>f.file.mtime.ts,"asc").limit(4).file.link)`
- 📊 Stats:
	- Total Files: `$=dv.pages().length` 
	- Inbox Items: `$=dv.pages('"All/Inbox"').length`
	- Music: `$=dv.pages('"All/Music"').length`
	- Mini-essays: `$=dv.pages('"All/Knowledge"').length + dv.pages('"All/Mind"').length`
	- Mind: `$=dv.pages('"All/Mind"').length`
	- UX: `$=dv.pages('"All/Knowledge/UX"').length`