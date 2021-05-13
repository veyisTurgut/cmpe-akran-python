### Terminale ya da başlat menüsüne "idle" yazarak Python terminali açalım.

<details> <summary> MATH</summary>

- ADDITION & SUBTRACTION & MULTIPLICATION
     ```
     >>> 15 + 4
     19
     >>> 15 - 4
     11
     >>> 15 * 4
     60  
     >>> 3.2 + 2
     5.2   
     >>> 3.2 - 3.2 
     0.0
     >>> 3.2 * 5
     16.0
     ```
 
 - FLOAT DIVISION vs INTEGER DIVISION
     ```
     >>> 15 / 4
     3.75
     >>> 15 // 4
     3
     ```

- POWER & REMAINDER
     ```
     >>> 2 ** 3
     8
     >>> 15 % 7
     1
     ```

- math LIBRARY
   ```
   >>> import math
   >>> math.floor(8.4)
   8
   >>> math.ceil(7.1)
   8
   >>> math.round(7.6)
   8
   >>> math.pi
   3.141592653589793
   >>> math.e
   2.718281828459045
   >>> math.inf
   inf
   >>> math.fabs(-5)
   5
   >>> math.sqrt(25)
   5.0
   >>> math.sin(math.pi/2)
   1.0
   >>> math.log(10)
   2.302585092994046
   >>> math.log(100,10)
   2.0
   >>> math.gcd(8,12)
   4
   >>> math.comb(5,2)
   10
   >>> math.pow(2,3)
   8.0
   ```
</details>

<details> <summary> STRINGS</summary>
  
 - CONCATENATION
   ```
   >>> "hello world"
   'hello world'
   >>> "hello" + " world"
   'hello world'
   >>> "hello" * 2 
   'hellohello'
   ```
 - ESCAPE CHARACTER 
   ```
   >>> "hello \"Ali\""
   'hello "Ali"'
   >>> """hello
   world
   in
   multiple lines"""
   'hello\nworld\nin\nmultiple lines'
   ```
 - FORMATTING
   ```
   >>> "hello {}".format("world")
   'hello world'
   >>> "Hesap {} TL.".format("2")
   'Hesap 2 TL.'
   ```
 - INDEXING 
   ```
   >>> "helloo"[0]
   'h'
   >>> "helloo"[2]
   'l'
   >>> "helloo"[-1]
   'o'
   >>> "helloo"[1:3]
   'el'
   >>> "helloo"[:-2]
   'hell'
   >>> "helloo"[1:]
   'elloo'
   ```
- METHODS 
   ```
   >>> "hello world".upper()
   'HELLO WORLD'
   >>> "HELLO world".lower()
   'hello world'
   >>> "hello world".title()
   'Hello World'
   >>> "hello world".find("lo")
   3
   >>> "hello world".count("o")
   2
   >>> "helLO world".islower()
   False
   >>> "hello world".replace("hello","byebye")
   `'byebye world'
   ```
</details>

<details> <summary> VARIABLES</summary>

  - DECLARATION
    ```
    >>> x = 5
    >>> y = 4.3
    >>> z = "hello"
    >>> Y = 8
    >>> a, b = 5, 6
    >>> a, b = b, a+b
    ```
  - TYPE()
    ```
    >>> type(x)
    <class 'int'>
    >>> type(y)
    <class 'float'>
    >>> type(z)
    <class 'str'>
    >>> type(Y)
    <class 'int'>
    >>> type(True)
    <class 'bool'>
    >>> type(False)
    <class 'bool'>
    ```
  - CASTING
    ```
    >>> int(2.6)
    2
    >>> float(2)
    2.0
    >>> str(2.6)
    '2.6'
    >>> str(2)
    '2'
    >>> int(False)
    0
    >>> bool(2)
    True
    >>> int(y)
    4
    ```
</details>

<details> <summary>  INPUT()</summary>

   ```
   >>> input()
   2
   '2'
   >>> int(input())
   2
   2
   >>> float(input("Please enter a number: "))
   Please enter a number: 3.14
   3.14
   ```
</details>

<details> <summary>  PRINT()</summary>
     
   ```
   >>> print()
   
   >>> print(5)
   5
   >>> print(3+7.2)
   10.2
   >>> print("hello")
   'hello'
   >>> print("hello" + " world")
   'hello world'
   >>> print(x)
   5
   >>> print(x * y)
   21.5
   >>> print(x, y, "hello")
   5 8 hello
   >>> print(x, y, "hello", sep="xx")
   5xx8xxhello
   ```
</details>

<details> <summary> COMPARISON and BOOLEANS </summary>
  
    ```
    >>> 9 > 2
    True
    >>> 9 >= 9.0
    True
    >>> 9 < 2
    False
    >>> 9 <= 2
    False
    >>> 9 == 2
    False
    >>> 9 != 9.0
    False
    >>> 3*5 == 15
    True
    ```
  
</details>

<details> <summary> LISTS  </summary>
  <br> "Python knows a number of compound data types, used to group together other values. The most versatile is the list, which can be written as a list of comma-separated values (items) between square brackets. Lists might contain items of different types, but usually the items all have the same type."[1]
  
  <br> **This part is completely taken from https://docs.python.org/3/tutorial/introduction.html#lists**<br>
  
  ```
  >>> squares = [1, 4, 9, 16, 25]
  >>> squares
  [1, 4, 9, 16, 25]
  ```
  
  ```
  >>> squares[0]  # indexing returns the item
  1
  >>> squares[-1]
  25
  >>> squares[-3:]  # slicing returns a new list
  [9, 16, 25]
  >>> squares[:]
  [1, 4, 9, 16, 25]
  ```
  
  ```
  >>> squares + [36, 49, 64, 81, 100]
  [1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
  ```
  
  ```
  >>> cubes = [1, 8, 27, 65, 125]  # something's wrong here
  >>> 4 ** 3  # the cube of 4 is 64, not 65!
  64
  >>> cubes[3] = 64  # replace the wrong value 
  >>> cubes
  [1, 8, 27, 64, 125]
  ```
  
  ```
  >>> cubes.append(216)  # add the cube of 6
  >>> cubes.append(7 ** 3)  # and the cube of 7
  >>> cubes
  [1, 8, 27, 64, 125, 216, 343]
  ```
  
  ```
  >>> letters = ['a', 'b', 'c', 'd', 'e', 'f', 'g']
  >>> letters
  ['a', 'b', 'c', 'd', 'e', 'f', 'g']
  >>> # replace some values
  >>> letters[2:5] = ['C', 'D', 'E']
  >>> letters
  ['a', 'b', 'C', 'D', 'E', 'f', 'g']
  >>> # now remove them
  >>> letters[2:5] = []
  >>> letters
  ['a', 'b', 'f', 'g']
  >>> # clear the list by replacing all the elements with an empty list
  >>> letters[:] = []
  >>> letters
  []
  ```
  
  ```
  >>> letters = ['a', 'b', 'c', 'd']
  >>> len(letters)
  4 
  ```
  
  ```
  >>> a = ['a', 'b', 'c']
  >>> n = [1, 2, 3]
  >>> x = [a, n]
  >>> x
  [['a', 'b', 'c'], [1, 2, 3]]
  >>> x[0]
  ['a', 'b', 'c']
  >>> x[0][1]
  'b'
  ```
</details>

### Şimdi Pycharm'a geçelim.

<details> <summary> IF and INDENTATION </summary>
    
  There can be zero or more elif parts, and the else part is optional. The keyword ‘elif’ is short for ‘else if’.
  
  ```python
  num = int(input("Enter a number:\n"))
  if num < 0:
    print("You entered a negative number")
  elif num == 0:
    print("You entered zero")
  else:
    print("You entered a positive number")
  ```
  ```python
  num = int(input("Enter a number:\n"))
  if num >= 85:
    print(5)
  elif num >= 70:
    print(4)
  elif num >= 60:
    print(3)
  elif num >= 50:
    print(2)
  else:
    print(1)
  ```
  ```python
  num1 = int(input("Enter a number:\n"))
  num2 = int(input("Enter anoher number:\n"))
  if num1 == num2:
    print("you entered equal numbers")
  else:
    if num1 > num2:
        print("first number was greater")
    else:
        print("second number was greater")
  ```
</details>
  
<details> <summary> LOOPS</summary>
    <br>
  In computer science, a loop is a programming structure that repeats a sequence of instructions until a specific condition is met. 
    
  - ### WHILE LOOP
    <br> The while statement is used for repeated execution as long as an expression is true.
    ```python
    i = 1
    while i < 6:
      print(i)
      i += 1
    ```
    ```python
    import time

    timer = 10
    while timer != 0:
        print(f"bomb will explode in {timer}")
        timer = timer - 1
        time.sleep(1) # sleep 1 seconds
    print("BOOOOM!!")
    ```
    ```python
    num = int(input("Enter numbers to add or type 0 to exit: "))
    sum = num
    while num != 0:
        num = int(input(f"Sum is {sum}. Enter another number or type 0 to exit: "))
        sum += num
    print(f"Sum is: {sum}")
    ```
    ```python
    text = input("Type something and I'll find the number of words in it!\n")
    index = 0
    number_of_words = 0
    while index < len(text):
        if text[index] == " ":
            number_of_words += 1
        index += 1
    print(f"There are {number_of_words + 1} words in \"{text}\".")
    ```

  - ### FOR LOOP
    <br> A For Loop is used to repeat a specific block of code a "known" number of times. 
  
    ```python
    fruits = ["apple", "banana", "cherry"]
    for x in fruits:
     print(x)
    ```
    ```python
    for x in "banana":
     print(x)
    ```
    ```python
    # Measure some strings:
    words = ['cat', 'window', 'defenestrate']
    for w in words:
       print(w, len(w))
    ```
    ```python
    for i in range(5):
       print("*"*i)
    ```
    ```python
    for i in range(5):
       for j in range(i):
            print(j*i,end=" ")
       print()
    ```
  - ##### RANGE()
    If you do need to iterate over a sequence of numbers, the built-in function range() comes in handy. It generates arithmetic progressions:
    ```
    >>> list(range(0, 30, 5))
    [0, 5, 10, 15, 20, 25]
    >>> r = range(0, 20, 2)
    >>> r
    range(0, 20, 2)
    ```
    ```python
    my_list = ['pop', 'rock', [10], 5.2, -3,  'jazz']
    for i in range(len(my_list)):
        if type(my_list[i]) == str:
            print(my_list[i][:-1])
        elif type(my_list[i]) == int:
            print(my_list[i]**2)
    ```
  - ##### BREAK
    Break out a for loop.
    ```python
    for i in range(9):
    if i > 3:
      break
    print(i)
    ```
  - ##### CONTINUE
    Skip the iteration, but continue with the next iteration.
    ```python
    for i in range(9):
    if i == 3:
      continue
    print(i)
    ```
</details>


<details> <summary> TUPLES and SET and DICT </summary>
  
  
  
</details>

<details> <summary> EXERCISES </summary>
  
  * find factorial <br/> 
    ```python
    number = int(input("Enter a number!\n"))
    ## edge cases are important
    if number < 0:  # number is negative
        print("Number must be positive!")
    elif number == 0 or number == 1:    # number is 0 or 1
        print(number)
    else: # number is positive
        factorial = 1
        for i in range(1, number + 1):  # multiply every number starting from 1 to "number"
            factorial = factorial * i
    print(factorial)
    ```
  * check armstrong number<br/> 
    ```python
    #armstong number: A number that is equal to the sum of cubes of its digits.
    number = int(input("Enter a number!\n"))
    sum = 0                   # we are gonna add the cubes of digits to this variable
    temp = number             # temporary variable to play with so that we wont forget the value of "number"
    while temp > 0 :          # while temp is greater than 0, do these
        digit = temp % 10     # last digit of the variable
        sum = sum + digit**3  # add cube of the digit to cumulative sum
        temp = temp // 10

    if sum == number:
        print("Yes, {} is an Armstrong number!".format(number))
    else:
        print("No, {} is not an Armstrong number".format(number))
    ```
  * print fibonacci<br/> 
    ```python
    number = int(input("Enter a number!\n"))

    if number <= 0:                         # dont forget to check edge cases
        print("Enter positive numbers")
    elif number == 1:
        print(1)
    else:
        n1, n2 = 0,1
        for i in range(number):
            # n1, n2 = n2, n1 + n2
            # or
            temp = n2     # a temporary variable to hold n2. so, we wont forget n2.
            n2 = n1+n2
            n1 = temp
    print("{}th fibonacci number is {}".format(number,n2))
    ```
  * check prime <br/> 
    ```python
    import math

    number = int(input("Enter a number!\n"))
    if number > 0 :
        hasDivisor = False
        for i in range(2,math.ceil(math.sqrt(number))):
        if number % i == 0:
            hasDivisor = True
            break
    if hasDivisor:
        print("{} is not prime!".format(number))
    else:
        print("{} is prime!".format(number))
    ```
  * check palindrome<br/> 
    ```python
    input = input("Enter a text!\n")
    text = input.replace(" ","")                      # remove whitespaces
    isPalindrome = True
    for i in range(len(text)//2):                     # loop until half of the string
        if text[i] != text[len(text)-1-i]:            # if nth from the beginning and nth from the ending
            isPalindrome = False                      # characters does not match, finish
            break
    if not isPalindrome:
        print("{} is not palindrome.".format(input))
    else:
        print("{} is palindrome.".format(input))
    ```
  * reverse number<br/> 
    ```python
    number = int(input("Enter a number!\n"))
    remainder, reverse, temp = 0, 0, number
    while temp > 0:
        remainder = temp % 10
        reverse = reverse*10 + remainder
        temp = temp // 10
    print("reverse of {} is {}".format(number,reverse))
    ### think it like that:
    ### remai   rever       temp
    ### 0       0           423
    ### 3       0*10+3=3    42
    ### 2       3*10+2=32   4
    ### 4       32*10+4=324 0
    ```
  * decimal to binary<br/> 
    ```python
    number = int(input("Enter a number!\n"))
    temp = number
    result = ""
    while temp > 0:
        result = str(temp % 2) + result  ## append remainder to the left
        temp = temp // 2                 ## divide number by two
    print("Binary representation of {} is {}".format(number,result))
    ```
  * bubble sort<br/> 
    ```python
    arr = [65,-26,41,4,62,21,145,3,-21,12,18,54]  
     n = len(arr)

     # Traverse through all array elements
     for i in range(n):
          # Last i elements are already in place
          for j in range(0, n-i-1):
               # traverse the array from 0 to n-i-1
               # If the element found is greater than the next element
               if arr[j] > arr[j+1] :
                    arr[j], arr[j+1] = arr[j+1], arr[j]   # Swap

     print ("Sorted array is: ", arr)
    ```
    illustration: <br>
    ![image](https://user-images.githubusercontent.com/47869761/118177373-47774100-b43b-11eb-98a0-e4511bb4bd87.png)
    <br> source: https://www.geeksforgeeks.org/bubble-sort/
    
  * binary search<br/> 
    ```python
    arr = [-5, 2, 6, 8, 10, 11, 16, 17, 100] # array MUST be already sorted to begin binary search
     x = 9                                   # number to be searched for
     lower_index = 0
     higher_index = len(arr)
     result = -1                              # if x is not found, result is -1
     while lower_index <= higher_index:

         mid = lower_index + (higher_index - lower_index) // 2; # middle of the list
     
        # Check if x is present at mid
        if arr[mid] == x:
            result = mid                # great we found it!
            break                       # break the loop

        # If x is greater, ignore left half
        elif arr[mid] < x:
            lower_index = mid + 1       # x is more than middle element of the list, so ignore other half

        # If x is smaller, ignore right half
        else:
            higher_index = mid - 1      # x is less than middle element of the list, so ignore other half

    if result != -1:
        print ("Element is present at index {}".format( result))
    else:
        print ("Element is not present in array")
    ```
  * find prime factors<br/> 
    ```python
    import math
     
    def primeFactors(number):
        if number < 2:
            print("number must be greater than 2.")
            return ""
        # First handle 2's.
        while number % 2 == 0: # if number is even, print 2 and divide by two
            print (2)
            number = number // 2
             
        # since we got out of the loop above, we are pretty sure that number is now odd.
        # let's iterate over odd numbers starting from 3 to sqrt(number).
        for i in range(3,int(math.sqrt(number))+1,2):
            print("xxx",i)
            # if i divides n , print i and divide n
            # actually this is the same as the first loop, just i instead of 2
            while number % i== 0:
                print (i)
                number = number // i
                 
        # this is the last factor
        if number > 1:
            print (number)
             

    number = 1
    primeFactors(number)
    ```
  
</details>

<details> <summary> INTERESTING STUFF </summary>
   
  * url shortener <br/> 
    ```python
    import pyshorteners

    def shortener(link):
        shortener_object = pyshorteners.Shortener()
        short_link = shortener_object.tinyurl.short(link)
        return short_link

    link = input("Enter url: ")
    short = shortener(link)
    print(short)
    ```
  * youtube video downloader <br/> 
    source: https://www.dynamiccoding.tech <br>
    ```python
    # necesary imports
    from tkinter import *
    import pathlib
    from pytube import YouTube
    # if you get error, type "pip install pytube" to cmd
    from tkinter import messagebox, filedialog

    def Browse():
        download_directory = filedialog.askdirectory(initialdir=pathlib.Path.cwd())
        download_path.set(download_directory)

    def Download():
        youtube_link = video_link.get()
        download_folder = download_path.get()
        getVideo = YouTube(youtube_link)
        videoStream = getVideo.streams.first()
        videoStream.download(download_folder)
        messagebox.showinfo("SUCCESSFULLY", "DOWNLOADED AND SAVED IN\n" + download_folder)

    def Widgets():
        link_label = Label(root, text="Youtube link :", bg="#E8D579", width=20)
        link_label.grid(row=1, column=0, pady=5, padx=5)

        link_text = Entry(root, width=55, textvariable=video_link)
        link_text.grid(row=1, column=1, pady=5, padx=5, columnspan=2)

        destination_label = Label(root, text="Destination : ", bg="#E8D579", width=20)
        destination_label.grid(row=2, column=0, pady=5, padx=5)

        destination_text = Entry(root, width=40, textvariable=download_path)
        destination_text.grid(row=2, column=1, pady=5, padx=5, columnspan=2)

        browse_b = Button(root, text="Browse", command=Browse, width=10, bg="#05E8E0")
        browse_b.grid(row=2, column=2, pady=1, padx=1)

        download_b = Button(root, text="Download", command=Download, width=10, bg="#05E8E0")
        download_b.grid(row=3, column=1, pady=3, padx=3)

    # creating mainwindow
    root = Tk()
    root.geometry("500x110")
    root.resizable(0,0)
    root.title("Our Very Own Youtube Downloader")
    # creating tkinter variables
    video_link = StringVar()
    download_path = StringVar()
    Widgets()
    root.mainloop()
    ```
  * convert video to audio <br/> 
    source: https://www.dynamiccoding.tech <br>
    ```python
    import moviepy.editor
     # pip install moviepy

     path = "C:/Users/Veyis/Desktop/"
     video_name ="iddaacom  Aston Villa - Everton (0-0) - Maç Özeti - Premier League 202021.mp4" # path of the video
     video = moviepy.editor.VideoFileClip(path+video_name)

     audio_data = video.audio
     audio_data.write_audiofile(path+"audio_name.mp3")
     ```
  * fetch instagram profile details <br/> 
    ```python
    from instagramy import InstagramUser
    SESSION_ID=""
    user = InstagramUser("lanadelrey",sessionid=SESSION_ID)
    # print(user.user_data)
    # print(user.posts)
    #### Sort users post with respect to likes and print out likes, comments, url.
    sortedposts = sorted(user.posts, key=lambda item: item[0], reverse=True)
    for post in sortedposts:
        print(post[0], post[2], post[7], sep=", ")
    print(user.biography)
    print(user.no_of_mutual_follower)
    print(user.other_info)
    print(user.connected_fb_page)
    print(user.number_of_followers)
    print(user.profile_picture_url)
    ```
  * number guessing game<br/> 
    ```python
    import random
    import math

    x = random.randint(0, 100)  # a random number between 0 and 100
    count = 0                   # the number of guesses.

    while True:
        count += 1
        # taking guessing number as input
        guess = int(input("Guess a number between 0 and 100:- "))
     
        if x == guess: # found it
            print("Congratulations you did it in ",
                  count, " try")
            # Once guessed, loop will break
            break
        elif x > guess: # guess is smaller
            print("You guessed too small!")
        elif x < guess: # guess is higher
            print("You Guessed too high!")

    ```
  * rock paper scissors <br/>
    ```python
    import random

    user_win = 0
    computer_win = 0
    while True:
        user_action = input("Enter a choice: r, p, s for rock, paper, scissors respectively: ")
        possible_actions = ["rock", "paper", "scissors"]
        computer_action = random.choice(possible_actions)
        print(f"\nYou chose {user_action}, computer chose {computer_action}.\n")

        if user_action == computer_action:
            print(f"Both players selected {user_action}. It's a tie!")
        elif user_action == "r":
            if computer_action == "scissors":
                print("Rock smashes scissors! You win!")
                user_win += 1
            else:
                print("Paper covers rock! You lose.")
                computer_win += 1
        elif user_action == "p":
            if computer_action == "rock":
                print("Paper covers rock! You win!")
                user_win += 1
            else:
                print("Scissors cuts paper! You lose.")
                computer_win += 1
        elif user_action == "s":
            if computer_action == "paper":
                print("Scissors cuts paper! You win!")
                user_win += 1
            else:
                print("Rock smashes scissors! You lose.")
                computer_win += 1

        print(f"""You: {user_win}
    Computer: {computer_win}""")
        play_again = input("Play again? (y/n): ")
        if play_again.lower() != "y":
            break

    print(f"""
    FINAL SCORE
    You: {user_win}
    Computer: {computer_win}""")

    ```
  * website blocker<br/> 
    ```python
    
    ```
  * pdf merge <br/> 
    ```python
    
    ```
  * random password generator <br/> 
    ```python
    
    ```
</details>
<br>
Derived from  https://docs.python.org/3/tutorial/ and  https://www.w3schools.com/python/
<br>
[1]: https://docs.python.org/3/tutorial/introduction.html#lists
<br>
