# extracellular-matrix

The texts for the [extracellular](https://github.com/exrhizo/extracellular) project

Writings on complexity and human/computer hybrid intelligence.


# Getting started
Install Obsidian, open this folder as a vault.

The plugins are not included in this repo, does this mean an extra step is required?
#### Plugins used
 - Community
	 - Media Extended
	 - Annotator (Obsidian Annotator)
	 - gpt3-notes
		 - I am getting a 429
		 - Go to window>developer>console
			 - app.plugins.plugins['gpt3-notes'].constructor
			 - and then go to the sourcecode and create a breakpoint to test
		- Could use "community-plugin: BRAT" to dev install from repo
			- [see this guide](https://medium.com/@ricraftis/how-to-integrate-chatgpt-into-obsidian-b474a01439e8)


# How this will be read in the ECM app

### Landing pages
Root for each of the urls, e.g. `exrhizo.me`, `fordcorssing.tbd`, `primer.tbd`, ...
They include the Top level menu and links to subpages.

For example `exrhizo.me` has [[exrhizo/Resume]] in the menu, the url for this should be `exrhizo.me/resume` and at the same time, the other folders out to be available. For instance: `exrhizo.me/Spin_Glass_Primer/Phase_Transition` should show [[Spin_Glass_Primer/Phase_Transition]]. All of this will be handled in the vercel router.

### Regular page Export

This is an open question how to parse these,
If Obsidian is easy to use as a library, it can called by a NX executor
if that part of Obsidian is closed source, than create a plugin that creates the export

#### Export Format

The export format will be json, something like this?
```
pages = {
	key: {
		title: 'from the yaml',
		meta: { example: 'the remaining yaml' },
		sections: [
			{
				blocks: [
					"#Markdown",
					"More text"
				]
			}
		]
	},
}
```

As I write, this it will be the biggest question, how to do the data structure. It will be fed into the main app, and will be used to configure the static site.

It will need to support uploading static assets, resolving links and img tags as well as embedding.

The actual strucuture of the pages can be changed as well, to facilitate linking.

Ideally there will be a way to inject parameters into the react components, for instance to have a image float to the left or be inline or be a part of a courasel.

Sections I imagine as a way to add some more structure, where --- is used to designate the seperation of groups of blocks.




# Rough plan for writtings

[Visual inspiration in FIGMA](https://www.figma.com/file/3X8uVvz65oVgjSLKgWZgdd/Share-able?node-id=402%3A2&t=Tv2M8kOj2gsi5QPk-1)

### Ford Crossing LLC
- page for Alex's consultancy
![[00_Static/Temp/sketch-fc-full-length.png|150]]

### Spin Glass Primer
- The core text that could become a book

![[00_Static/Temp/sketch-fc-renormalization-example.png|300]]

### Exhizo
- SEE [exrhizo.me](https://exrhizo.me/)
- [[exrhizo/Home]]
- including playspace, the human factor
- probably a page on [Coordinape](https://docs.google.com/document/d/1v3K4_Q8LWVUxFfwujDv7b8dBTcRoIucnGTVh-_zRS0o/edit)

### The Art Studio
- What is it called?
	- Affectography
	- Sentigraphy
	- Counter Map
- Multiplayer data aggregation?
- A generalized system for multiscale coherence
- Play and games of the great easter sun
- Hybrid / Chimera