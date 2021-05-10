### Terminale ya da başlat menüsüne "idle" yazarak Python terminali açalım.

<details> <summary> MATH</summary>

- ADDITION & SUBTRACTION & MULTIPLICATION
   - `>>> 15 + 4` <br/> `19`
   - `>>> 15 - 4` <br/> `11`
   - `>>> 15 * 4` <br/> `60`
   - `>>> 3.2 + 2` <br/> `5.2`
   - `>>> 3.2 - 3.2` <br/> `0.0`
   - `>>> 3.2 * 5` <br/> `16.0`
 
- DIVISION
   - FLOAT DIVISION vs INTEGER DIVISION
     - `>>> 15 / 4` <br/> `3.75`
     - `15 // 4` <br/> `3`

- POWER & REMAINDER
   - `2 ** 3`<br/> `8`
   - `15 % 7`<br/> `1`

- math LIBRARY
   - `>>> import math`
   - `>>> math.floor(8.4)`<br/> `8`
   - `>>> math.ceil(7.1)`<br/> `8`
   - `>>> math.round(7.6)`<br/> `8`
   - `>>> math.pi`<br/> `3.141592653589793` <br/>`>>> math.e`<br/> `2.718281828459045` <br/>`>>> math.inf`<br/> `inf`
   - `>>> math.fabs(-5)`<br/> `5`
   - `>>> math.sqrt(25)`<br/> `5.0`
   - `>>> math.sin(math.pi/2)` <br/> `1.0`
   - `>>> math.log(10)`<br/> `2.302585092994046`<br/>  `>>> math.log(100,10)`<br/> `2.0`
   - `>>> math.gcd(8,12)`<br/> `4`
   - `>>> math.comb(5,2)`<br/> `10`
   - `>>> math.pow(2,3)`<br/> `8.0`
</details>

<details> <summary> STRINGS</summary>
  
 - CONCATENATION
   - `>>> "hello world"`<br/> `'hello world`
   - `>>> "hello" + " world"`<br/> `'hello world'`
   - `>>> "hello" * 2 `<br/> `'hellohello'`
 - ESCAPE CHARACTER 
   - `>>> "hello \"Ali\""`<br/> `'hello Ali'`
   - `>>> """hello` <br/>
`world` <br/>
`in` <br/>
`multiple lines"""` 
<br/> `'hello\nworld\nin\nmultiple lines'`
 - FORMATTING
   - `>>> "hello {}".format("world")`<br/> `'hello world'`
   - `>>> "Hesap {} TL.".format("2")`<br/> `'Hesap 2 TL.'`
 - INDEXING 
   - `>>> "string"[0]`<br/> `'s'`
   - `>>> "string"[2]`<br/> `'t'`
   - `>>> "string"[-1]`<br/> `'g'`
   - `>>> "string"[1:3]`<br/> `'tr'`
   - `>>> "string"[:-2]`<br/> `'stri'`
   - `>>> "string"[1:]`<br/> `'tring'`
</details>

<details> <summary> VARIABLES</summary>

  - DECLARATION
    - `>>> x = 5`
    - `>>> y = 4.3`
    - `>>> z = "hello"`
    - `>>> Y = 8`
    - `>>> a, b = 5, 6`
    - `>>> a, b = b, a+b`
  - TYPE()
    -  `>>> type(x)`<br/> `'<class 'int'>'`
    -  `>>> type(y)`<br/> `'<class 'float'>'`
    -  `>>> type(z)`<br/> `'<class 'str'>'`
    -  `>>> type(Y)`<br/> `'<class 'int'>'`
    -  `>>> type(True)`<br/> `'<class 'bool'>'`
    -  `>>> type(False)`<br/> `'<class 'bool'>'`
  - CASTING
    - `>>> int(2.6)`<br/> `2`
    - `>>> float(2)`<br/> `2.0`
    - `>>> str(2.6)`<br/> `'2.6'`
    - `>>> str(2)`<br/> `'2'`
    - `>>> int(False)`<br/> `0`
    - `>>> bool(2)`<br/> `True`
</details>

<details> <summary>  INPUT()</summary>

 - `>>> input()`<br/> `2` <br/> `'2'`
 - `>>> int(input())`<br/> `2` <br/> `2`
 - `>>> float(input("Please enter a number"))`<br/> `Please enter a number3.14` <br/> `3.14`
</details>

<details> <summary>  PRINT()</summary>
  
  - `>>> print()`<br/> ` `
  - `>>> print(5)`<br/> `5`
  - `>>> print(3+7.2)`<br/> `10.2`
  - `>>> print("hello")`<br/> `'hello`
  - `>>> print("hello" + " world")`<br/> `'hello world'`
  - `>>> print(x)`<br/> `5`
  - `>>> print(x * y)`<br/> `21.5`
  - `>>> print(x, y, "hello")`<br/> `5 8 hello`
  - `>>> print(x, y, "hello", sep="xx")`<br/> `5xx8xxhello`

</details>

<details> <summary> COMPARISON and BOOLEANS </summary>
  
  - `>>> 9 > 2`<br/> `True`
  - `>>> 9 >= 9.0`<br/> `True`
  - `>>> 9 < 2`<br/> `False`
  - `>>> 9 <= 2`<br/> `False`
  - `>>> 9 == 2`<br/> `False`
  - `>>> 9 != 9.0`<br/> `False`
  - `>>> 3*5 == 15`<br/> `True`
  
</details>

### Şimdi Pycharm'a geçelim.

<details> <summary> IF and INDENTATION </summary>
  
  
  
</details>
  
<details> <summary> LOOPS</summary>

  - ### WHILE
  - ### FOR
  - ##### CONTINUE
  - ##### BREAK
  - ##### RANGE()
</details>

<details> <summary> LISTS and TUPLES </summary>
  
  
  
</details>

<details> <summary> SET and DICT </summary>
  
  
  
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
    
    ```
  * binary search<br/> 
    ```python
    
    ```
  * find prime factor<br/> 
    ```python
 
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
    ` `
  * convert video to audio <br/> 
    ` `
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
  * number huessing <br/> 
    ` `
  * rock paper scissors <br/>
    ` `
  * website blocker<br/> 
    ` `
  * pdf merge <br/> 
    ` `
  * random password generator <br/> 
    ` `
</details>
Derived from  https://docs.python.org/3/tutorial/ and  https://www.w3schools.com/python/
