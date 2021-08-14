---
title: "Surf history dumps - Chess"
layout: post
date: 2021-05-16 22:30
image: /assets/images/6-surf-history-chess/lichess-box-1024.png
headerImage: true
tag:
- surf history
- game
- chess
- reference
star: false # this turns on the highlight on the blog. 
category: blog
author: aman
description: Surf history dump - Chess, engines, databases, etc
excerpt_separator: <!--more-->
toc: false
---

## What?

I picked up Chess(again!). Yeah yeah, I'll fix the formatting for this blog later. This is just another info dump. I read a lot about Chess databases, engines, books and other resources. Just a surf history dump of all of that.

<!--more-->
### Databases

Best, but paid:

* ChessBase 16
* ChessBase Mega Database 2021

Other databases:

* <https://database.lichess.org/>
* Lichess elite database - <https://database.nikonoel.fr/>
I filtered all (standard) games from lichess to only keep games by players rated 2400+ against players rated 2200+, excluding bullet games.

* Caïssabase <http://caissabase.co.uk/>  <- seems like the best free choice (FYI, Caïssa is the goddess of chess)

* TWIC - <https://www.theweekinchess.com/twic> (donate/subscribe when you get rich)

To download PGNs from TWIC:

```seq 1220 1230 | parallel -j10 wget https://www.theweekinchess.com/zips/twic{}g.zip```

Collection to chess games around the internet which you can download for free

<http://www.chessgameslinks.lars-balzer.info/>

...okay, a lot more in chrome bookmarks. Too lazy to paste here.

ScidvsPc is a good pgn/scid viewer. (Installed. run `scid` on terminal)
<https://www.reddit.com/r/chess/comments/tw9as/how_to_use_scid/>
Chessx is another scid viewer. Haven't installed it yet.

Pgnscid is a command line utility (included with Scid) to convert PGN files to si4 databases. It's main advantage over Scid Imports is that it is more reliable for large PGN imports.
> pgnscid myfile.pgn

and a Scid database (consisting of "myfile.si4", "myfile.sg4" and "myfile.sn4") is created, with errors and warnings written to "myfile.err".

To create the database in a different directory, or with a different name, one may add the database name to the command line. For eg:
> pgnscid myfile.pgn mybase

To split large pgn files:
<https://github.com/cyanfish/pgnsplit>

### Engines

Some good engines:

* Stockfish - the most popular one (On lichess, also installed on local)
* LC0 - Neural network based - <https://lczero.org/play/quickstart/>

^ Installed lc0. There are different models/weights available. Of course, for potato PC, 10b and 16b are good enough for my CPU.
<https://lichess.org/blog/X9PUixUAANCqFRSh/introducing-maia-a-human-like-neural-network-chess-engine>

^Installed all these engines in scid vs pc (ubuntu). I've installed Stockfish on _the_ box as well and configured Scid vs PC to ssh into the box and start the engine lol. Quick hack, but that gets me a free remote Stockfish on a beefy server!!

Chess titles: ```GM > IM > FM > CM```

There's also NM - but each country has their own criteria

### Resources

Lichess is superb for studying. Solve puzzles daily. Try to overcome your fear of playing online, bitch.

Lichess also has a learn from your mistakes thingy. Pretty useful.

Always analyze your games and if you don't know how you should have responded, check in the database. Lichess has a good one. I have also downloaded some databases locally. USE THEM!

~~Plan to contribute to Lichess via Fishnet. Have applied for Fishnet Key~~ SUCCESS! Now I'm donating some idle cycles from my box and I'm a patron too! :)

Shoutout to [@lichess](https://lichess.org/). Just 2 words, for completely changing my life - thank you

For long term learning, spaced repetition has proven to be the most effective. chessable.com utilizes a spaced repetition model to help you learn and retain that material. It has several "short and sweet" series for your learning and furthermore has videos that come with some modules. While a time investment, it can rapidly improve your play.

Learning tactics:

Use lichess.org's tactics trainer. If you miss a problem, input it into a self-made chessable book. To do this, create a book, add a line, and, using the dropdown, select load position. Copy and paste the FEN string, and then input the move sequence. Following this, make sure you keep up with your reviews and these should eventually become second nature to you.
<https://chesstempo.com/> has a good trainer

(source for lots of stuff here: <https://www.reddit.com/r/chessbeginners/comments/hd9cma/good_resources_for_new_players_guide/>)

Stop getting into chess drama. I spent my 4 hours reading up about the fat fritz 2 drama, delving into all the articles/videos talking about it. Going down that rabbit hole is not worth your precious time. Another reminder that TIME IS PRECIOUS!

Could have used that time to play some chess, solve some tactics or finish up this blog :P

Regarding openings on r/chess:

* Focus on simple openings
* At a beginner level, there is no need to study opening lines in great depth. Keep it simple with standard, theory-light e4/d4 lines: Italian, Scotch, and Queen's Gambit for white, 1... e5 and QGD for black. Rather than memorizing moves, learn the basic ideas in each opening while adhering to the following general principles:
  * Develop your pieces
  * Control the center
  * Don't move a minor piece twice early
  * Castle your king
  * Connect your rooks
* Avoid theory-heavy openings like the King's Gambit, Sicilian or Grünfeld; entire books have been written on single lines of the Sicilian, and learning the theory behind each move at a beginner level is a huge time sink with very little upside. Also avoid hypermodern openings like the Modern/King's Indian Defence that counter-intuitively cede the center to your opponent, as the resulting structures will be difficult to play as a beginner.

The right way to open a game:
<https://learn.chessbase.com/en/page/the-opening-of-a-game-of-chess>

listudy.org is good for some practice
A couple on QGA/D:

* <https://listudy.org/en/studies/x1ffpt-queens-gambit-declined-from-lichess>
* <https://listudy.org/en/studies/9ufpyr-queens-gambit-declined>

**Keep a mental checklist:**

You should consider the following on every turn, starting with the most forcing move possibilities: What options do I have to give check to the enemy king, and do they accomplish anything? Am I in danger of being checked? Are any of my pieces hanging or underdefended? Are there any tactics in the position? (opportunities to create a fork, pin, skewer, etc. etc.) Can I place any of my pieces in a more active position? Can I occupy or control any outpost squares or open files? Can I blockade an enemy's knight or bishop with a pawn push? As you continue to practice and play, you'll be able to go through this process faster and faster, and with fewer errors.

Some youtube playlists:

* [Chess Fundamentals by IM John Bartholomew](https://www.youtube.com/playlist?list=PLl9uuRYQ-6MBwqkmwT42l1fI7Z0bYuwwO)

* [Gotham Chess Guide](https://www.youtube.com/playlist?list=PLBRObSmbZluRBQOO_6FzyxQUaFyzusSl0) and [10-minute Chess Openings by IM Levy Rozman](https://www.youtube.com/playlist?list=PLBRObSmbZluTpMdP-rUL3bQ5GA8v4dMbT)

* [Beginner to Chess Master by NM ChessNetwork (Jerry)](https://www.youtube.com/playlist?list=PLQsLDm9Rq9bHKEBnElquF8GuWkI1EJ8Zp)

* [Endgame Courses by NM Peter Lalic](https://www.youtube.com/playlist?list=PL70993586E3E01AE7)

* [Jan's Opening Clinic by GM Jan Gustafsson](https://www.youtube.com/playlist?list=PLAwlxGCJB4NeNtW355ibzvWXOhmxfStA9)

* Also a good collection - <https://lichess.org/video>

Good youtube channels to learn from:

* Chessbase India
* Agadmator
* John Bartholomew
* Greg Shahade

check out these channels - kingscrusher, chessnetwork

### Lichess shortcuts

General:

* ? : Show help dialog (analysis mode/studies)
* s : search users
* You can scroll over the board to move in the game.
* Press shift+click or right-click to draw circles and arrows on the board.

In game mode:

* z : Zen mode (hides everything but the board and move list)
* f : Flip board
* /w (in chat) : whisper to spectators (only spectators see this until the game is finished)

In studies:

* d : Comment on this position
* g : Annotate with glyphs

In analysis mode/studies:

* ←/→ (arrow keys on your keyboard) or j/k : Move backward/forward
* ↑/↓ or 0/$ : Go to start/end
* Shift←/Shift→ or Shift J/Shift K: Enter/exit variation
* Shift I : Inline notation
* l : Toggle local computer analysis
* z : Toggle all computer analysis
* a : Computer arrows
* space : Play computer best move
* x : Show threat
* e : Opening/endgame explorer
* f : Flip board
* c : Focus chat
* Esc : Unfocus chat
* Shift C : Show/hide comments
