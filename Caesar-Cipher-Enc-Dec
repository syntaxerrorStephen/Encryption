def encrypt(text,s):
    result = ""
 
    # traverse text
    for i in range(len(text)):
        char = text[i]
 
        # Encrypt uppercase characters
        if (char.isupper()):
            result += chr((ord(char) + s-65) % 26 + 65)
 
        # Encrypt lowercase characters
        else:
            result += chr((ord(char) + s - 97) % 26 + 97)
 
    return result

def decrypt():
  letters = "abcdefghijklmnopqrstuvwxyz"
  enc_string = input("Enter encrypted string:  ")
  x = 0
  while x < 26:
      x = x + 1 
      stringtodecrypt=enc_string
      stringtodecrypt=stringtodecrypt.lower()
      ciphershift=int(x)
      stringdecrypted=""
      for character in stringtodecrypt:
          position = letters.find(character)
          newposition = position-ciphershift
          if character in letters:
              stringdecrypted = stringdecrypted + letters[newposition]
          else:
              stringdecrypted = stringdecrypted + character
              
      ciphershift=str(ciphershift)
      print("You used a cipher shift of "+ciphershift)
      print("Your decrypted message reads:")
      print(stringdecrypted)
      print("\n")

usrChoice = input("Do you want to encrypt or decrypt?:  ")

if usrChoice == "Encrypt":
  #check the above function
  text = input("What do you want to encrypt?: ")
  s = 16
  print ("Text  : " + text)
  print ("Shift : " + str(s))
  print ("Cipher: " + encrypt(text,s))
  
elif usrChoice == "Decrypt":
  decrypt()

else:
  exit()
