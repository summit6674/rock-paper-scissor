# rock-paper-scissor
import random
player = input('choose your move ').lower()
rand_int = random.randint(0,2)
if rand_int == 0:
  computer = 'rock'
elif rand_int == 1:
   computer = 'paper'
else:
  computer = 'scissor'
print('computer played ' + computer)

if player == computer:
  print("it's a tie")
elif player == 'rock':
  if computer == 'paper':
    print('computer wins ')
  elif computer == 'scissor':
    print('you win ')
  elif player != 'paper' or 'scissor':
    print('wrong move')
elif player == 'paper':
  if computer == 'rock':
    print('you wins ')
  elif computer == 'scissor':
    print('computer wins')
  elif player != 'rock' or 'scissor':
    print('wrong move')
elif player == 'scissor':
  if computer == 'rock':
    print('computer wins')
  elif computer == 'paper':
    print('you wins')
  elif player != 'rock' or 'paper':
    print('wrong move')
