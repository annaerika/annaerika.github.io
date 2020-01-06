---
layout: default
---

### KIK-LG219 Command line tools for linguists

In this course we learned the basics of working in a command line interface (CLI). In the first weeks we were introduced to the command line environment and learned how to navigate in a UNIX system as well as how to connect to a remote server. Later, we learned about corpus processing, which sure will come in handy for many language specialists. After this we were able to apply our skills in basic scripting. Finally, the contents of week six and seven taught us how to install and run programs and what version control like Git is, and why it is so powerful.  

Here I will briefly list and describe the themes and key commands introduced in each week's contents.

#### week 1: Setting up & essential commands

The first week was all about setting up the command line environment and learning how to make use of very basic commands like `cd`, `mkdir`, `ls`, `cat` and `less`. We got an introduction to mainly *emacs* but were encouraged to use any text editor we desired. For example, I worked with emacs for the most part of the course but eventually switched to *nano*. 

#### week 2: Digging deeper in the UNIX system, processes & remote servers

The first part of this week's tasks included getting a deeper insight into the previous contents of the first course week. Some key subjects were using different options for commands (`ls -F`), handling and modifying file permissions with `chmod` and finding ourselves in the system using `pwd`. We were also to learn how to compress and decompress files and directories with the commands `gzip` and `tar` in order to hand in our weekly homework.

The following part was an introduction to processes. We mainly learned theory related to the theme but also experienced how to run commands in the background for a random period of time and eventually kill a process. For instance, `sleep 5` puts bash asleep for five seconds. To run this process in the background, we write `sleep 5 &`.

Finally we covered a topic I personally found the most interesting and very useful: switching between local and remote servers. We learned to use the *ssh-program*, which uses secure shell to connect to a remote server. We even got to see an interview by Tatu Ylönen, the creator of ssh.  

#### week 3: Corpus processing for rookies

Text and corpus processing. Probably one of the topics that we students found most challenging. We started off by checking that our system supports utf-8 encoding, because working with a lot of corpora will eventually lead to the need of proper language settings. Fairly soon we also learned to use the commands `unix2dos` and `dos2unix`, which convert Unix text files to a Windows plain text format and vice versa:
> `unix2dos unixpoem.txt`

For many questions in our weekly quizzes we had to find all instances of a word in a text. For this we worked with regular expressions and the grep command:
> `egrep "\b[Bb]ird\b" bird.txt` seeks all instances of **bird** or **Bird** in **bird.txt**. `\b` stands for word boundary. `egrep` is the same as `grep -E` and stands for extended regular expressions.

> `egrep "\bnest\b" bird.txt | wc -l` seeks all instances of **nest** in **bird.txt**. `wc -l` counts all the lines where **nest** appears.
Other useful commands that we learned are `head` (to read lines beginning from the first line of the file) and `tail` (to read lines from the last line of the file), `uniq` to search all repated lines and read them as one line only, `sort` to sort the lines ina file into either alphabetical or numerical order and finally `tr` to translate or transform some characters into others (for example, capital letters to lower case letters).

Besides having fun with ReGex we read about formatted text files, like .csv (comma-separated-values). A .csv-file can look like something like this:
![csv_example](./assets/img/csv_example.png)

#### week 4:  

#### week 5:

#### week 6:

#### week 7:

#### week 8: Final Assignment

The final assignment for this course was creating a webpage using GitHub templates. This is mine, enjoy!
