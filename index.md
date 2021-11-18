## Ellie's Programming Portfolio

#Adventure Game
![] (file:///Users/elliejones/Desktop/Screen%20Shot%202021-11-18%20at%203.57.25%20PM.png)

````
public void mouseDialogue()
        {
            textColor(ConsoleColor.Green);
            WriteLine($"Mouse: Hi there! I'm {this.name}. Are you lost? Yes or No?");
            textColor(ConsoleColor.White);
            ans = ReadLine().ToLower();
            Clear();
            textColor(ConsoleColor.Green);
            if (ans.Equals("yes"))
            {
                WriteLine($"{this.name}: Don't worry! I'll help you! Here, take this, it's a snake charmer just in case you need it. That's all I can really do for you though, sorry. Goodbye now!");
                Game.firstPlayer.inventory.Add("Snake Charmer");
            }
            else if (ans.Equals("no"))
            {
                WriteLine($"{this.name}: Oh, okay then. Goodbye!");
                textColor(ConsoleColor.DarkYellow);
                WriteLine("Narrator: The mouse runs away.");
            }
            Game.currentCharacter.hasVisited(true);
        }
````
