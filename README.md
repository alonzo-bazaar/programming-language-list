# Introduction and Ratio Essendi
A list of programming langauges, repo created because I decided to post a list for shits and giggles and people were suggesting so many additions I decided that, you know what, fuck you, make a pull request.

So here's the repo, because, as previously stated, fuck you.

# Format
We have a `list.csv` file, this file is the coore goddamn thing of the repo, althought the format of `list.csv` is quite self explainatory, I will here document so you don't have to fucking ask me about it.  
As you may guess from its goddamn fucking name, `list.csv` is a list, in a `.csv` file, and is thus structured according to the `csv` format, documented in [rfc 4180](https://www.rfc-editor.org/info/rfc4180/), and kinda updated in [rfc 7111](https://www.rfc-editor.org/info/rfc7111/), but 4180 is enough for our purposes.  

The list csv has two columns, `name` and `website`:
- `name` contains the name of the langauge in the list
- `website` contains a [resolvable url](https://xkcd.com/1700/) to a website about the langauge, so that
  - I can verify the language exist and that you're not shitting me
  - someone interested in the langauge can go rtfm and not fucking bug me about it

If you wish to have the list in a different format, such as json, sqlite, or what have thee, fucking convert it yourself, it's a goddamn csv, it takes like 6 lines of python at best to convert it.

# Note the following
When adding a new language to the list, please keep the following in mind:
1. the list is sorted lexicographically by langauge name, keep it that way or I'm gonna smack you 
2. do not put leading or trailing whitespace in the language name or in the url, in the csv format that whitespace is considered part of the name/url
3. keep the language name lowercase
4. if the name or url contain commas, wrap them in double quotes `""`, if they contain quotes, wrap the name/url in double quotes, then escape all double quotes in the name with anouther double quote, that's how csv escapes shit
5. if the name or url contain newlines, that's your fucking problem

