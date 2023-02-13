I use the grep command 

## Grep -l ##

# Ex 1: 
```
# code block #
 grep -l "Lucayans" ./written_2/*/*/*
 
 # output #
 grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory
grep: ./written_2/non-fiction/OUP/Castro: Is a directory
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz2/Bahamas-History.txt
```
This grep statment checks if if the path ./written_2/*/*/* contains any string called "Lucayans", 
if so it returns the list of the file name that matches the input string only. It's useful because because can print the file path to the string only. 

# Ex 2 :

```
# code block #
[cs15lwi23adt@ieng6-201]:skill-demo1-data:539$ grep -l "Hedonism" ./written_2/*/*/*

# output #

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory
grep: ./written_2/non-fiction/OUP/Castro: Is a directory
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz1/HandRJamaica.txt
```

This grep statment checks if if the path ./written_2/*/*/* contains any string called "Hedonism", 
if so it returns the list of the file name that matches the input string only. It's useful because because can print the file path to the string only. 

## grep -n ##

# Ex 1: #

```
# code block #

[cs15lwi23adt@ieng6-201]:skill-demo1-data:540$ grep -n "Lucayans" ./written_2/*/*/*

# output #

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory 
./written_2/travel_guides/berlitz2/Bahamas-History.txt:6:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modeuries befost crops and from what they caught from sea and shore. Nothincalled theg in the experience of these gentle people could have prepare from Soutd them for the arrival of the Pinta, the Niña, and the Santa , survivin
Maria at San Salvador on 12 October 1492. Columbus believed tsea and shhat he had reached the East Indies and mistakenly called thesave prepare people Indians. We know them today as the Lucayans. Columbu Maria at s claimed the island and others in the Bahamas for his royal d reached 
Spanish patrons, but not finding the gold and other riches hee know the was seeking, he stayed for only two weeks before sailing towrs in the ards Cuba.                                                   ld and oth
./written_2/travel_guides/berlitz2/Bahamas-History.txt:7:The  sailing t
Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passSpaniards ed through the archipelago en route to and from the Caribbeanipwrecks a, Florida, Bermuda, and their home ports. On Eleuthera the expelago en plorers dug a fresh-water well — at a spot now known as “Spanhome portsish Wells” — which was used to replenish the supplies of wateot now knor on their ships before they began the long journey back to Eies of waturope with their cargoes of South American gold. As for the LEurope witucayans, within 25 years all of them, perhaps some 30,000 peowithin 25 ple, were removed from the Bahamas to work — and die — in Sparom the Banish gold mines and on farms and pearl fisheries on Hispanioland pearl a (Haiti), Cuba, and elsewhere in the Caribbean.   
```

The grep -n prints out the matched line and their line number that contains "Lucayans" in the file in the path. This is useful if we want to know the exact line of the input what the paragraph is talking about it. 

# Ex 2: #

```
# code block #

[cs15lwi23adt@ieng6-201]:skill-demo1-data:541$ grep -n "Hedonism" ./written_2/*/*/*

# output #

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory       
grep: ./written_2/non-fiction/OUP/Castro: Is a directory     
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory   
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory   
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz1/HandRJamaica.txt:7:       
 Hedonism II ❁❁❁❁❁ (AI) Norman Manley Blvd. , P.O. Box 25,  
 
 ```
 
 The grep -n prints out the matched line and their line number that contains "Hedonism" in the file in the path. This is useful if we want to know the exact line of the input what the paragraph is talking about it. 
 
## grep -i ## 

# Ex 1: #

```
# code block #

[cs15lwi23adt@ieng6-202]:skill-demo1-data:500$ grep -i  "hedonism" ./written_2/*/*/*

# output 
grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory
grep: ./written_2/non-fiction/OUP/Castro: Is a directory
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz1/HandRJamaica.txt:        Hedonism II ❁❁❁❁❁ (AI) Norman Manley Blvd. , P.O. Box 25,
./written_2/travel_guides/berlitz1/HistoryMadrid.txt:        Franco era through acts of hedonism and creative films, music and
./written_2/travel_guides/berlitz1/IntroMallorca.txt:        the unbridled hedonism of topless beaches and singles bars, and the
./written_2/travel_guides/berlitz1/WhatToMadeira.txt:        Brazilian-style 
samba rhythms — but don’t expect the hedonism or

grep -i prints out the file in the path that contains the input string no matter the case. This is useful when we want search if the path contain a string, no matter the syntax, which is useful for research. 


# Ex 2: #

``` 
# code block #

[cs15lwi23adt@ieng6-202]:skill-demo1-data:501$ grep -i  "hogmanay" ./written_2/*/*/*

# output #

grep: ./written_2/non-fiction/OUP/Abernathy: Is a directory
grep: ./written_2/non-fiction/OUP/Berk: Is a directory
grep: ./written_2/non-fiction/OUP/Castro: Is a directory
grep: ./written_2/non-fiction/OUP/Fletcher: Is a directory
grep: ./written_2/non-fiction/OUP/Kauffman: Is a directory
grep: ./written_2/non-fiction/OUP/Rybczynski: Is a directory
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt:        world,” called 
Hogmanay. The whole population comes out into the
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:        Hogmanay      
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:        into a five-night Hogmanay Festival of torchlight parades, street
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:        <www.edinburghshogmanay.org>). For those who still have some
./written_2/travel_guides/berlitz1/WhatToEdinburgh.txt:        shortbread (traditionally served at Yuletide and Hogmanay) is rich in

The grep -i command search for the path in written_2 if any of the file contains the string "hogmanay", if so then prints the file path and the line that contains it. This command is useful for research about a particular string since we don't need to care about case. 

## grep -c ##

# Ex 1: #

``` 
# code block #

[cs15lwi23adt@ieng6-202]:skill-demo1-data:504$ grep -c "Hogmanay" ./written_2/*/*/IntroEdinburgh.txt

# output #

1

grep -c prints the count of line that contains "Hogmanay" in the file IntroEdinburgh. This command is helpful if you want to make a data chart of the appearance of input string in a path. 

# Ex 2: # 
```
# code block #

[cs15lwi23adt@ieng6-202]:skill-demo1-data:506$ grep -c "Western" ./written_2/*/*/*/*

# output #
./written_2/non-fiction/OUP/Abernathy/ch1.txt:0
./written_2/non-fiction/OUP/Abernathy/ch14.txt:0
./written_2/non-fiction/OUP/Abernathy/ch15.txt:0
./written_2/non-fiction/OUP/Abernathy/ch2.txt:0
./written_2/non-fiction/OUP/Abernathy/ch3.txt:0
./written_2/non-fiction/OUP/Abernathy/ch6.txt:0
./written_2/non-fiction/OUP/Abernathy/ch7.txt:0
./written_2/non-fiction/OUP/Abernathy/ch8.txt:0
./written_2/non-fiction/OUP/Abernathy/ch9.txt:0
./written_2/non-fiction/OUP/Berk/CH4.txt:4
./written_2/non-fiction/OUP/Berk/ch1.txt:3
./written_2/non-fiction/OUP/Berk/ch2.txt:3
./written_2/non-fiction/OUP/Berk/ch7.txt:1
./written_2/non-fiction/OUP/Castro/chA.txt:0
./written_2/non-fiction/OUP/Castro/chB.txt:0
./written_2/non-fiction/OUP/Castro/chC.txt:0
./written_2/non-fiction/OUP/Castro/chL.txt:0
./written_2/non-fiction/OUP/Castro/chM.txt:0
./written_2/non-fiction/OUP/Castro/chN.txt:0
./written_2/non-fiction/OUP/Castro/chO.txt:0
./written_2/non-fiction/OUP/Castro/chP.txt:0
./written_2/non-fiction/OUP/Castro/chQ.txt:0
./written_2/non-fiction/OUP/Castro/chR.txt:0
./written_2/non-fiction/OUP/Castro/chV.txt:0
./written_2/non-fiction/OUP/Castro/chW.txt:0
./written_2/non-fiction/OUP/Castro/chY.txt:0
./written_2/non-fiction/OUP/Castro/chZ.txt:0
./written_2/non-fiction/OUP/Fletcher/ch1.txt:1
./written_2/non-fiction/OUP/Fletcher/ch10.txt:1
./written_2/non-fiction/OUP/Fletcher/ch2.txt:1
./written_2/non-fiction/OUP/Fletcher/ch5.txt:2
./written_2/non-fiction/OUP/Fletcher/ch6.txt:1
./written_2/non-fiction/OUP/Fletcher/ch9.txt:0
./written_2/non-fiction/OUP/Kauffman/ch1.txt:0
./written_2/non-fiction/OUP/Kauffman/ch10.txt:0
./written_2/non-fiction/OUP/Kauffman/ch3.txt:0
./written_2/non-fiction/OUP/Kauffman/ch4.txt:0
./written_2/non-fiction/OUP/Kauffman/ch5.txt:0
./written_2/non-fiction/OUP/Kauffman/ch6.txt:0
./written_2/non-fiction/OUP/Kauffman/ch7.txt:0
./written_2/non-fiction/OUP/Kauffman/ch8.txt:0
./written_2/non-fiction/OUP/Kauffman/ch9.txt:0
./written_2/non-fiction/OUP/Rybczynski/ch1.txt:0
./written_2/non-fiction/OUP/Rybczynski/ch2.txt:0
./written_2/non-fiction/OUP/Rybczynski/ch3.txt:2

the grep -c prints out the count of line that contains "Western" in the path after OUP. This command is helpful if you want to make a data chart of the appearance of input string in a path. 
