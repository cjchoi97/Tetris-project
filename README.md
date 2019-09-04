# Tetris
### Background
This is a take on the classic tetris game. It functions as normal with the cascading pieces and the action of lining up pieces to clear lines. However, the colors of the whole board change as each piece is put into place.

### Sample Code
This following set of code is where pygame, which is the game module in python, is initiated. Music is loaded, and the actual tetris board is made using the attributes from the Board class.
```python
class Tetris:
    def __init__(self):
        pygame.init()       #initiate pygame

        pygame.mixer.music.load('tetrisb.mid')
        
        pygame.mixer.music.play(-1, 0.0)
       #pygame.mixer.music.play(loop, start = 0.0)
        
        tetrisBoard = Board()

        screen = pygame.display.set_mode((30*tetrisBoard.COLS,\
                                          30*tetrisBoard.ROWS))
                                            #sets dimensions
                                            #sets display
                #pygame.display.set_mode((width * height))
        
        ctr = 0 #also used to control speed
```

### Technologies
In this project we used tkinter package and pygame module. Pygame was mainly used for event handling and tkinter was mainly used to handle the GUI.
