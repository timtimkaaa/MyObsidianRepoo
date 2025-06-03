---
banner: "![[flowersjpg.jpg]]"
cssclasses:
  - dashboard
banner_x: "0.5"
banner_y: 1
---
# Choose your journey...

- 📝 Notes
	- Learning: `$=dv.pages('"All/Learning"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`
	- Mind: `$=dv.pages('"All/Mind"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`
	- Drinks: `$=dv.pages('"All/Teas"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`
- 📖 Reading
	- [[NEW Man And His Symbols - Carl Jung]]
	- [[Moychay]]
- 📲 UX
	- [[UX to learn]]
	- [[TO]]
	- [[UX Portfolio]]
- 🎨 Art
	- [[Art !deas]]
	- [[Art Gallery]]
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
- 🗃️ Oldest file updates: 
	`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"asc").limit(4).file.link)`
- 📊 Stats:
	- Total Files: `$=dv.pages().length` 
	- Inbox Items: `$=dv.pages('"All/Inbox"').length`
	- Music: `$=dv.pages('"All/Music"').length`
	- Mini-essays: `$=dv.pages('#mini-esssay').length`
	- UX: `$=dv.pages('"All/UX"').length`