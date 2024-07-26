vim motions and commands  
not sorted in any particular order, might face some mistakes as well

#### misc
- vimcasts
- vimtutor
- vimbegood
- practical vim by drew nell
- vimtips wiki
- vimawesome

### set system variables
| command   | |
|--------------- | --------------- |
| :set number | |
| :set relative number | |
| :set tabstop=4 | |
| :set option! | toggles the previous value |
| :set option? | shows the current value |
| :set invoption | toggles the previous value |
| :set nooption | turns off |
| :set incsearch | search highlighting |


### help topics
| command   | |
|--------------- | --------------- |
| :help | manual |
| :h ins-completion |  |
| :h complete | customise AutoComplete |
| :digraphs | list of combinations (Ctrl k -> Ye => ¥) |
| :digraph | define own digraph |
| object-motion | |
| mark-motions | |
| text-objects | |
| registers | |
| map-which-key | |
| key-notation | |

### common commands
| command   | |
|--------------- | --------------- |
| i | insert before cursor |
| a | insert after  cursor |
| I | insert before line |
| A | insert after  line |
| b | moves to beginning of the word |
| B | jump.backward.by.words (no punctuation) |
| w | to start of the next word |
| W | jump.by.words.(spaces separate words) |
| e | moves to end of the word |
| E | jump to.end.of.words.(no punctuation) |
| o | open new line after current line |
| O | open new line before current line |
| 0 | to beginning of line |
| $ | move to end 	  of the line |
| ^ | first non-blank character of line |
| _ | to first word in line            (can be used with motion to jump between lines) |
| - | to previous line's first word   (can be used with motion to jump between lines) |
| * | move to same next word |
| # | move to same previous word |
| gg | beginning of the file |
| G | to end of the file |
| 5G | go the 5th line |
| 25% | to 1/4 of file |
| Shift 0 & Shift 9 | block |
| { } | through paragraphs |
| (  ) | through sentences |
| f | forward to  letter/symbol |
| F | to letter/symbol |
| t | letter/symbol |
| 3f | will find 3rd occurrence |
| T | letter/symbol backward  |
| gi | mode at last edit point |
| gv | highlight |
| % | end/beginning of ()[]{}''"" |
| ctrl u d f b |  jump between page |
| s | remove a character and => insert |
| S | delete content of current line => insert |
| x | to remove right character |
| X | to remove left character |
| C | content of line from cursor to end => insert |
| Y | yank the line after the cursor |
| D | delete the line after the cursor |
| r | to replace a character |
| 3ra | will replace 3 char with a |
| R | replace mode |
| cc | -delete the content in line and INS |
| [p | paste but with indentation |
| ]P | paste but with indentation |
| u | undo |
| U | undo all the changes in last/current edited line |
| Cltr+r | redo |
| / | to search |
| ? | search for upside of the page |
| n | next result |
| N | previous result |
| ;, | between after use of f F t T |
| 5 | INSERT work Esc |
| d5w | delete 5 words |
| d) | delete up to end of the sentence. hello. hi. |
| gU{motion} | 'u' for lowercase |
| gUe | -to end fo the word |
| g~{motion} | uppercase and lowercase |
| 3~ | will change the 3 letter's case |
| vi({ | inside symbol/command   |
| va{ | visual around symbol/command   |
| o | o to switch back to { |
| ciw | change inside word(motion)|
| viw | selects word |
| yi( | -copy everything in () |
| dis | delete inside sentence |
| cip | change inside paragraph |
| dit | delete inside tags HTML/XML |
| c2i{ | change inside { 2 meaning outside { |
| J | to join the lines |
| gJ | to join the lines / no indentation is removed or space is added |

#### write files
|    |  |
|--------------- | --------------- |
| :w | write file |
| ZZ | write file and exit |
| :q | quit file |
| :q! | quit without saving file |
| ZQ | quit without saving file and exit |
| :w filename | will save file with that name if it's new file |
| :w filename | will copy file with that name if it's old file |
| :w >> file | will copy existing content in the mentioned file |
| :wa | will save all opened buffers |
| :w! | will save all even if there are any warnings |
| :w !sudo tee % | will save file with sudo |


#### local mark
|    |  |
|--------------- | --------------- |
| ma | to mark the location with 'a' |
| `a | to go to marked location 'a' |
| 'a | to go to marked line 'a' |
| d'a | will delete till mark 'a' from current position |
| y'a | yank from current cursor to mark a |
| :wshadadelmark A ! | delmark A  |

#### global mark
|    |  |
|--------------- | --------------- |
| mA | to mark the location with 'A' |
| `A | to go to marked location 'A' |
| 'A | to go to marked line 'A' |

#### indent
|    |  |
|--------------- | --------------- |
| =5j | indent 5 lines below |
| =ap | indent around paragraph |
| >> | indent right |
| << | indent left |
| >4j | indent > 4 lines below |
| >} | indent till end of the paragraph |

#### visual block and digit
|    |  |
|--------------- | --------------- |
| Ctrl V | visual block mode |
| Ctrl V I | in selected multiple lines |
| Ctrl a | increment of digit value |
| Ctrl x | decrement of digit value |
| g Ctrl a | increase all the selected digits |
| : norm AHello | add "Hello" at end of each line |
| Ctrl e y | scroll page while lines being selected |
| K | preview documentation |

#### Insert mode
| command   | |
|--------------- | --------------- |
| Ctrl p | matching words in backward direction |
| Ctrl n | matching words in forward direction |
| Ctrl y | confirm selection from popuped list |
| Ctrl xl | AutoComplete line |
| Ctrl e | close popup without any selection |
| Ctrl t | in insert mode indent right current line |
| Ctrl d | in insert mode indent left current line |
| 0 Ctrl d | delete all indentation in line |
| - | move to first character of previous line |
| + | move to first character of next line |
| 3$ | will move to end at 3rd line end counting current |
| 7| | will move to 7th column position |

#### For big line have multiple lines in one line |
| command   | |
|--------------- | --------------- |
| M | move to middle of the page |
| gj | move to below line |
| gk | move to above line |
| g^ | beginning of the line |
| g$ | end of the line |
| zz | reposition current line to middle |  
| zt | reposition current line to top |
| zb | reposition current line to bottom |
| Ctrl o | jump to old location |
| Ctrl i | jump to previous location |

#### g commands
|    |  |
|--------------- | --------------- |
| g; | to last change location |
| g, | to newer change location |
| gi | to last insert location |
| gv | to last visual location |
| ga | displays value of character in decimal hexadecimal and octal |
| g Ctrl g | displays info of cursor |
| Ctrl g | displays file info |
| g_ | to the end of the line excluding the new line character |
| g0 | will move to beginning current line space  |
| gm | move to middle of line considering screen size |
| gM | move to middle of line |
| ge | move to previous words end |
| g* | will go to next matching word even inside word |
| g# | will go to previous matching word even inside word |

#### registers
|    |  |
|--------------- | --------------- |
| "ayy | " to go to register 'a' then saving line to it  |
| "Ayy | to add addition content to "a register |
| "Ayip | to add addition content to "a register |
| "ap | to paste register a |
| "agp | to paste register a, the cursor moves after pasted content |
| :reg a | to see the content of the register |
| qaq | to clear the register "a |
| "0p | default yanked content is stored in 0 register |
| "1p | stored last deleted content |
| "2p | stored 2nd last deleted content |
| 1-9 | same till 9 |
| "+y | stores data into system level clipboard |
| "*y | yanks highlighted |
| "*p | paste highlighted even outside the vim |


#### buffers
|    |  |
|--------------- | --------------- |
| :e# | switch back to previous buffer |
| :e1 | switch back to 1st |
| :e2 | switch back to 2nd |
| Ctrl 6 | switch back to previous buffer |
| :bn | next buffer |
| :bp | previous buffer |

#### tabs
|    |  |
|--------------- | --------------- |
| :tabe filenm | opens file in new tab |
| :0tabe filenm | opens file at first tab |
| :$tabe filenm | opens file at last tab |
| :tabn | switch to next tab |
| :tabp | switch to previous tab |
| :tabr | switch to first tab |
| :tabp | switch to last tab |
| :tabm | moves the tab to last position |
| :tabm 0 | moves the tab to first position |
| :tabm +2 | moves the tab after two tabs |
| :tabm -2 | moves the tab before two tabs |
| 2gt | switch to 2nd tab |
| 2gT | switch to previous 2nd tab |

#### splits
|    |  |
|--------------- | --------------- |
| :sp | splits window horizontally   |
| :vs | splits window vertically |
| Ctrl w w | moves to below/right |
| Ctrl w W | moves to above/left |
| Ctrl w tb | to top/bottom |
| Ctrl w hjkl | |
| Ctrl w HJKL | moves the window itself at farthest |

#### search and replace
|    |  |
|--------------- | --------------- |
| :%s/old/new/g | |
| :s/old/new/g | |
| :1,4s/old/new/g | |
| :s/$/; | ; at the end of selected lines |

#### search
|    |  |
|--------------- | --------------- |
| /search/s+2 | goes at +2 character of search  |
| /search/e+2 | goes at +2 of end of word |
| /search/e | goes at end of search  |
| /search/+2 | goes at 2 line below the match |
| :noh :hlsearch | highlight search |
| //s+3 | empty search will add the content to previous search |

#### replace
|    |  |
|--------------- | --------------- |
| :s/a/b | will replace a with b, only for once replacement |
| :s/a/b/g | will replace all a with b |
| :s/a | will delete a |
| :s/a/b/i | will replace all a with b regardless of case sensitive |
| :4,$s/a/b | will replace a with b, from 4st line to the end of line |
| :%s/a/b | will replace a with b, in entire file |
| :%s//b | will replace a with b, in entire file, // meaning the previous search |

#### advance search and replace
|    |  |
|--------------- | --------------- |
| :g/search/d | g for global, search string, delete |
| :g/search/ | will display all the lines with matching string  |
| :g/search/d a | will delete matching and put inside register a |
| :g/^:s/t0 | will search for lines starting with :s and copy it on top |
| :g/apple s/orange/fig | will search all the lines containing apple and will replace orange with fig in them |
| :g/^:s/ normal >> | will indent all the lines starting with :s |
| normal! | if don't want user defined mapping to be considered |
| :v/:s/d | will delete all the lines which do not contain :s (g! can also be used) |

#### ranges
|    |  |
|--------------- | --------------- |
| :.w | will only write the current line |
| :5d | will delete the 5th line of the file |
| :$d | will delete the last line of the file |
| :5m0 | will move 5th line to 0 line |
| :5t0 | will copy 5th line to 0 line |
| :5co0 | will copy 5th line to 0 line |
| :2,5d | will delete 2nd to 5th line |
| :2,$-2d | will delete 2nd to last line will leave last two lines |
| :%d | will delete all the lines |
| :/one/,/two/d | will delete line from containing one to containing two  |
| :/one/;+2d | will delete line containing one and 2 lines after it |
| :5;/one/d | will delete from 5th line to the pattern |
| :'a'bd | will delete line form a mark to b mark |
| 5: | will have selection from current line to 5th next line |

#### external commands
|    |  |
|--------------- | --------------- |
| :!ls | |
| :!ls co* | will show starting with co  |
| :.! date | will replace current line with date |
| :%!sort | will sort all the lines |
| :3,5!sort | will sort mentioned lines |
| :r! cmd | insert output of the command below current line |
| :r filename | insert content of the file |
| :!grep '^c' % | will display matching lines |

#### terminal
|    |  |
|--------------- | --------------- |
| :terminal | |
| Ctrl w N | will go to normal mode in terminal  |
| Ctrl w : | will go to command mode in terminal |

#### commandline
| command   | |
|--------------- | --------------- |
|    |  | |--------------- | --------------- |
| Ctrl b | will go to beginning / Home  |
| Ctrl e | will go to end / Home  |
| Ctrl w | will delete word before cursor |
| Ctrl u | will delete all character before cursor |
| Ctrl r | will insert register content |
| % | shorthand for current file name  |
| = | will take basic calculations |

#### command line window
|    |  |
|--------------- | --------------- |
| q: | last command list |
| q/? | last search list |
| Ctrl f | to go command list if already in command mode |
| Ctrl c | will take selected command in edit mode |

#### in file mode
|    |  |
|--------------- | --------------- |
| % | to create new file   |
| d | to create new directory   |
| so | to source the changes   |

#### visual mode
| Visual Mode   | |
|--------------- | --------------- |
| visual mode o   | select the other cornor    |
| visual block O   | move to other color of the current line   |
| gn   |  last searched pattern in forward direction and visually select the portion  |
| gn   |  extends the selection if already in visual mode  |
| gN   |  same as gn but in backward direction  |
| cgn   |  clears next search and gets into insert mode|
| .   |  repeats the previous task |

#### regex
| regex   | |
|--------------- | --------------- |
| ^word   |  will search for word that is at the beginning of the line |
| word$   |  will search for word that is at the end of the line |
| $^   | empty lines |
| \<word | will only find word which starts with word |
| word\> | will only find word which ends with word |
| e.d | result -> end eod ead |
| e.*d | result -> e to last occurrence of d |
| e\_.d | as above end of the line search |
| abc* | will follow zero or more occurrence of 'c' |
| abc\? | will folllllow zero or one occurrence of 'c' |
| abc\+ | will follow one or more occurrence of 'c' |
| ?abc\= | for backward search, will follow one or more occurrence of 'c' |
| abc\{1,4\} | will folllllllllllllow one or four occurrence of 'c' |
| abc\{1,\} | will follow atleast four occurrence of 'c' |
| abc\{,4\} | will follow upto four occurrence of 'c' |
| abc\{4} | will follow exact four occurrence of 'c' |
| . | . |
| non-greddy | can be used in substitution |
| w\{-}o | will find w till next o |
| ab\{-1,4}c | . |
| e[[ano]]d | result -> end eod ead |
| <\[[kno]][[ano]]\> |  |
| \a | matches any alphabet character  [a-zA-Z]|
| \A | matches other than alphabet character  [^a-zA-Z]|
| \l | matches lowercase alphabets  [a-z]|
| \L | matches other than lowercase alphabets  [^a-z]|
| \u | matches uppercase alphabets  [A-Z]|
| \U | matches other than uppercase alphabets  [^A-Z]|
| \d | matches any digits  [0-9]|
| \D | matches other than digits  [^0-9]|
| \o | matches any octal character  [0-7]|
| \O | matches other than octal character  [^0-7]|
| \x | matches hexadecimal character  [0-9a-fA-F]|
| \X | matches other than hexadecimal character  [^0-9a-fA-F]|
| \h | matches alphabet and underscore  [a-zA-Z_]|
| \H | matches other than alphabet and underscore  [^a-zA-Z_] |
| \w | matches word character  [a-zA-Z0-9_]|
| \W | matches other than word character  [^a-zA-Z0-9_]|
| \s | matches space and tab character  [ \t]|
| \S | matches other than space and tab character  [^ \t]|
| \.\_s\u | . |

#### visual mode
| alternation   | grouping |
|--------------- | --------------- |
| /min\|max\|both | will search both min and max |
| cool\(er\|est\|\) | a(b\|c)d  will search for abd\|acd cool cooler coolest |
| s/to/X/g | to tototo totottooo |
| s/\(to\)\+/X/g | to tototo totottooo |

#### back references
|    |  |
|--------------- | --------------- |
| \(\a\)\1 | aa pp TT ll SSSSS |
| \(\a\)\1\+ | aa pp TT ll SSSSS |
| s/\d\+/(&)/g | 34 gets replaced with (34) |
| s/\(\w\+\),\(\w\+\)/\2,\1/g | replaces yeah,yo with each other |
| s/\(_\)\?_/\1/g | removes one _ and replaces two __ with one _yo_ __yooo__ |
| s/\(\d\+\)\%(abc\)\+\(\d\+\)/\2:\1/g | will replace 12abcabcabc24 with 24:12, using % before to make it non capturing group |
| s/a \(\d\{3}\)\+/b (\1)/ | replaces 'a 123456789' with 'b (789)' |
| s/a \(\%(\d\{3}\)\+\)/b (\1)/ | replaces 'a 123456789' with 'b (123456789)' |
| . | . |
| . | . |

#### look arounds
| alternation   | grouping |
|--------------- | --------------- |
| ice\d\@! | ice ice34 icedd ice05 |
| s/ice\d\@!/X/g | iceiceice324 |
| par\(.*\<par/>\)\@! | looks for word which doest have par after it parse par paresh |
| at\(\(go\)\@!.\)*par | cat,dog,parrot cat,goes,parrot |
| _\@<!ice | negative cat,dog lookbehind _ice ice _(ice) 42ice |
| \(cat.*\)\@<!dog | fox,cat,dog fox,dog,cat  |
| . | fox,cat,dog fox,dog,cat |
| ice\d\@= | iced ice23 icer ice ice42 |
| _\@<=ice | iced _ice 432ice _(ice) |
| . | difference is that it'll only select the ice not the rest of the part |
| \(cat.*\)\@10<!dog | 10 will only look for 10 bytes |

#### atomic grouping
| alternation   | grouping |
|--------------- | --------------- |
| /0*\d\{3,\} | result of greedy 00432 043 324 |
| /\(0*\)\d\{3,\} | result of atmoic 00432 043 324 |

#### set start and end of the match
| alternation   | grouping |
|--------------- | --------------- |
| \zs | set the start of the match |
| s/\<\w\zs\w*\W*//g | sea eat car rat elf tea |
| \ze | set the end of the match |
| /ice\ze\d | ice ice_2 ice2 iced |

#### magic modifiers
| alternation   | grouping |
|--------------- | --------------- |
| \m | magic mode is activaed by default |
| \M | to disable the magic mode |
| a.b | a.b a=b a*b acb |
| \Ma.b | only searches for a.b |
| \Ma\.b | \ to escape to make it like magic mode |
| \v | can use () {} + ? without prefix \ |
| \<his\> | in normal mode to search for a word |
| \v<his> | same results with very magic mode |
| a<b.*\v<end> | \v is not necessary to use at the start of th line, will search a<b which has 'end' word |
| \vone|two|three | instead of \one\|two\|three |
| very nomagic | \V |
| \V^.*{}$ | matches \V^.*{}$ |
| \V^.*{}$\m.*abcd | \V^.*{}$ can also be used with magic mode |

#### case sensitivity
| alternation   | grouping |
|--------------- | --------------- |
| this | this This tHis tHIS |
| \cthis | \c can be used anywhere this This tHis tHIS  |
| \Cthis | \c can be used anywhere this This tHis tHIS  |
| set ic | ignore case sensitive |
| set ic! | dont ignore case sensitive |
| set noic | dont ignore case sensitive |
| s/boom/booom/gi | boom Boom  boOm|
| . | adding 'i' at the end will mark it as insensitive |

#### backreferences
| alternation   | grouping |
|--------------- | --------------- |
| \u | Uppercase the next character |
| \U | UPPERCASE the following character |
| \l | lowercase the next character |
| \L | lowercase the following character |
| \e or \E | will end further case changes |
| \L or \U | will also override any existing conversion |
| s/\<\l/\u&/g | will convert first letter of the line to uppercase, \l is = [a-z] |
| s/\<\L/\l&/g | THIS WILL CONVERT FIRST LETTERS TO LOWER CASE, \L is = [A-Z] |
| s/\v(\l)_(\l)/\1 \u\2/g | will change this_word to this Word |
| s/\v\l\zs_(\l)/ \u\1/g | same as_above will change this_word to this Word |
| s/.*/\L&/g | cOnvErTs aLL charactER to loWER case|
| s/\a\+/\u\L&/g | wiLL caPitalZe all the worDS |
| s/\v(\a+)(:\a+)/\L\1\U\2/g | will make hEY:yo to hey:YO |
| alternate delimiters |  |
| s,yo/yoyo/,yo.yo. | yo/yoyo/yoooo|

#### escape sequences
| alternation   | grouping |
|--------------- | --------------- |
| \t | searches the tabs |
| \r | carriage return, can be used in substitution |
| \n | end o line character, new line character |
| \%d | matches character specified by decimal digits \%d39 'h' |
| \%x | matches character specified by hexadecimal digits \%d39 'h' |
| \%o | matches character specified by octal digits \%d39 'h' |
|  | can only be used in searching not in replacement |

#### replacement expression
| alternation   | grouping |
|--------------- | --------------- |
| \= | when replacement string starts with \= it's treated at vim expression |
| s/date:\zs /\=strftime("%Y-%m-%d")/ | date:   |
| s/\d\+/\=submatch(0)*2/g | 4 and 3 submatch() fn is similar to backreferences |
| . | 0 gives the entire matched string |
| . | 1 refers to the first capture group and so on |
| s/\(.*\)\zs/\=" = " . eval(submatch(1)) | 10 + 2 - 3 |
10 * 2 - 3
| s/"[^"]\+"/\=substitute(submatch(0), '[aeiou]', '\u&', 'g')/g | "hai" "hoy" |

#### misc
| alternation   | grouping |
|--------------- | --------------- |
| \%V | match inside visaul area only |
| s/\%V10/X/g | yea101001011010  100101010|
| \%[set] | match zero or more of these characters on the same order, as much as possible |
| /spa\%[red] | `spa` 'spar' 'spare' 'spad' |
| /ap\%[[pt]ly] | ap app appl apply apt aptl aptly |
| \_^ \_$ | restrict the match to start of line and end of line respectively, for multiline patters |
| /lastword\_.*\_^firstword | . |
| \%^ \%$ | restrict the match to start of file and end of file |
| ~ | represents the last replacement string, replace yooo with yooo 'yooo' |
| /~ | searches yooo /~' will search for 'yooo' |

#### macro
| alternation   | grouping |
|--------------- | --------------- |
| g/pattern/ norm @r | will execute macro at register r on the pattern |
| add @r | adding @r macro to macro it selfwill call it another time |
| . | wlll keep on doing until the macro execution pattern fails |

#### misc
| alternation   | grouping |
|--------------- | --------------- |
| Ctrl-x | used for AutoComplete |
| Ctrl-l | followed by Ctrl-x will auto complete the whole line |
