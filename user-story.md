### as a player, i want solo play mode, so that i can play that game when no one is around
    - Feature Tasks:
        - player can choose what color to play with
        - player can restart the game if wanted
        - player can choose the bot difficulty
    - Acceptance Tests:
        - ensure the color the player choose is correct
        - ensure the game is started when the player choose to restart the game
        - ensure the difficulty the player choose is correct
### as a player, i want multiplayer mode, so that i can play with others
    - Feature Tasks:
        - players can choose to set a timer 
        - players can choose to end the game with a draw or surrender
    - Acceptance Tests:
        - ensure the timer is working when players set it
        - ensure the game is ended when the players end the game
### as a player, i want to see my available moves, so that i can move a piece of mine to attck directly a piece of other player pieces
    - Feature Tasks:
        - player/s can require to highlight all pieces of his/her can move
        - player/s can require to see the highlighted pieces available moves 
    - Acceptance Tests:
        - ensure the highlighted pieces have correct moves and available for each player when they are required
        - ensure the available moves for the highlighted pieces are shown in the screen correctly
### as a player, i want to know what pieces of mine under attack, so that i can move the important piece of them and avoid a direct attack from the other player
    - Feature Tasks:
        - player/s can require to highlight all pieces of his/her under attack
        - player/s can require to see the highlighted pieces moves to escape
    - Acceptance Tests:
        - ensure the highlighted pieces are under attack for each player when they are required
        - ensure the escape moves for the highlighted pieces are shown in the screen correctly
### as a player, i want to see chess pieces moves, so that i can remember what move i can do with a specific piece 
    - Feature Tasks:
        - player/s can require to see the all pieces moves
    - Acceptance Tests:
        - ensure the moves list has correct moves and is shown clear for players when it is required 