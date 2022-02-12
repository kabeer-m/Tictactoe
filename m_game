game = [["   ","   ","   "],    # The main screen of the game
       ["   ","   ","   "],
       ["   ","   ","   "]]

print("type -end- at any turn to end the game")

print()                         # empty line space

def check():                    # Function for checking if user input is valid
    while True:                                 
            global X
            X = input("enter row: ")
            if X == "end":
                c== 0
                away()
                break
            if X.isdigit == False:
                print("invalid input - please try again")
                continue
            elif X.isdecimal() == False:
                print("invalid input - please try again")
                continue
            global Y
            Y = input("enter column : ")
            print()
            if Y.isdigit() == False:
                print("invalid input - please try again")
                continue
            elif X.isdecimal() == False:
                print("invalid input - please try again")
                continue
            
            X = int(X)          # converting string values to integers
            Y = int(Y)          # cus default input is string
            
            if X > 3 or X < 1 or Y > 3 or Y < 1 :  # checks if int input valid
                print("input out of bounds - please try again")  
                continue
            elif game[X-1][Y-1] == " X " or game[X-1][Y-1] == " O ":
                print("Spot taken - please try again")
                continue
            else:
                break

           
def screen():                   # printing each row of screen in seperate lines
        print(game[0])
        print(game[1])
        print(game[2])

screen()                        # Print scrren for the first time


def away():                     # exit function
            x = input("again? Y/N")
            print()
            print("-------RESTART------")
            print()
            if x == "y"  or x == "Y":       # game reset
                        global game
                        game.clear()
                        game = [["   ","   ","   "],
                                ["   ","   ","   "],
                                ["   ","   ","   "]]
                        screen()
                        print()
                        main_game()
            else :
                exit()

 

def main_game():                # function containing the game
    global c                      
    c= 0                        # value which counts each loop ie : turn
    while True :
    
        if c == 9 :             # on ninth turn, asks if reset or end
            print("-------DRAW-------")
            c== 0
            away()
        
    
        elif c%2 == 0:          # even loops == X's turn
            print("X turn")
            print()
            
            check()
                
            game[X-1][Y-1] = " X "
            
            screen()
            print()
    
            if game[0][0] == game[1][0] == game[2][0] == " X " or game[0][1] == game[1][1] == game[2][1] == " X " or game[0][2] == game[1][2] == game[2][2] == " X ":
                print("X WON!!!!!!")
                away()
                
            elif  game[0][0] == game[0][1] == game[0][2] == " X " or game[1][0] == game[1][1] == game[1][2] == " X " or game[2][0] == game[2][1] == game[2][2] == " X ":
                print("X WON!!!!!!")
                away()
                
            elif game[0][0] == game[1][1] == game[2][2] == " X " or game[0][2] == game[1][1] == game[2][0] == " X ":
                print("X WON!!!!!!")
                away()
                
            
            else:
                c += 1           # adding 1 to "c"
                continue
    
    
        elif c%2 != 0 :          # odd loops == O's turns
            print("O turn")
            print()
    
            check()
                
            game[X-1][Y-1] = " O "
            screen()
            print()
    
            if game[0][0] == game[1][0] == game[2][0] == " O " or game[0][1] == game[1][1] == game[2][1] == " O " or game[0][2] == game[1][2] == game[2][2] == " O ":
                print("O WON!!!!!!")
                away()
                
            elif  game[0][0] == game[0][1] == game[0][2] == " O " or game[1][0] == game[1][1] == game[1][2] == " O " or game[2][0] == game[2][1] == game[2][2] == " O ":
                print("O WON!!!!!!")
                away()
                
            elif game[0][0] == game[1][1] == game[2][2] == " O " or game[0][2] == game[1][1] == game[2][0] == " O ":
                print("O WON!!!!!!")
                away()
                
            
            else :
                c += 1        # adding 1 to "c"
                continue

main_game()                   # summons main game
