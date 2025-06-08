---
banner: "![[flowersjpg.jpg]]"
---
---
banner: "![[flowersjpg.jpg]]"
cssclasses:
  - dashboard
banner_x: "0.5"
banner_y: 1
---
# Choose your journey...

- 📝 Notes
	- Knowledge: `$=dv.pages('"Knowledge"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`
	- Mind: `$=dv.pages('"Mind"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`
	- Drinks: `$=dv.pages('"Teas"').sort(f => f.file.mtime.ts, "desc").limit(1)[0].file.link`
- 📖 Reading
	- [[NEW Man And His Symbols - Carl Jung]]
	- [[Moychay]]
- 🚑 First aid toolkit:
	- [[Reasons to live and not consume rn]]
	- [[Checklist of things to feel happy right now]]
	
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
`$=dv.list(dv.pages('"Inbox"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ✅ TODOs: 
`$=dv.list(dv.pages('"TODOs"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ☕ Brewing:
`$=dv.list(dv.pages('"Projects in progress"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- 🗃️ Oldest file updates: 
	`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"asc").limit(4).file.link)`
- 📊 Stats:
	- Total Files: `$=dv.pages().length` 
	- Inbox Items: `$=dv.pages('"Inbox"').length`
	- Music: `$=dv.pages('"Music"').length`
	- Mini-essays: `$=dv.pages('#mini-esssay').length`
	- UX: `$=dv.pages('"All/UX"').length`