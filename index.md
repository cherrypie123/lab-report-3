I use the grep command 

Grep -l
Ex 1: 
# code block 
 grep -l "Lucayans" ./written_2/*/*/*
 
 # output 
 grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory
grep: ./written_2/non-fiction/OUP/Castro: Is a directory
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz2/Bahamas-History.txt

This grep statment checks if if the path ./written_2/*/*/* contains any string called "Lucayans", 
if so it returns the list of the file name that matches the input string only. It's useful because because can print the file path to the string only. 

Ex 2:

# code block 
[cs15lwi23adt@ieng6-201]:skill-demo1-data:539$ grep -l "Hedonism" ./written_2/*/*/*

# output 

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory
grep: ./written_2/non-fiction/OUP/Castro: Is a directory
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz1/HandRJamaica.txt

This grep statment checks if if the path ./written_2/*/*/* contains any string called "Hedonism", 
if so it returns the list of the file name that matches the input string only. It's useful because because can print the file path to the string only. 

Grep -n
Ex 1:
# code block

[cs15lwi23adt@ieng6-201]:skill-demo1-data:540$ grep -n "Lucayans" ./written_2/*/*/*

# output 

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory 
./written_2/travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modeuries befost crops and from what they caught from sea and shore. Nothincalled theg in the experience of these gentle people could have prepare from Soutd them for the arrival of the Pinta, the Niña, and the Santa , survivin
Maria at San Salvador on 12 October 1492. Columbus believed tsea and shhat he had reached the East Indies and mistakenly called thesave prepare people Indians. We know them today as the Lucayans. Columbu Maria at s claimed the island and others in the Bahamas for his royal d reached 
Spanish patrons, but not finding the gold and other riches hee know the was seeking, he stayed for only two weeks before sailing towrs in the ards Cuba.                                                   ld and oth
./written_2/travel_guides/berlitz2/Bahamas-History.txt:7:The  sailing t
Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passSpaniards ed through the archipelago en route to and from the Caribbeanipwrecks a, Florida, Bermuda, and their home ports. On Eleuthera the expelago en plorers dug a fresh-water well — at a spot now known as “Spanhome portsish Wells” — which was used to replenish the supplies of wateot now knor on their ships before they began the long journey back to Eies of waturope with their cargoes of South American gold. As for the LEurope witucayans, within 25 years all of them, perhaps some 30,000 peowithin 25 ple, were removed from the Bahamas to work — and die — in Sparom the Banish gold mines and on farms and pearl fisheries on Hispanioland pearl a (Haiti), Cuba, and elsewhere in the Caribbean.     

The grep -n prints out the matched line and their line number that contains "Lucayans" in the file in the path. This is useful if we want to know the exact line of the input what the paragraph is talking about it. 

Ex 2:

# code block

[cs15lwi23adt@ieng6-201]:skill-demo1-data:541$ grep -n "Hedonism" ./written_2/*/*/*

# output 

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory       
grep: ./written_2/non-fiction/OUP/Castro: Is a directory     
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory   
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory   
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz1/HandRJamaica.txt:7:       
 Hedonism II ❁❁❁❁❁ (AI) Norman Manley Blvd. , P.O. Box 25,  
 
 The grep -n prints out the matched line and their line number that contains "Hedonism" in the file in the path. This is useful if we want to know the exact line of the input what the paragraph is talking about it. 
 
 
