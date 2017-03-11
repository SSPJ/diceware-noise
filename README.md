## Purpose

This script connects to Random.org over https and downloads a pool of 60 "keys" which are used to generate human-readable passphrases from words off the Diceware word list.

Default password length is 7 words; default word list (included) is original English 7,777. Both of these can easily be changed.

**Sample output:** shark bauer ned guyana hh weco argo

## Usage

1. Download english_alphabet and put it somewhere
2. Open a terminal or command prompt in the location you saved it and type
    ```
    perl english_alphabet
    ```
If you want a different length password/phrase, use *-n number_of_words*

    ```
    perl english_alphabet -n 12
    ```
If you want a different word list, use *-f filename*

    ```
    perl english_alphabet -f other_dictionary.txt
    ```
where *other_dictionary.txt* must be a set of entries, one per line, of 5 numbers followed by spaces/tabs and a word, number, or puncutation mark. Eg:

    ```
    12345 aword
    12346 differentword
    12351 &
    ```

## License

Embedded wordlist taken from http://world.std.com/~reinhold/diceware.html<br />
It is provided by A G Reinhold under a Creative Commons CC-BY 4.0 license<br />
It is not A G Reinhold's intent that Diceware be done by computers.

Executable code provided for personal use, modification, redistribution, etc in the spirit of the GPL.
