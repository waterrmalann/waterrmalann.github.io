+++
title = "Conversational Games Bot"
date = 2021-01-19
+++

As a way of spending the large amounts of free time I've been getting lately, I've been playing a lot of conversational games (*like Truth or Dare, Would You Rather, the usual..*) with my friends over Telegram, the chat app. We were collecting the prompts and questions manually from various articles and websites on the internet. Of course, this was a tedious process.

I then realized if I could just add a chat games bot to the group, it would save us all the time and effort of scouring the internet and instead just shoot us prompts and questions so that it's much easier and convenient. Telegram supports official API-supported bot accounts and so there must be bots that do this, I thought..

I then started looking for such bots and of course there was. Although I couldn't find bots that had multiple games, I found bots for Truth or Dare and Would You Rather. Unfortunately though, many of them were either offline, unreliable, or mostly gave us NSFW questions which we did not want.

*sigh*, I decided to screw it and make my own...

#### But before that!

I had to learn how to make a Telegram bot and after some 10 minutes of googling, I came across an API wrapper written in my favourite language called [python-telegram-bot](https://pypi.org/project/python-telegram-bot/) which was perfect because it was so simple I did not even bother reading much of the documentation (*I mean like, who has time for that anyways!*). And just like a true programmer, I CTRL + C and CTRL + V-ed their example starter bot code into my IDE and started writing away.

I tried to find free APIs for the games we usually played and was mostly unlucky. But crawling through various Reddit articles, I finally managed to find undocumented APIs for [either.io](https://either.io) and [Will You Press The Button](https://willyoupressthebutton.com/) which I could take advantage of. For the games I could not find good API solutions for (Truth or Dare, Never Have I Ever, etc..), I decided to make their respective commands read random lines from newline separated .txt files which I later filled with prompts and questions I could find.

#### Thus, the chat games bot was born!

Once I was done with the bot, it featured the following games:

- Truth or Dare
- Would You Rather
- Never Have I Ever
- This or That
- Will You Press The Button

It all worked out perfectly and we started using it a lot. I also realized that some people were discovering my bot and adding it to their groups with the commands having high usage rates, which did put a smile on my face ;)

I then open-sourced the bot on my GitHub. *Links at the bottom.*

#### Bringing it to Discord

Inspired by the success of the Chat Games Bot that I made for Telegram, I wanted to bring it to Discord, which too featured an official bot API and lacked similar bots. I already had plenty of experience with Discord bots so this was a pretty easy task, and most of the code from the Telegram version of the bot was reusable including the text files with the questions and prompts. Once I was done, I decided to put it on a [bot listing](https://top.gg) site.

#### And then it blew up...

I really wasn't expecting much to happen but I could not be any wrong. The bot literally blew up and was added to over 50 guilds (200+ users) in under a week and hit the maximum cap of 100 servers (as I did not verify the bot) within three weeks. It was by then being used by over 800 unique users and the usage rate was through the roof. I obviously wasn't prepared for this kind of growth so it was really surprising but it also made me happy to see so many people using something that I made.

#### The future.

I plan on working on the bots and expanding their question database alongside possibly adding more games like Trivia, Just a minute, and more pretty soon™. Keep an eye on their respective GitHub pages for updates!

The bot is hosted on Discord 24x7 and you can invite it using this [link](https://discord.com/api/oauth2/authorize?client_id=793051926953984000&permissions=280640&scope=bot). For Telegram, you can add [@YetAnotherTruthOrDareBot](http://telegram.me/YetAnotherTruthOrDareBot) to your groups but I would recommend hosting your own instance temporarily because I cannot guarantee 24x7 uptime. It’s actually pretty simple and I’ve provided instructions in the ReadMe file.

#### Source Code

Both versions of the bot are completely open-source, AGPLv3 licensed, and available on my GitHub.

- 🔗 [**Conversational Games Bot | Telegram**](https://github.com/waterrmalann/telegram-conversational-games-bot)
- 🔗 [**Conversational Games Bot | Discord**](https://github.com/waterrmalann/discord-conversational-games-bot)

That’s it about the chat games bot. Thanks for the read!