# Quiz

print("welcome to quiz")
playing = input("Do you want to play(yes/No)? ")

if playing.lower() != "yes":
    quit()

print("ok let's play")

ll=list()
answer ={ "what is captial of andhra" : "Amaravati",
           "what is national animal" :"Tiger",
           "what is captial of india" :"delhi",
           "what is captial tamilnadu" : "chennai",
           "what is CM of andhra":"PSPK"
}
ll.append(input("1.what is captial of andhra "))
ll.append(input("2.what is national animal "))
ll.append(input("3.what is captial of india "))
ll.append(input("4.what is captial tamilnadu "))
ll.append(input("5.what is CM of andhra "))
ll1= list(answer.values())

score=0
j=0
while j < 5:
    if ll[j].lower() == ll1[j].lower():
        score+=1
    else:
        print("correct answer for {0} question is : {1}".format(j+1,ll1[j]))
    j = j+1
print("{0}/5".format(score))
