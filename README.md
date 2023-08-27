# Blackjack

# 🃏 Game Description:

Welcome to the world of Blackjack! This game follows classic Blackjack rules with a few twists. The goal is to beat the computer by having a hand value as close to 21 as possible without going over. Here's how the game works:

# ⚙️ How the Code Works:

1. The game begins by displaying the Blackjack logo using ASCII art.

2. It follows these house rules:
   - The deck of cards is unlimited in size.
   - There are no jokers.
   - The Jack, Queen, and King all count as 10.
   - The Ace can count as either 11 or 1.

3. A function called `deal_card()` is defined, which returns a random card from the deck. The deck consists of cards with values [11, 2, 3, 4, 5, 6, 7, 8, 9, 10, 10, 10, 10]. Cards are not removed from the deck as they are drawn.

4. Another function, `calculate_score(cards)`, takes a list of cards as input and returns the score. It accounts for Blackjack (a hand with only 2 cards: Ace + 10) and handles the Ace's flexible value.

5. The `compare(user_score, computer_score)` function determines the game outcome, considering possible scenarios like going over 21 (busting), drawing, or achieving a Blackjack.

6. The main game logic is in the `play_game()` function, which:
   - Deals two cards each to the player and the computer.
   - Continues the game loop until it's either the player's turn to draw or the game is over.
   - Prompts the player to draw another card or pass.
   - Lets the computer draw cards until its score is at least 17.
   - Compares final scores and determines the winner.

7. After each game, the player is asked if they want to play again. If they answer 'yes,' the console is cleared, and a new game of Blackjack starts.

# 🔒 Code Specifications:

- The code uses an external module `art` and `clear()` function. These external files are kept private and can be provided upon request.

- The game follows the described house rules, including handling the value of the Ace and checking for Blackjack.

- Players are prompted to continue playing as long as they choose to play again.

- The game provides feedback on the result of each round, including whether the player won, lost, or drew.

- The game loops and allows for multiple rounds until the player decides to quit.

# 📝 Note:

Please note that the external file `art` and `clear()` function are not included in the code posted on GitHub. Users who wish to run this code will need to request access to these separately to ensure the full functionality of the game.
