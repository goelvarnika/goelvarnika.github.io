# 4-12-2019
## Today I started with exploring awk command in bash shell.awk command searches files for text containing a pattern.When a line or text matches, awk performs a specific action on that line/text. 
Let's start with simple programs
  1. print the first field
     awk ’{print $1}'
  2. print the second field
     awk ’{print $2}’
  
  3. print the last field
    awk ’{print $NF}’
  
  4. print the penultimate field
     awk ’{print $(NF-1)}’
  rev | cut -f2 | rev
  5. print the number of fields
     awk ’{print $NF}’
  6. print the number of
syllables (sequences of vowels) in a file which are more than ten times
<br>
I used genesis.txt which I first tokenised by using 'tr' command 
<br>
I then replaced all consonants by x which I replaced by a new line
<br>
I counted each vowel sequence by using uniq -c command 
<br>
so my final command is
<br>
<i> tr -sc 'A-Za-z' '\012' < genesis |sed 's_[^AEIOUaeiou]_x_g'|tr -s 'x' '\012'|sort|uniq -c|awk '$1>10 {print}'<i>
<br>
<h1> how to create a bigram </h1>
<i>tr -sc ’A-Za-z’ ’\012’ < genesis > genesis.words
<br>
tail +2 genesis.words > genesis.nextwords
<br>
paste genesis.words genesis.nextwords<i>
7. It is said that English avoids sequences of -ing words.Find bigrams where both words end in -ing. Do these count as counter-examples to the -ing -ing rule?
<br> code
<i>paste genesis.hist genesis.w2|sort|uniq -c|awk '$2~ /ing$/ && $3~ /ing$/'</i>
<br>
tomorrow I will study Mutual Information, shell scripting 
