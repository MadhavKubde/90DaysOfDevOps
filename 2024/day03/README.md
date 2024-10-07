# Day 3 Task: Basic Linux Commands with a Twist

Task: What are the Linux commands to

1. View the content of a file and display line numbers.
2. Change the access permissions of files to make them readable, writable, and executable by the owner only.
3. Check the last 10 commands you have run.
4. Remove a directory and all its contents.
5. Create a `fruits.txt` file, add content (one fruit per line), and display the content.
6. Add content in `devops.txt` (one in each line) - Apple, Mango, Banana, Cherry, Kiwi, Orange, Guava. Then, append "Pineapple" to the end of the file.
7. Show the first three fruits from the file in reverse order.
8. Show the bottom three fruits from the file, and then sort them alphabetically.
9. Create another file `Colors.txt`, add content (one color per line), and display the content.
10. Add content in `Colors.txt` (one in each line) - Red, Pink, White, Black, Blue, Orange, Purple, Grey. Then, prepend "Yellow" to the beginning of the file.
11. Find and display the lines that are common between `fruits.txt` and `Colors.txt`.
12. Count the number of lines, words, and characters in both `fruits.txt` and `Colors.txt`.

Reference: [Linux Commands for DevOps Used Day-to-Day](https://www.linkedin.com/pulse/linux-commands-devops-used-day-to-day-activit-chetan-/)

[← Previous Day](../day02/README.md) | [Next Day →](../day04/README.md)



Solutions :-

cd
touch DevOps.txt
cat DevOps.txt 
vim DevOps.txt 
cat -n Devops.txt
cat -n DevOps.txt
chmod 700 DevOps.txt 
ls -l
history | tail -n 10
mkdir AWS
ls
rm -r AWS/
echo -e "Apple\nBanana\nCherry\NMango\nOrange" > fruits.txt
cat fruits.txt
echo -e "Apple\nMango\nBanana\nCherry\nKiwi\nOrange\nGuava" > devops.txt
echo "Pineapple" >> devops.txt
cat devops.txt
head -n 3 fruits.txt | tac
tail -n 3 fruits.txt | sort
echo -e "Red\nPink\nWhite\nBlack\nBlue\nOrange\nPurple\nGrey" > Colors.txt
cat Colors.txt
echo "Yellow" | cat - Colors.txt > temp && mv temp Colors.txt
ct Colors.txt
comm -12 <(sort fruits.txt) <(sort Colors.txt)
wc fruits.txt
wc Colors.txt