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
An incomplete application of full regex support on native FileMaker custom functions. Implementation based on and altered from [tiny-regex-c](https://github.com/kokke/tiny-regex-c).

### Supported regex-operators
The following features / regex-operators are supported by this library.

  -  `.`         Dot; matches any character
  -  `^`         Start anchor; matches beginning of string
  -  `$`         End anchor; matches end of string
  -  `*`         Asterisk; match zero or more (greedy)
  -  `+`         Plus; match one or more (greedy)
  -  `?`         Question; match zero or one (non-greedy)
  -  `[abc]`     Character class; match one of {'a', 'b', 'c'}
  -  `[^abc]`   Inverted class; match one of NOT {'a', 'b', 'c'}
  -  ~~`[a-zA-Z]` Character range(s); match character set of ranges { a-z | A-Z }~~
  -  ~~`[^a-zA-Z]` Inverted range(s); match character set of NOT ranges { a-z | A-Z }~~
  -  `(word)` Matches'word' as a group
  -  ~~`(word|match)` Matches 'word' or 'match' as a group of characters~~
  -  `a{3}`  Matches 'a' 3 times
  -  `a{3,}`  Matches 'a' 3 times or more (greedy)
  -  `a{3,5}`  Matches 'a' 3-5 times (greedy)
  -  `\s`       Whitespace, \t \f \r \n \v and spaces
  -  `\S`       Non-whitespace
  -  `\w`       Alphanumeric, [a-zA-Z0-9_]
  -  `\W`       Non-alphanumeric
  -  `\d`       Digits, [0-9]
  -  `\D`       Non-digits
  -  `\\`       Backslash
  -  `\t \f \r \f \v`       All escaped space characters (not tested)
  -  `\[ \] \( \) \{ \}`       All escaped grouping characters (not tested)
  -  ~~`\^ \- \| \`       All escaped in-group characters within grouping chars~~
  -  `\. \^ \$ \* \+ \?`       All escaped special characters outside grouping chars (not tested)
