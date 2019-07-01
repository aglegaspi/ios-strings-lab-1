# Strings Lab 1

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

Write code that prints out all the numbers from 1 to 10 as a single string.
(Hint: the `String()` function can convert an Int to a String)

```swift
My Answer:

let myRange = 1...10

for i in myRange {
    print(String(i), terminator: " ")
```

***
## Question 2

Write code that prints out all the even numbers from 5 to 51 as a single string.

```swift
My Answer:

let evenRange = 5...51

for e in evenRange {

if e % 2 == 0 {
    print(String(e), terminator: " ")
    }
}
```

***
## Question 3

Write code that prints out every number ending in 4 between 1 and 60 as a single string.

```swift
My Answer:

let powerRanges = 1...60

for p in powerRanges {

    if p % 10 == 4 {
        print(String(p), terminator: " ")
    }
}

```

***
## Question 4

Print each character in the string `"Hello world!"`

```swift
My Answer:

let myString = "Hello World!"

for l in myString {
    print(l)
}


```

***
## Question 5

Print out the last character in the string below.  You cannot use the Character literal "!" (i.e you must access `myStringSeven`'s characters).

`let myStringSeven = "Hello world!"`

```swift
My Answer:

let myStringEnd = myString.endIndex
let lastCharIndex = myString.index(before: myStringEnd)
let lastChar = myString[lastCharIndex]
print(lastChar)

```

***
## Question 6

Write code that switches on a string, given the following conditions:
- If the string's length is even, print out every character.
- If the string's length is odd, print out every other character.

```swift
My Answer:

let switchString = "yoodl"

switch switchString.count % 2 {
    case 0:
        for i in switchString {
            print(i)
        }
    default:
        for (index,letter) in switchString.enumerated() {
            if index % 2 != 0 {
                print(letter)
            }
        }
}

```

***
## Question 7

Initialize a String with a character. Show that it is a Character, and not another String, that you're using to initialize it.

```swift
My Answer:

let myChar: Character = "!"
myChar == Character("!")

```

***
## Question 8

Build five pairs of **canonically equivalent** strings, the first of each being a pre-composed character and the second being one that uses combinable unicode scalars. Show that they are equivalent.

```swift
My Answer:

var letter1 = "B"
var letter2 = "\u{0042}"
letter1 == letter2

var letter3 = "c"
var letter4 = "\u{0063}"
letter3 == letter4

var letter5 = "z"
var letter6 = "\u{007A}"
letter5 == letter6

var letter7 = "O"
var letter8 = "\u{004F}"
letter7 == letter8

var letter9 = "a"
var letter99 = "\u{0061}"
letter9 == letter99

```

***
## Question 9

**Using only Unicode**, print out `"HELLO WORLD!"`

```swift
My Answer:

let heWe = "\u{0048}\u{0045}\u{004C}\u{004C}\u{004F} \u{0057}\u{004F}\u{0052}\u{004C}\u{0044}\u{0021}"

```

***
## Question 10

**Using only Unicode**, print out your name.

```swift
My Answer:

print("\u{0041}\u{006C}\u{0065}\u{0078}")

```

***
## Question 11

**Using only Unicode**, print out `"HELLO WORLD!"` in another language.

```swift
My Answer:

```

***
## Question 12

Print the below flower box using the following information.

- The unicode number for ⚘ is U-2698
- The top and bottom of the box are represented by dashes and the rows are |
- Use the terminator argument in your print statements to print on the same line.
- Hint: It may be useful to try printing out a box of just one character to start then work your way from there.

```swift
Flower Box:
- - - - - - - - - - -
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
- - - - - - - - - - -
```

```swift
My Answer:

```

***
## Question 13

Write a program that sets up a chess board using Unicode.

```swift
Chess Board:
♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖
♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙




♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜
```

```swift
My Answer:

```

***
## Question 14

You are given a string stored in the variable `aString`. Create new string named `replacedString` that contains the characters of the original string with all the occurrences of the character `"e"` replaced by `"\*"`.

```swift
var aString = "Replace the letter e with \*"
// Your code here
 ```

Example:

Input:
`var aString = "Replace the letter e with *"`

Expected values:
`replacedString = "R*plac* th* l*tt*r * with *"`

```swift
My Answer:

```

***
## Question 15

You are given a string stored in variable `aString`. Create a new string called `reverse` that contains the original string in reverse order. Print the reversed string.

```swift
var aString = "this string has 29 characters"
var reverse = ""
```

// Your code here

```swift
My Answer:

```


```

Example:
Input:
`var aString = "Hello"`

Output:
`"olleH"`

***
## Question 16

You are given a string stored in variable `aString`. Print `true` if `aString` is a palindrome, and `false` otherwise. A **palindrome** is a string which reads the same backward or forward.

```swift
let aString = "anutforajaroftuna"

// Your code here
```

```swift
My Answer:

```


```

Example 1:
Input:
`var aString = "anutforajaroftuna"`

Output:
`true`

Example 2:
Input:
`var aString = "Hello"`

Output:
`false`

***
## Question 17

You are given a string stored in variable `problem`. Write code so that you print each word of the string on a new line.

```swift
var problem = "split this string into words and print them on separate lines"
```

```swift
My Answer:

```

```

Example:
Input:
`var problem ="split this string into words and print them on separate lines"`

Output:
```swift
split
this
string
into
words
and
print
them
on
separate
lines
```

***
## Question 18

You are given a string stored in variable `problem`. Write code that prints the longest word in the string.

```swift
var problem = "find the longest word in the problem description"

```

```swift
My Answer:

```

Example:
Input:
`var problem = "find the longest word in the problem description"`

Output:
`description`

Hint: Keep track of the longest word you encounter and also keep track of its length.

***
## Question 19

Given a string in English, create a tuple containing the number of vowels and consonants.

```swift
let vowels = "aeiou"
let consonants = "bcdfghjklmnpqrstvwxyz"
let input = "Count how many vowels I have!"
```

```swift
My Answer:

```

***
## Question 20

Given a string of words separated by a `" "`. Write code that prints out the length of the last word.

If there is no last word print out `"No last word"`.

Example:
Input: `"How are you doing this Monday?"`

Output: `7`

```swift
My Answer:

```

***
