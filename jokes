#imported to clear text
import subprocess










        
def joke_app():

    #User reviews CAN BE APPENDED
    reviews = ["It was good!", "Good jokes!"]

    #Joke list
    joke_list = [
    ["Guess what!", "What?", "Chicken butt!" ],
    ["Guess who!", "Who?", "Chicken poo!" ],
    ["Guess why!", "Why?", "Chicken thigh!" ]
    ]




    # Joke generator
    def joke_generator(choice):
        print(joke_list[choice][0])
        print(joke_list[choice][1])
        print(joke_list[choice][2])


    #Asks user if they want to her joke
    descision = input("Do you want to hear a joke? (Yes or No): ")

    #If no then programs quits
    if descision.lower() == "no":
        print("Okay, suit yourself!")

    #if yes starts while loop
    while descision.lower() == "yes":
        joke_number = int(input("Pick a number between 1 and 3: "))
        #Makes use try again if they input number too low or high
        if joke_number < 1:
            print("Not a valid joke number!") 
        elif joke_number > 3:
            print("Not a valid joke number!") 
        elif joke_number == 1: #Depending on number they input it chooses different joke on list
            joke_generator(0)
        elif joke_number == 2:
            joke_generator(1)
        elif joke_number == 3:
            joke_generator(2)
        
        #FUNCTION TO DECIDE IF THEY CHOSE ANOTHER JOKE OR NOT
        def joke_reviewer(decide):
            if decide == 1:
                subprocess.call('reset')
                print("Heres another one coming right up!")
            elif decide == 2:
                review = input("Please write a short review of our app!: ")
                reviews.append(review)
                subprocess.call('reset')
                print("Thank you for using the app!")
                print("These are the current reviews:")
                print(reviews)
                
            
        # MAKES USER CHOOSE BETWEEN ANOTHER JOKE OR FINISHING
        joke_result = input("Do you want to hear another joke or no? Yes or no:  ")
        
        #Calls functiion, yes equaling 1 and no equalling 2
        if joke_result.lower() == "yes":
            joke_reviewer(1)
            continue
        elif joke_result.lower() == "no":
            joke_reviewer(2)
            break

joke_app()