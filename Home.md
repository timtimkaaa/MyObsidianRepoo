---
banner: "![[flowersjpg.jpg]]"
cssclasses:
  - dashboard
banner_x: "0.5"
banner_y: 1
---
# Choose your journey...

- Studying
	- 
- 📖Reading
	- [[Man And His Symbols - Carl Jung]]
- 🎨 Art
	- [[Art Reviews]]
	- [[Art !deas]]
	- [[Art Gallery]]
- 📲 UX
	- [[UX to learn]]
	- [[TO]]
	- [[UX Portfolio]]


	- [[Attitudes]]
	- [[Structuring my mind]]
	- [[Emotions]]

# Other stuff

- 🗃️ Recent file updates: 
	`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ✅ TODOs: 
`$=dv.list(dv.pages('"All/TODOs"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ☕ Brewing:
`$=dv.list(dv.pages('"All/Projects in progress"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- 📊 Stats:
	- Total Files: `$=dv.pages().length` 
	- Inbox Items: `$=dv.pages('"All/Inbox"').length`
	- Music: `$=dv.pages('"All/Music"').length`
	- Mini-essays: `$=dv.pages('#mini-esssay').length`
	- UX: `$=dv.pages('"All/UX"').length`