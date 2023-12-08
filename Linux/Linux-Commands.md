\[ [Wikipeter](../README.md) > [Linux](../Linux.md) > Linux Commands \]
# Linux Commands

| **Linux Command** | **Description** | **Example** |
| --- | --- | --- |
| **cat** |  Short for con**cat**enate, allows you to combine and display the contents of multiple files. This command on a single file will enable you to display its contents.|`cat file.log`|
| **cut** | The **cut** command allows you to extract specific sections (columns) of lines from a file or input stream by "cutting" the line into columns based on a delimiter and selecting which columns to display. Use the `-d` option to set delimiter and the `-f` for position. | `cut -d ' ' -f1 file.log`<br><br>`cut -d ' ' -f1,3,6 file.log` |
| **less** | The less command allows you to view the contents of a file one page at a time. Compared to the cat command, this allows you to easily review the contents without being overwhelmed by the large quantity of the log file. | `less file.log` |
| **head** | The head command lets you view the first 10 entries from the top of the file. Use `-n` to specify number of lines displayed. | `head`<br>`head -n 3` |
| **tail** | The tail command lets you view the last 10 entries from the top of the file. Use `-n` to specify number of lines displayed. | `tail`<br>`tail -n 3` |
| **wc** | The wc command stands for **word count**. It's a command-line tool that counts the number of lines, words, and characters in a text file. Use `-l` to display the line count only. | `wc`<br>`wc -l` |
| **nl** | The nl command stands for **number lines**. It renders the contents of the file in a numbered line format. | `nl` |
