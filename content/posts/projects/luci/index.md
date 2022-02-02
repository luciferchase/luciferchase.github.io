---
title: "Luci: The Discord Bot"
subtitle: "A General-Purpose Fun Discord-Bot"
date: 2021-06-02
draft: false

categories: ["projects"]
tags: ["Coding", "Python"]

summary: >-
  A General-Purpose Fun Discord-Bot with lots and lots of features.

featuredImage: avatar.webp
---

{{< admonition type=failure title="Project Abandoned" open=true >}}
Development for this awesome bot had to be stopped due to some personal reasons.

The original library on which this was based [discord.py](https://github.com/Rapptz/discord.py) was scrapped - [The Future of discord.py](https://gist.github.com/Rapptz/4a2f62751b9600a31a0d3c78100287f1), due to lack of support from Discord Devs 😞.
{{< /admonition >}}

# Luci: The Discord Bot

{{< admonition type=abstract title="Luci" open=true >}}
GitHub Repo: [luciferchase/luci](https://github.com/luciferchase/luci)\
A General-Purpose Fun bot with lots and lots of features.
{{< /admonition >}}

# Commands

## Moderation

| Commands                  | What it does?                                             |
| ---------                 | ---------------------------------                         |
| mute                      | Mute someone for a time interval                          |
| unmute                    | Unmute a muted person                                     |
| kick                      | Kick a member out!                                        |
| ban                       | Ban them! Good riddance                                   |
| unban                     | Unban a member                                            |
| bans                      | See list of members who are banned                        |
| baninfo                   | See info about a particular banned member                 |
| addrole                   | Add a role to a member                                    |
| removerole                | Remover a role from a member                              |
| purge             | Purge a member's messages (You can purge your own messages too)   |
| clean                     | Clean your own messages                                   |
| hackban                   | Ban someone who is not in the server                      |
| lock | Lockdown a channel or the server (members will not be able to send any message) |
| unlock                    | Unlock a locked server or channel                         |

## Games

| Commands                  | What it does?                                             |
| ---------                 | ---------------------------------                         |
| aki                       | Play the famous Akinator the game                         |
| tictactoe [alias = ttt]   | Play the classic Tic Tac Toe game against Luci            |
| quiz                      | Play a trivia quiz from over 20 categories                |

## Conversation games

| Commands                  | What it does?                                             |
| ---------                 | ---------------------------------                         |
| truth                     | Ask a truth question. No lie!                             |
| dare                      | Dare someone                                              |
| neverhaveiever [alias = nhie] | Never have I ever...                                  |
| wouldyourather [alias = wyr]  | Would you rather...                                   |

## Fun Commands

| Commands                  | What it does?                                             |
| ---------                 | ---------------------------------                         |
| meme                      | Meme goes brrrrr!                                         |
| memespam                  | So that you don't have to beg for meme 50 times           |
| avatar    [alias = av]    | See the avatar of a user (must be from the same guild)    |
| bigmoji   [alias = e ]    | Enlarge an emoji                                          |
| Comics                    | Get a ohno, Saturday Morning Breakfast Cereal (smbc), The Perry Bible Fellowship (pbf), Cyanide and Happiness (cah), XKCD (xkcd), Mr. Lovenstein (mrls), Chainsawsuit (chainsaw), Sarah's Scribbles (sarah), Dilbert (dilbert), Calvin and Hobbes (calvin), Garfield (garfield), Odd is out (oddones) Commic |
| poll                      | Make a poll                                               |
| nitro [alias = n] | Don't have nitro? Don't worry, send an animated emote through bot |
| insult                    | Evil insult 😈                                            |
| shout                     | Emojify words                                             |
| dm                        | DM someone through the bot (but why would you do that anyway 🤔) |
| alphanato [alias = nda]   | Get military phonetics                                    |
| photo                     | Get a photo from unsplash                                 |
| wallpaper                 | Get today's Bing Wallpaper                                |

## Animals Awwwww :heart:

| Commands                  | What it does?                                             |
| ---------                 | ---------------------------------                         |
| dog                       | Get a cute doggo pic                                      |
| dogfact                   | Get a random fact about dogs                              |
| cat                       | Get a cute catto pic                                      |
| catfact                   | Get a random fact about cats                              |
| panda                     | Get a cute panda pic                                      |
| birb                      | Get a cute bird pic                                       |
| redpanda                  | Get a cute redpanda pic                                   |
| koala                     | Get a cute koala pic                                      |

## Nerd Commands

| Commands                  | What it does?                                             |
| ---------                 | ---------------------------------                         |
| math [alias = calc]       | Handy-dandy calculator (supports very complex stuff too)  |
| integrate                 | Integrate an expression (not fully functional yet 😬)     |
| derive                    | Differentiate an expression                               |
| factorise [alias = solve] | Find roots of a polynomial                                |
| tangent                   | Find tangent to a curve at a point                        |
| definite integrate        | Do definite integration on a curve                        |

The command that I am most proud of, however are these:

## Schedule Memes

You can schedule to send memes (from a particular subreddit; default is r\dankmemes) to a channel hourly/twice a day/daily/whatever. You can schedule the time interval in any way.

## Schedule Wallpaper

Send daily bing wallpapers to a channel.

# TODO

There are lots and lots of things that I want to add to the bot. You can open an Issue and suggest anything that you want me to add and I will try my best.
