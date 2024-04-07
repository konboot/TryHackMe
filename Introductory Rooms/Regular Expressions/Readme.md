<h1 align="center" font-size=300px>

<b>REGEX</b>
<br>{Regular Expression}
</h1>

<h2 align="center">Task1: Introduction</h2>

<p align="center">Regular expressions (or Regex) are patterns of text that you define to search documents and match exactly what you're looking for.
<br>There are two ways to test your expressions:

- Create a text file with some test paragraphs (in a Unix machine) and then use egrep <pattern> <file> to see what matches and what doesn't, or
- Use an online editor like https://regexr.com/. You can add your own text in the "Text" field, and then type your expressions (patterns) in the "Expression" field.

![image](https://github.com/konboot/TryHackMe/assets/53315283/56397693-bf15-44a9-b3fe-53779778c6f6)

<h2 align="center">Task2: Charsets</h2>
<p>When searching for a specific string in a file or block of text, you can search for it as is, with <b>grep 'string' <file_name> </b>

- [abc] will match a, b, and c (every occurrence of each letter)
[abc]zz will match azz, bzz, and czz.

- You can also use a - dash to define ranges:
[a-c]zz is the same as above.

- And then you can combine ranges together:
[a-cx-z]zz will match azz, bzz, czz, xzz, yzz, and zzz.

- Most notably, this can be used to match any alphabetical character:
[a-zA-Z] will match any single letter (lowercase or uppercase).

- You can use numbers too:
file[1-3] will match file1, file2, and file3.

- Then, there is a way to exclude characters from a charset with the ^ hat symbol, and include everything else.
[^k]ing will match ring, sing, $ing, but not king.

- Of course, you can exclude charsets, not just single characters.
[^a-c]at will match fat and hat, but not bat or cat.

![image](https://github.com/konboot/TryHackMe/assets/53315283/1e998611-8b2e-4043-9a1a-6c35ea42052b)

</p>

<h2 align="center">Task3: Wildcards and optional characters</h2>
The wildcard that is used to match any single character (except the line break) is the . dot. That means that a.c will match aac, abc, a0c, a!c, and so on.

Also, you can set a character as optional in your pattern using the ? question mark. That means that abc? will match ab and abc, since the c is optional.

Note: If you want to search for . a literal dot, you have to escape it with a \ reverse slash. That means that a.c will match a.c, but also abc, a@c, and so on. But a\.c will match just a.c.

![image](https://github.com/konboot/TryHackMe/assets/53315283/0d1b9bd0-b89a-4e0a-a968-0ad246537312)

<h2 align="center">Task4: Metacharacters and repetitions</h2>
There are easier ways to match bigger charsets. For example, \d is used to match any single digit. Here's a reference:

- \d matches a digit, like 9
- \D matches a non-digit, like A or @
- \w matches an alphanumeric character, like a or 3
- \W matches a non-alphanumeric character, like ! or #
- \s matches a whitespace character (spaces, tabs, and line breaks)
- \S matches everything else (alphanumeric characters and symbols)

Note: Underscores _ are included in the \w metacharacter and not in \W. That means that \w will match every single character in test_file.

Often we want a pattern that matches many characters of a single type in a row, and we can do that with repetitions. For example, {2} is used to match the preceding character (or metacharacter, or charset) two times in a row. That means that z{2} will match exactly zz.

Here's a reference for each repetition along with how many times it matches the preceding pattern:

- {12} : exactly 12 times.
- {1,5} : 1 to 5 times.
- {2,} : 2 or more times.
- *:  0 or more times.
- +: 1 or more times.

![image](https://github.com/konboot/TryHackMe/assets/53315283/de3c9573-a3c3-4853-b2f5-79dfb78d3552)
![image](https://github.com/konboot/TryHackMe/assets/53315283/b658b82e-8951-419a-a2ab-74829c0a249c)

<h2 align="center">Task5: Starts with/ ends with, groups, and either/ or</h2>
Sometimes it's very useful to specify that we want to search by a certain pattern in the beginning or the end of a line. We do that with these characters:
<br>^ - starts with
<br>$ - ends with

So for example, if you want to search for a line that starts with abc, you can use ^abc.
If you want to search for a line that ends with xyz, you can use xyz$.

Note: The ^ hat symbol is used to exclude a charset when enclosed in [square brackets], but when it is not, it is used to specify the beginning of a word.

You can also define groups by enclosing a pattern in (parentheses). This function can be used for many ways that are not in the scope of this tutorial. We will use it to define an either/ or pattern, and also to repeat patterns. To say "or" in Regex, we use the | pipe.

For an "either/or" pattern example, the pattern during the (day|night) will match both of these sentences: during the day and during the night.
For a repetition example, the pattern (no){5} will match the sentence nonononono

![image](https://github.com/konboot/TryHackMe/assets/53315283/dc541e7b-b744-4347-94d1-4fb8dd9b71e2)
![image](https://github.com/konboot/TryHackMe/assets/53315283/faa16d2b-8696-49d2-abcf-53817f317454)

