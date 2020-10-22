print("Encouragement bot thingy")
print()
while True:
  description = input("Could you describe how you feel in one word?  ")

  list_of_words = description.split()

  feelings_list = []
  encouragement_list = []
  counter = 0
  
  for each_word in list_of_words:
    
    if each_word == "sad":
      feelings_list.append("sad")
      encouragement_list.append("there is a small chance that tomorrow will be a better day")
      counter += 1
    if each_word == "happy":
      feelings_list.append("happy")
      encouragement_list.append("hapiness is temporary")
      counter += 1
    if each_word == "tired":
      feelings_list.append("tired")
      encouragement_list.append("go and sleep")
      counter += 1
    if each_word == "useless":
      feelings_list.append("useless")
      encouragement_list.append("you are more useful than annoying ads that companies spend thousands on")
      counter += 1
    if each_word == "shitty":
      feelings_list.append("shitty")
      encouragement_list.append("we all feel like shit")
      counter += 1
    if each_word == "stressed":
      feelings_list.append("stressed")
      encouragement_list.append("if you are stressed, then too bad for you")
      counter += 1
    if each_word == "great":
      feelings_list.append("great")
      encouragement_list.append("you will still die, someday")
      counter += 1
    if each_word == "good":
      feelings_list.append("good")
      encouragement_list.append("there are millions of children dying of starvation in Africa")
      counter += 1
    if each_word == "terrible":
      feelings_list.append("terrible")
      encouragement_list.append("the millions of children dying of starvation in Africa are feeling more terrible than you")
      counter += 1
    if each_word == "genocide":
      feelings_list.append("like starting a genocide")
      encouragement_list.append("people generally don't like that")
      counter += 1
    if each_word == "crappy":
      feelings_list.append("crappy")
      encouragement_list.append("your country has a sewerage system, so use it")
      counter += 1


  if counter == 0:
    
      output = "Sorry I don't really understand. Please use different words?"

  elif counter == 1:
    
      output = "It seems that you are feeling quite " + feelings_list[0] + ". However, do remember that "+ encouragement_list[0] + "! Hope you feel better :)"  

  else:

    feelings = ""    
    for i in range(len(feelings_list)-1):
      feelings += feelings_list[i] + ", "
    feelings += "and " + feelings_list[-1]
    
    encouragement = ""    
    for j in range(len(encouragement_list)-1):
      encouragement += encouragement_list[i] + ", "
    encouragement += "and " + encouragement_list[-1]

    output = "It seems that you are feeling quite " + feelings + ". Please always remember "+ encouragement + "! Hope you feel better :)"

  print()
  print(output)
  print()
