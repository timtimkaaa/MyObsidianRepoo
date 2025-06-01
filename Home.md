---
banner: "![[flowersjpg.jpg]]"
cssclasses:
  - dashboard
banner_x: "0.5"
banner_y: 1
---
# Choose your journey...

- 🧠 Mind and inner world
	- [[Attitudes]]
	- [[Structuring ]]
	- [[Emotions]]
	- [[Study Spirituality]]
	- [[Study Philosophy]]
	- [[Study Mini-essays]]
- 🎨 Art
	- [[Art Mini-essays]]
	- [[Art !deas]]
	- [[Art Gallery]]
	- [[Study Music]]
	- [[Study Art]]
- 📲 UX
	- [[Study UX]]
	- [[UX Portfolio]]

# About vault

- 🗃️ Recent file updates: 
	`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- TODOs:
`$=dv.list(dv.pages('"TODOs"').sort(f=>f.file.mtime.ts,"desc").file.link)`
- ☕ Brewing
- 📊 Stats
	- Total Files: `$=dv.pages().length` 
	- Music: `$=dv.pages('"Mind"').length`
	- Sermon Notes: `$=dv.pages('"Sermon Notes"').length`
	- Inbox Items: `$=dv.pages('"Inbox"').length`
	- Journal Entries: `$=dv.pages('"Daily Notes"').length`