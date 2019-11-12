# MonsterPong
Our entry for [Github GameOff 2018](https://itch.io/jam/game-off-2018)

### How to play
**Arrow keys** to move your paddle, **spacebar** to shoot.

Play a pong match against a monstrous enemy. If and when you defeat it, steal one of its body parts for yourself. Parts affect your statistics, which in turn affect the game as follows:
* **attack** (atk) - the number of balls you shoot
* **defense** (def) - the strength of the bricks behind your paddle
* **health** (hp) - your points

### Credits
The game was developed by Michele 'Buch' Bucelli and Andrea Di Primio. Graphics are licensed under CC-By-SA 3.0 and available on [OpenGameArt](https://opengameart.org/content/monsterpong-assets)

Fun hack: If it’s too challenging to defeat the computer, hack the AI! Removing the following from script.js lines 707-710 will force your opponent to make some monstrously inefficient decisions when it comes to which balls to intercept, giving you the advantage.

// Checks if there are balls attached and finds the nearest incoming ball
for ( var i = 0; i < this.balls.length; ++i ) {
-   if ( this.balls[i].v[1] < 0 && this.balls[i].x[1] < nearestIncomingBall.x[1] )
-      nearestIncomingBall = this.balls[i];
-   if ( this.balls[i].x[1] < nearestBall.x[1] )
-      nearestBall = this.balls[i];

   if ( this.balls[i].bound == 2 && this.t >= 3.5 )
      this.shoot ( 2 );
}

Witch
