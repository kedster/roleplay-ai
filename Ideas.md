[ PLAYER  1 INPUTS TURN] ----------------------------------------------Context is added via form, like charecter creation, Game is initated, and all plays not know the rotation order get a prompt and time to answer, the person who is 
     |                                                                        First gets the shortest prompt, and each submission is context
     | (turns, 1–2 sec input delay ok)
     v
+-----------------------------------+
|  CENTRAL STORY AI (Dungeon Master)|
|  - Updates story context          |-- this should be a Main seperate LLM
|  - Tracks world + characters      |
+-----------------------------------+
     |                               
     | Story continues               
     v
[ STORY UPDATE SENT TO ALL PLAYERS ]
     |
     |  -------------------------------------------------------------------------(Parallel observation)
     |                                                  +----------------------------------+        +---------------------------+
     v                                                  | REFEREE AI (Scoring Moderator)   |------->|   SCORE LOG (hidden)      |
     |                                                  | - Observes interactions          |        |   - creativity points     |
     |                                                  | - Infers implicit behavior       |        |   - teamwork markers      |
     |                                                  +----------------------------------+        +---------------------------+

[ PLAYER  2 INPUTS TURN]-------------------------------------------------------------------------------------------------------------------------------- Context added via charector and repsonce. 
     |
     | (Meta-guidance loop, not per-turn)
     v
+----------------------------------+
| AI MODERATOR                     |
| - Reminds Story AI of past facts |------- This is a Random selected player who can add additional context, but any player can introduce divrgence, the greater the deigence score, the lower the player score and impact i.e. you sabotage the game it detects
|                                  |         sabatoge and gives you a bad score, as if you were traveling none of your team mates would listen to you. the same here ai no longer listens to your impact to the story basd onteh weights of your teammates
| - Nudges long-term arc           |
+----------------------------------+

     |
     | End of 10-min session
     v
+----------------------------------+
| SCORER AI (Wrap-up)              |
| - Processes Referee AI logs      |-- this should be a seperate LLM
| - Outputs summary + player scores|
+----------------------------------+
