---
banner: "![[flowersjpg.jpg]]"
cssclasses:
  - dashboard
banner_x: "0.5"
banner_y: 1
---
# Choose your journey...

- Studying
	- [[]]
- 📖Reading
- 🎨 Art
	- [[Art Mini-essays]]
	- [[Art !deas]]
	- [[Art Gallery]]
- 📲 UX
	- [[Study UX]]
	- [[UX Portfolio]]


	- [[Attitudes]]
	- [[Structuring my mind]]
	- [[Emotions]]

# Other stuff

- 🗃️ Recent file updates: 
	`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ✅ TODOs: 
`$=dv.list(dv.pages('"Remote/TODOs"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ☕ Brewing:
`$=dv.list(dv.pages('"Remote/Projects in progress"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- 📊 Stats:
	- Total Files: `$=dv.pages().length` 
	- Inbox Items: `$=dv.pages('"Remote/Inbox"').length`
	- Music: `$=dv.pages('"Remote/Music"').length`
	- Mini-essays: `$=dv.pages('#mini-esssay').length`
	- UX: `$=dv.pages('"Remote/UX"').length`