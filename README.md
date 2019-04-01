     _   _             _____          _                
    | \ | |           / ____|        | |               
    |  \| | ___  ___ | |     ___   __| | ___ ______    
    | . ` |/ _ \/ _ \| |    / _ \ / _` |/ _ \______|   
    | |\  |  __/ (_) | |___| (_) | (_| |  __/          
    |_| \_|\___|\___/ \_____\___/ \__,_|\___|          
    | | (_)                                            
    | |_ _ _ __  _   _ ______ _ __ ___  __ _  _____  __
    | __| | '_ \| | | |______| '__/ _ \/ _` |/ _ \ \/ /
    | |_| | | | | |_| |      | | |  __/ (_| |  __/>  < 
     \__|_|_| |_|\__, |      |_|  \___|\__, |\___/_/\_\
                  __/ |                 __/ |          
                 |___/                 |___/           


# NeoCode-tiny-regex
An incomplete regex implementation on native FileMaker custom functions

### Supported regex-operators
The following features / regex-operators are supported by this library.

NOTE: inverted character classes are buggy - see the test harness for concrete examples.


  -  `.`         Dot, matches any character
  -  `^`         Start anchor, matches beginning of string
  -  `$`         End anchor, matches end of string
  -  `*`         Asterisk, match zero or more (greedy)
  -  `+`         Plus, match one or more (greedy)
  -  `?`         Question, match zero or one (non-greedy)
  -  ~~`[abc]`     Character class, match if one of {'a', 'b', 'c'}~~
  -  ~~`[^abc]`   Inverted class, match if NOT one of {'a', 'b', 'c'}~~
  **`NOTE: This feature is currently broken for some usage of character ranges!`**
  -  ~~`[a-zA-Z]` Character ranges, the character set of the ranges { a-z | A-Z }~~
  -  `\s`       Whitespace, \t \f \r \n \v and spaces
  -  `\S`       Non-whitespace
  -  `\w`       Alphanumeric, [a-zA-Z0-9_]
  -  `\W`       Non-alphanumeric
  -  `\d`       Digits, [0-9]
  -  `\D`       Non-digits
