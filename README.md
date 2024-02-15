# driving-a-car-app
 #this is a simple python program:

#Car driving program

beginning=print(''' ready to start the engine 
                    Type 'help' for assistance''')


while True:
    command = str(input('>')).lower()
    started = False


  if command == "help":
        print(''' 
type "START" to start the engine
type "STOP" to stop the car
type "Exit" to terminate the game''')

  elif command == 'start':
        if started:
            print('The Car is running')
        else:
            started= True
            print('Car Started')






  elif command == 'stop':
        if not started:
            print('The car did not start')
        else:
            started= False
            print('Car is stopped...')




  elif command == 'quit':
        print('the App is terminated')
        break

  else:
        print("sorry i don't understand")
