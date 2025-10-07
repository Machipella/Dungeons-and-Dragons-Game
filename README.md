# Dungeons-and-Dragons-Game
simple script for my small dungeons and dragons game.
print("Dungeons and Dragons")
while True:     
 print("You are in a Dungeon, do you go right or left?")
 direction= input("Choose right or left: ")
 if direction == "left":
        print("You have fallen into a pit and died. Game Over.")
        break
 elif direction != "left" and direction != "right":
    continue
 elif direction == "right":
        print("You have encountered a Dragon!")
        action = input("Do you want to fight or run? ")
        if action == "fight":
            print("You have defeated the Dragon! You win!")
            break
        elif action == "run":
            print("You have escaped safely. You win!")
            break
        weapons = ["sword", "bow", "magic"]
        print("Choose your weapon: sword, bow, or magic")
        weapon = input("Enter your weapon choice: ")
        if weapon in weapons:
            print(f"You have chosen the {weapon}. You bravely face the Dragon and win!")
            break
        Powers = ["fire", "ice", "lightning"]
        print("Choose your power: fire, ice, or lightning")
        power = input("Enter your power choice: ")
        if power in Powers:
            print(f"You have chosen the {power} power. You use it to defeat the Dragon and win!")
            break
        else:
            print("Invalid choice. The Dragon attacks you while you hesitate. Game Over.")
            break

