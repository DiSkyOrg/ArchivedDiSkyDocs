<p align="center">
	<a href="https://disky.tech/">
		<img src="https://disky.tech/logo.png" alt="Logo" width="100" height="100">
	</a>
	<h3 align="center">DiSky</h3>
	<p align="center">
		Welcome to DiSky's wiki!
		<br/>
		<a href="https://disky.tech/"><strong>Visit official website</strong></a>
		<br/>
		<br/>
		<a href="https://itsthesky.info/">Author</a>
		·
		<a href="https://discord.gg/whWuXwaVwM">Discord</a>
		·
		<a href="https://github.com/SkyCraft78/">Github</a>
	</p>
	<br/>
	<p align="center">
		Here you will see how to use DiSky to connect your server with your discord.<br/>
		A wide wiki will be waiting for you, from the installation of your Discord Bot to many examples from DiSky.<br/>
		If you have any feedback, want to improve, or even create yourself a page on the wiki, feel free to join our Discord!
	</p>
</p>
<details open="open">
	<summary>Table of Contents</summary>
	<ol>
		<li>
			<a href="#about-the-project">About The Project</a>
			<ul>
				<li><a href="#whats-disky-">What's DiSky ?</a></li>
				<li><a href="#difference-between-disky--vixio-">Difference between DiSky & Vixio ?</a></li>
				<li><a href="#3-versions-to-choose">3 versions to Choose</a></li>
			</ul>
		</li>
		<li>
			<a href="#getting-started">Getting Started</a>
			<ul>
				<li><a href="#discord-bot-setup">Discord Bot Setup</a></li>
				<li>
					<a href="#server-bot-setup">Server Bot Setup</a>
					<ul>
						<li><a href="#new-way-v4">New Way</a></li>
						<li><a href="#old-way-38-ark">Old Way</a></li>
					</ul>
				</li>
			</ul>
		</li>
		<li>
			<a href="#basics">Basics</a>
			<ul>
				<li><a href="#why-retrieving-instead-of-getting">Why retrieving instead of getting?</a></li>
				<li><a href="#difference-between-user-and-member">Difference between user and member</a></li>
				<li><a href="#how-bots-are-working-through-disky">How bots are working through DiSky?</a></li>
				<li><a href="#difference-between-deleting--destroying">Difference between deleting & destroying</a></li>
				<li><a href="#how-are-organized-channels">How are organized channels?</a></li>
				<li><a href="#how-works-components-on-discord">How works components on Discord?</a></li>
			</ul>
		</li>
		<li>
			<a href="#features">Features</a>
			<ul>
				<li><a href="#commands">Commands</a></li>
				<li><a href="#embeds">Embeds</a></li>
				<li><a href="#slash-commands">Slash Commands</a></li>
				<li><a href="#webhooks">Webhooks</a></li>
				<li><a href="#react-section">React Section</a></li>
				<li><a href="#audio">Audio</a></li>
				<li><a href="#buttons">Buttons</a></li>
				<li><a href="#dropdowns">Dropdowns</a></li>
				<li><a href="#oauth2">OAuth2</a></li>
			</ul>
		</li>
	</ol>
</details>

---

# About The Project

The new generation of Discord managing via Skript!

### What's DiSky ?

DiSky is a new generation addon, allowing to develop a Discord bot using Skript only. Very little knowledge is required to create advanced features with DiSky. Take for example the interactions or components, which allow to add dynamism to your messages: a few lines of code and it's functional!

### Difference between DiSky & Vixio ?

DiSky is all updated regularly which is unfortunately not the case with Vixio. In addition to the interactions, you can use the components (buttons and dropdown) as well as the audio effects (speed, bast boost, etc...) and many other effects / expressions. Finally, you should know that DiSky ARK uses JDA5, where Vixio is stuck under JDA 4 (JDA is the library used to integrate with Discord). If you want to stay with Vixio, you are free to do so, but it will be a big disadvantage for your server!

### 3 versions to Choose

|                                                         Version 4 Alpha                                                         |                                                        Version 3.0 ARK                                                         |                               Version 2.0                               |
| :-----------------------------------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------: |
|                                  [Github](https://github.com/DiSkyOrg/DiSky "Version 4 Alpha")                                  |                               [Github](https://github.com/SkyCraft78/DiSky3/ "Version 3.0 ARK")                                |      [Github](https://github.com/SkyCraft78/DiSky/ "Version 2.0")       |
| [Download](https://cdn.discordapp.com/attachments/955054375468924979/955158343675162705/DiSky_4.0-alpha7.jar "Version 4 Alpha") | [Download](https://cdn.discordapp.com/attachments/955049142130999347/955144406002974781/DiSky_3.8.0-ARK.jar "Version 3.0 ARK") | [Download](https://github.com/SkyCraft78/DiSky/releases/ "Version 2.0") |
|                                               [Docs](https://disky.tech/v4/docs/)                                               |                                                              Docs                                                              |                                  Docs                                   |
|                                                          Best Version!                                                          |                                                      Updated & Supported!                                                      |                     No longer supported / updated!                      |

---

# Getting Started

Before using DiSky, you **must** have a bot on your developer account. Don't worry, it's free and anyone can do this!

### Discord Bot Setup

- [x] Create application

Go to [Discord Developer Applications](https://discord.com/developers/applications) and click on `New Application` (top-right corner):

![image](https://user-images.githubusercontent.com/101949465/159255003-5af03409-37d9-46bb-82eb-5aa38e3a0c42.png "Image")

A new window will appear. Name your application as you want, since it's not the discord name of your bot, and then click on `Create`:

![image](https://user-images.githubusercontent.com/101949465/159255142-52e9d73b-e249-4d51-a9d4-d24ee5c05410.png "Image")

For that example, I'll call it `DiSky`. On that page, click on the `Bot` tab on the left:

![image](https://user-images.githubusercontent.com/101949465/159255587-c57ed91d-9bac-4a4f-92f0-0f544dce9089.png "Image")

- [x] Create Bot

Click `Add Bot` in the top right and finally `Yes, do it!`:

![image](https://user-images.githubusercontent.com/101949465/159255645-d35f1041-ac64-44c6-a521-9db13e439ba7.png "Image")

You can now also edit your bot's discord name and profile picture. To copy the bot's token, first click the `Reset Token` button and then `Yes, do it!` button.

![image](https://user-images.githubusercontent.com/101949465/159255948-fb28daa5-5276-4006-accc-87f71a131f90.png "Image")

⚠️ **You NEED to activate Gateway intents for the bot to work! Scroll a little downer and activate both lever**:

![image](https://user-images.githubusercontent.com/101949465/159256069-563199f2-bcaa-4d12-b5b1-8c77dca6d7fb.png "Image")

You, don't worry to save your edition by clicking on green `Save Changes` button:

![image](https://user-images.githubusercontent.com/101949465/159256099-66c7b360-82fe-4997-82cc-2ae12865c108.png "Image")

- [x] Invite the Bot

The new discord developer's panel offer a easy solution to generate the invite link of your bot. For that, go to the `OAuth2` tab on the right and then `URL Generator` tab:

![image](https://user-images.githubusercontent.com/101949465/159256312-ec340469-2e58-4b5c-876f-09234e6c1ef0.png "Image")

Now, scroll a little bit and select `Bot` checkbox. But to use the slash commands **DiSky** has provided you, you also need to select the `applications.commands` checkbox.

![image](https://user-images.githubusercontent.com/101949465/159256421-718ebf1d-3449-46d6-af4b-eab8055a616a.png "Image")

Then, after setting your bot's permissions, you can simply `Copy` the link generated below to invite it to any server!

![image](https://user-images.githubusercontent.com/101949465/159256533-c3c5f921-b743-488c-8b38-9451802e030d.png "Image")

**Congratulations! You now have your bot configured and ready to work! You can go to the next step to load it on your server.**

### Server Bot Setup

#### New Way (v4)

```applescript
define new bot named "DiSky":
	token: "ODIxNDYxMjI3Mzg4Nzk3MDU4.YFEDYg.XUgFNCqZoHyGaLt3hEsfXXhoKws"
	intents: default intents
	policy: all
	auto reconnect: true
	compression: none
```

#### Old Way (3.8 ARK)

You now have your bot's token, so you can start by loading your bot on your server. For that, simply copy paste:

```applescript
# You can chooses any other trigger, but I recommend to load your bot only once.
load:
	make new discord bot:
		login to "TOKEN" with name "NAME"
```

For example, I will myself put:

```applescript
load:
	make new discord bot:
		login to "ODIxNDYxMjI3Mzg4Nzk3MDU4.YFEDYg.XUgFNCqZoHyGaLt3hEsfXXhoKws" with name "DiSky"
```

The specified name doesn't matter with the name choosed in the discord developer portal.

⚠️ **Your TOKEN must be PRIVATE! Anyone who have access to it can use your bot for anythings else (like raid)!**

Let's use some code to change the status and the presence of our bot. Don't forget to replace the name DiSky I'm using by your own name you're using in the login effect!

```applescript
load:
	if "DiSky" isn't loaded on discord:
		make new discord bot:
			enable all default intent
			login to "ODIxNDYxMjI3Mzg4Nzk3MDU4.YFEDYg.XUgFNCqZoHyGaLt3hEsfXXhoKws" with name "DiSky"
			set status of bot "DiSky" to online
			set presence of bot "DiSky" to watching "The Beautiful DiSky"
```

That's all, my bot now has a custom status:

![image](https://user-images.githubusercontent.com/101949465/159259586-5e1e54a1-aa4c-41e5-93a6-b231d7c15188.png)

---

# Basics

### Why retrieving instead of getting?

Both methods return the same result, but the way they are doing is completely different;

Every discord entity (except for bots, channels and guilds) cannot be saved permanently, and are therefore cached, which means stored somewhere, to get back them later:

- Getting an entity will search over the cached entities
- Retrieving an entity will both cache the entity, then get it back from cached entities

So if sometimes, when using getting way on some entities, the result is not set, think about retrieving the entity instead!

### Difference between user and member

At the first look, we could say that both are the same thing. Not in Discord!

- An user is a discord user, common to whole Discord and which will hold properties such as name, avatar, etc...
- A member is a user that is in a guild, and have therefore special guild properties such as roles, nickname, etc...

In that way, we can say that a member is a user, but in a specific guild. Therefore, you can have multiple members holding the same user but are in different guilds.

### How bots are working through DiSky?

Bots are the core of DiSky, and without any of them loaded on the server you can't do anything.

They are used to:

- Fire events (member join, message received, etc..)
- Retrieve entities (channels, roles, members, etc...)
- Send messages
- ...

Keep in mind exceptions could occur if you are trying to sue DiSky without any loaded bots!

### Difference between deleting & destroying

Since 3.5.0, DiSky now offers a special effect called `destroy`, which is different than the `delete` effect from Skript.

**Deleting** something will delete the variable itself. In that way, it only works with variables (locals or not) and will clear its content **without** deleting its reference on Discord.

**Destroying** something will delete the entity from Discord but will keep what the entity could return in the variables. In that way, you can also simply delete non-variables expressions (`event-message` for example).

In practical terms, here's an example code with some results of it:

```applescript
# We imagine we are in an event.
# What expression do we have? We can use 'event-message', but need to store its ID for later after destroying the entity.

set {_msg} to event-message
set {_id} to discord id of {_msg}

destroy {_msg} # The message on discord will be deleted, but the variable will not be empty (but unusable)

# Then we can use {_id} which still store the message's ID, as long as the following line is not executed:
delete {_id}
```

### How are organized channels?

You can find below a small mind map on how works channels on Discord:

![image](https://user-images.githubusercontent.com/101949465/159301318-1392fb5b-77f9-4a85-b0aa-3c0d314e075c.png)

And a lot of these are represented in DiSky using the following code name:

- Guild Channel as `channel`
- Voice channel as `voicechannel`
- Text Channel as `textchannel`
- Thread Channel as `thread`
- News Channel as `newschannel`
- Store, stage, message, private and audio channels are not represented as generic types, since they are internal to DiSky.

By this organization, properties can apply to multiple entities at once, for example, sending a message is possible to every messaging channel (including text, thread, news, and store), connecting the bot is possible in every audio channel (voice and stage), etc...

### How works components on Discord?

Discord released a whole new feature for bot, components!

They currently only include **buttons** and **dropdown**, and you can therefore use them with DiSky.

However, this part will only provide an easy way to see components, and will not provide any code (check the right page for that).

Every bot message can only have 5 components row, and one row can be either one dropdown or 5 buttons (= one button row):

![image](https://user-images.githubusercontent.com/101949465/159301538-e1ef7c07-8851-4a10-91ba-69ff01f798f3.png)

So you can have a maximum of 5 dropdowns per message, or 25 buttons, or 2 dropdowns and 15 buttons, etc...

We are talking about the maximum, but a message can simply have just one dropdown, one button, or even no component at all!

In addition, as they are represented as entities by Discord, they have a Unique ID, so it's very easy to make beautiful features using the button or dropdown click events.

---

# Features

### Commands

Before using complex commands, you need to understand how they work.

Every command can have these settings:

- Personal usage (doesn't show any where except with the usage expression) (`usage`)
- Personal description (doesn't show any where except with the description expression) (`description`)
- Personal category (doesn't show any where except with the category expression) (`category`)
- Command's aliases to replace the main command name (`aliases`)
- Command's prefixes to set special chars in front of the command (`prefixes`)
- Executable state, either in guild or in private message (`executable in`)
- List of discord permissions needed to the member in order to execute the command (`permissions`)
- The message sent if the member doesn't have the require permission (`permission message`)
- Roles the command can be used by (`roles`)

For example, a very basic command like a reply one could be:

```applescript
discord command reply <text>:
	prefixes: !
	trigger:
		reply with argument 1
```

The bot will simply reply with the message specified.

However, let's say we only want that command executable in guild, and check if the first argument isn't set.

The result will then be:

```applescript
discord command reply [<text>]:
	prefixes: !
	executable in: guild
	trigger:
		if argument 1 is not set:
			reply with ":x: **You must specify an argument!**"
			stop
		reply with argument 1
```

You can now manage properties of custom type, such as role or member.

As example again, here's a simple "who is" command, using the first argument as the target.

If it's not specified, we simply take the event-user, meaning the member who executed that command:

```applescript
discord command whois [<member=%event-member%>]:
	prefixes: !
	executable in: guild
	trigger:
		make embed:
			set title of embed to "Who is %discord name of arg-1% ?"
			add "`•` Username: %discord name of arg 1%" to {_l::*}
			add "`•` Nick: %discord nickname of arg 1%" to {_l::*}
			add "`•` Tag: %tag of arg 1%" to {_l::*}
			add "`•` Mention: %mention tag of arg 1%" to {_l::*}
			add "`•` Mutual Guild: %size of mutual guild of arg 1%" to {_l::*}
			set description of embed to join {_l::*} with nl
			set thumbnail of embed to avatar of arg-1
			set color of embed to member color of arg-1
			set footer of embed to "Asked by %discord name of event-member%"
			set footer icon of embed to member avatar of event-member
			set timestamp of embed to now
		reply with last embed
```

### Embeds

Discord offers a rich-content sort of message used by bots: embeds!

They can have multiple properties to keep every information you have organized, and you'll see here how to create one, edit it and send it somewhere.

One embed itself is pretty big and can have a lot of values, even if only a title or an author is required to build the embed:

![image](https://user-images.githubusercontent.com/101949465/159285896-640b66e8-e762-4ae2-bbc3-21d1e24ef76a.png)

You can see in the orange line the limits of characters/fields the property can have. If you are going outside these limits, the embed will simply don't build!

However, every first sub-tree of property must has its main property, therefore:

- You cannot set an author icon without an author-name
- You cannot set a footer URL without a footer text
- You cannot set a title URL without a title text

Here are all possible values with the following code, that an embed can have:

```applescript
discord command embed:
	prefixes: !
	trigger:
		make embed:
			set title of embed to "Title"
			set description of embed to "Description%nl%The title leads to the URL, if given"
			set author of the embed to "Author name (Can point to URL)"
			set author icon of embed to "https://cdn.discordapp.com/emojis/825811394963177533.png?v=1"
			set author url of embed to "https://www.youtube.com/watch?v=i33DB6R8YUY"
			set color of the embed to orange
			add inline field named "Field Name" with value "Colour sets %nl%< that" to fields of embed
			add inline field named "Field Name" with value "Color is a java Color%nl%Not a string" to fields of embed
			add inline field named "Field Name" with value "Field value" to fields of embed
			add field named "Non-inline field name" with value "The number of fields that can be shown on the same row is limited to 3, but is limited to 2 when an image is included" to fields of embed
			set image of embed to "https://media.discordapp.net/attachments/237757030708936714/390520880242884608/8xAac.png?width=508&height=522"
			set thumbnail of embed to "https://cdn.discordapp.com/emojis/825811394963177533.png?v=1"
			set title url of embed to "https://www.crunchyroll.com/fr/tonikawa-over-the-moon-for-you"
			set footer of embed to "Footer text"
			set footer icon of embed to "https://cdn.discordapp.com/emojis/825811394963177533.png?v=1"
			set timestamp of embed to now
		reply with last embed
```

![image](https://user-images.githubusercontent.com/101949465/159286287-6d6523ef-34c5-47a4-8903-a7f12ad34679.png)

### Slash Commands

A Slash Command has 3 main properties:

- Name (the command name & the command itself, `/name` for example)
- Description (the command description showed in the UI)
- One (or more) Options (which are required or not)

There are currently 6 types options:

- `STRING` (a text, string, almost anything)
- `INTEGER` (rounded number, so no decimal here)
- `USER` (a guild user)
- `ROLE` (a guild role)
- `BOOLEAN` (only two state, true or false)
- `CHANNEL` (a guild text channel)
- `NUMBER` (a number)

Here's a usage example:

```applescript
slash command ban <user> [<string>] [<boolean>]:
	options:
		1:
			name: target
			description: The target user
		2:
			name: reason
			description: The reason of banning
			default values:
				1:
					name: Spamming
					value: Banned for spamming in channels
				2:
					name: Hacking
					value: Banned for hacking some one / the server (tried)
				3:
					name: Disrespecting
					value: Banned for disrespecting some one or the whole server
				4:
					name: Additional Warns
					value: Banned for multiple warns one after one
				5:
					name: Additional Warns
					value: Banned for multiple warns one after one
		3:
			name: tagged
			description: If the reason sould either show your name or not.
	description: Ban a sepcific user from the guild.
	bots: DiSky
	guilds: 681569058586247218
	trigger:
		retrieve user with id discord id of event-user with event-bot and store it in {_event-member}
		retrieve user with id discord id of arg 1 with event-bot and store it in {_target-member}
		{_event-member} is set
		{_target-member} is set
		if {_event-member} don't have discord permission administrator:
			reply with hidden ":x: **Oh no, you don't have the permission to do that :(**"
			stop
		set {_reason} to arg-2
		if {_reason} is set:
			if arg 3 is true:
				set {_reason} to "%{_reason}% - By %discord name of event-user%"
			ban discord member {_target-member} with reason {_reason}
		else:
			if arg 3 is true:
				ban discord member {_target-member} with reason "Banned by %discord name of event-user%"
			else:
				ban {_target-member}
		reply with hidden ":v: **%mention tag of {_target-member}% has been banned from %discord guild name of event-guild%!**"
```

### Webhooks

The only (current) way to register a webhook is to login with an URL / Token.

A webhook is only for one text channel, if you want it in another channel, the link / token will be different.

Go to the channel settings, into the `Integration` tab.

Click on `Create a Webhook`, in the first elemnt of the list.

The URL / Token can be copied via the `Copy URL` button!

> Don't manage name, avatar, etc ... for now. DiSky offers the way to edit them in the code directly!

Here's a usage example:

```applescript
discord command webhook:
	prefixes: !
	trigger:
		set {_webhookclient} to web hook from url "WEBHOOK_URL"
		set {_webhookbuilder} to new webhook builder
		set webhook avatar of {_webhookbuilder} to member avatar of event-member
		set webhook name of {_webhookbuilder} to "Webhook Name"
		set webhook content of {_webhookbuilder} to "Hello World !"
		make {_webhookclient} send {_webhookbuilder} and store it in {_msg} with bot "DiSky"
		reply with "Sent! `%discord id of {_msg}%`"
```

![image](https://user-images.githubusercontent.com/101949465/159291806-5cfcd4ca-c2ce-4575-80f6-0e20def547c1.png)

### React Section

DiSky offers you a whole new feature, the reaction section !

It works as a normal section, but the code inside it will be executed when someone reacts to the specified emote.

It work same as `add reaction` effect, but allow you to execute code.

You need first to make the section code:

```applescript
on message receive:
	# We check if the event-user is a bot or not
	event-user is not a discord bot
	# Here we manage the section.
	# Specify the reaction (here "x", mean the red cross) and the message
	react to event-message with reaction "x"
```

Then, we have to make the section itself, for example delete the message:

> ⚠️ Event value inside the reaction section are refering to values of the reaction add event!

```applescript
on message receive:
	# We check if the event-user is a bot or not
	event-user is not a discord bot
	# Here we manage the section.
	# Specify the reaction (here "x", mean the red cross) and the message
	react to event-message with reaction "x" to run:
		# We delete the message sent by a bot
		destroy event-message
```

And here you go! Any message sent by your bot will receive a ❌ reaction, and the message will be deleted if anyone reacts to this!

> 📗 NEW: You can now use cancel event to cancel the reaction add event inside a section!

Here's a usage example:

```applescript
discord command react [<text>] <boolean>:
	prefixes: !
	trigger:
		if arg 2 is true:
			react to event-message with emote (reaction arg-1) to run one time:
				reply with "**You reacted %mention tag of event-user%!**, but now you can't anymore :)"
		else:
			react to event-message with emote (reaction arg-1) to run:
				reply with "**You reacted %mention tag of event-user%!**"
```

![image](https://user-images.githubusercontent.com/101949465/159296123-6b4f9ecf-98b2-424e-ab5c-d880e317239a.png)

### Audio

DiSky offers you the way to manage your bot's audio handler.

Here, you'll see how to make the bot play a youtube track, search it if needed, handle error and apply audio effect such as speed, pitch or depth.

Here's a usage example:

```applescript
discord command play [<string>]:
	prefixes: *
	aliases: p
	trigger:
		if arg 1 is not set:
			reply with ":x: **You __must__ specify an URL or a YouTube input!**"
			stop
		if voice channel of event-member is not set:
			reply with ":x: **You __must__ be in a voice channel in order to join you!**"
			stop
		# Check if the event member who made the command is in the voice channel of the bot.
		set {_bot} to self member of event-bot in event-guild
		set {_force} to false
		if voice channel of {_bot} is set:
			discord id of voice channel of event-member is not discord id of voice channel of {_bot}
			reply with ":x: **Error, I'm already connected to another voice channel.**"
			stop
		connect event-bot to (voice channel of event-member)
		search in youtube for arg-1 and store it in {_r::*}
		# It mean it's a playlist and not a single track
		if arg-1 contain "list=":
			if {_r::*} is not set:
				reply with ":x: **Can't found that playlist!**"
				stop
			# We play all tracks listed on the playlist inputted
			play {_r::*} in event-guild
			make embed:
				set author of embed to "Successfully added **%size of {_r::*}% tracks** to your queue!"
				set author icon of embed to avatar of event-member
				set color of embed to orange
				set author url of embed to arg-1
			reply with last embed
		else:
			if {_r::1} is not set:
				reply with ":x: **Can't found anything for the input '%arg-1%'!**"
				stop
			play {_r::1} in event-guild
			set {_track} to {_r::1}
			make embed:
				set title of embed to "%{_track}%"
				set title url of embed to track url of {_track}
				set color of embed to lime
				set footer of embed to "Executed by %discord name of event-member%"
				set thumbnail of embed to track thumbnail of {_track}
				add "`•` Duration: %track duration of {_track}%" to {_l::*}
				add "`•` Author: %track author of {_track}%" to {_l::*}
				set description of embed to join {_l::*} with nl
			reply with last embed
```

DiSky offers you to manage some audio effect, currently three are supported:

- Speed
- Pitch
- Depth

Each of these have default value, maximum and minimum ones:

> ⚠️ I'm considering you know chat you are doing! DiSky will throw an internal error if you don't respect / check value when you change effect!

| **Effect** | **Minimum** | **Maximum** | **Default** |
| ---------- | ----------- | ----------- | ----------- |
| `Speed`    | 0.1         | 2.0         | 1.0         |
| `Pitch`    | 0.1         | 2.0         | 1.0         |
| `Depth`    | 0.1         | 0.9         | 0.1         |

The speed changes, of course, the speed of the track and the pitch changes his intensity.

The depth is a special audio effect, making wave with the bass and the music itself.

### Buttons

For a few weeks now, Discord has been deploying a new interaction system: buttons! They can be used on a post (maximum 5 / message) and do actions when clicked. They will surely replace the reaction menu, removing the rate limit that had the latter;

As you can guess, DiSky offers the possibility to create buttons, add them to messages and, using the event or sections, execute code on the click. That's what we will see on this page!

First of all, we need to look at the button itself. They have a fixed color, the button cannot have a custom color. They also have two different states:

- If they are enabled or disabled
- If they are link buttons (a link icon will appear)

Here is a small summary of the possible button formats:

![image](https://user-images.githubusercontent.com/101949465/159294185-0637b173-5a67-4e3f-84e6-622d0a862af7.png)

Here's a usage example:

```applescript
discord command buttons:
	prefixes: !
	trigger:
		set {_row} to new buttons row
		set {_row2} to new buttons row
		set {_row3} to new buttons row
		add new link button with url "http://itsthesky.info/" with style success with content "Gray Link Button" with emoji "star" to buttons of {_row}
		add new button with url "a" with style primary with content "Blue Default Button" with emoji "joy" to buttons of {_row2}
		add new button with url "b" with style secondary with content "Gray Default Button" with emoji "joy" to buttons of {_row2}
		add new button with url "c" with style danger with content "Red Default Button" with emoji "joy" to buttons of {_row2}
		add new button with url "d" with style success with content "Green Default Button" with emoji "joy" to buttons of {_row2}
		add new disabled button with url "e" with style primary with content "Blue Disabled Button" with emoji "sparkles" to buttons of {_row3}
		add new disabled button with url "f" with style secondary with content "Gray Disabled Button" with emoji "sparkles" to buttons of {_row3}
		add new disabled button with url "g" with style danger with content "Red Disabled Button" with emoji "sparkles" to buttons of {_row3}
		add new disabled button with url "h" with style success with content "Green Disabled Button" with emoji "sparkles" to buttons of {_row3}
		reply with "Buttons" with rows {_row} and {_row2} and {_row3}
```

![image](https://user-images.githubusercontent.com/101949465/159294737-ae7e9686-52f7-471e-972d-b7e7d808ad09.png)

### Dropdowns

Here's a usage example:

```applescript
discord command dropdown:
	prefixes: !
	trigger:
		make new dropdown with id "dropdownid":
			set min range of dropdown to 1
			set max range of dropdown to 3
			add new choice with value "test" with name "Name" with desc "Description" with reaction "art" to choices of dropdown
			add new choice with value "test1" with name "Name1" with desc "Description1" with reaction "joy" to choices of dropdown
			add new choice with value "test2" with name "Name2" with desc "Description2" with reaction "star" to choices of dropdown
			add new choice with value "test3" with name "Name3" with desc "Description3" with reaction "sparkles" to choices of dropdown
			add new choice with value "test4" with name "Name4" with desc "Description4" with reaction "white_check_mark" to choices of dropdown
		send "Dropdown" to event-channel with components last dropdown
```

![image](https://user-images.githubusercontent.com/101949465/159298408-c9220a66-b512-42f1-8e04-7c08074db26c.png)

### OAuth2

**⚠️ Warning:**

Keep in mind that OAuth2 is a pretty complex feature and is not good for newcomers!

This page will show everything that is currently possible with DiSky, without explaining basic functionalities!

Discord's OAuth2 is here to retrieve personal information about a specific user with its permission.

For that you'll need several features to work with DiSky's OAuth2 system:

- Bot's application (when creating a discord bot, you create first its application)
- Opened port on your machine (To handle user's response)
- Bot linked to its application

Here's basically how DiSky will do for the OAuth2 system:

1. Create a new OAuth2 system with Skript with Client ID & Client Secret, setting custom redirect domains & the scopes we want
2. Build its authorization URL and send it to the user
3. Wait for the user to click the link and accept the authorization
4. Get back the code that Discord send us through the redirection (redirection URL is `http://<CONFIGURED DOMAIN>:<CONFIGURED PORT>/oauth/`)
5. Exchange the code with Discord for real information asked according to the enabled scopes (identity, guilds, connections, etc...)

Let's introduce the real DiSky code for what the previous part explained:

```applescript
# We create a new OAuth2 system, the specified bot MUST have an application node, see above for more info.
set {_b} to create a new oauth system with event-bot

# Change the scopes (= what we will ask the user to share) between guilds, identity, email, connections, etc...
set scopes of {_b} to "identify" and "guilds" # Ask for user's info itself (mail, id, name, tag, etc..) and user's guilds

# The domain used for this builder.
# IT WILL BE REGISTERED AS 'DOMAIN:PORT/oauth/'!
# The domain must point to your machine, or you can also input the machine's digital IP.
# The port is unique and is 3650 by default! You can however change it in the 'auth.yml' in diSky folder.
set domain of {_b} to "disky.tech" # https://disky.tech:3650/oauth/ will be used for redirection

# The authorization URL can now be built and the user can whenever he wants login through it.
reply with "Click here to log in: %nl%<%build oauth {_b}%>" and store it in {msg}

# Fired when the user has sent a request to the related website back.
# Discord redirects the suer to the custom DiSky's server with a code, then DiSky will exchange this code for a valid Token.
# The token will be sued to get information about the user according to the enabled scopes.
when auth {_b} receive a response:
	# Event-user represents the LOGGED user, and not always the user who typed the command.
	edit {msg} to show "Logged as: %event-user%%nl%Guilds number: %size of event-guilds%"
```

Okay, you did the hardest part of OAuth2, good job!

You just have to register the redirect URL to the discord developer portal, else Discord will show an `Invalid OAuth2 REdirect URL` error:

1. Go to your bot's settings, click on OAuth then General on the right.
2. Click on Add Another from Redirects part, and add the formatted URL, so `http://DOMAIN:PORT/oauth/`
3. Don't forget to save!

**Changing redirect's page & Port**

DiSky handles both error & valid code pages on the webserver.

If you wanna change the simple `Login success` message on redirect, just edit the `valid.html` file in DiSky's folder.

Same for errors (null or invalid code), the file is called `error.html`

For the port, change the number at node `Port` in the `oauth.yml` file of DiSky's folder.

And tada 🎉 Your bot now supports OAuth2 and you'll be able to get users' personal information!
