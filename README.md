# Apple-Sound---From-Beeps-to-Music
5 rem program#1
10 i = 10: HOME
20 print "sound #1": print : list 30,37
30 print chr$ (7)
35 print "": Rem ctrl-G
40 goto 10000
50 i = 50 : HOME
60 print "sound #2": print : list 70,90
70 for loop = 1 to 10
80 print chr$ (7);
90 NEXT
100 goto 10000
110 i = 110:HOME
120 print "sound #3":print : list 130
130 x = peek (-16336)
140 goto 10000
150 i = 150: HOME
160 print "sound #4": print : list 170
170 no = -16336
180 for loop = 1 to 100
190 x = peek (no)
200 NEXT
210 goto 10000
220 i = 220: HOME
230 print "sound #5" : print : list 240
240 no = -16336
250 x = peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) + peek (no) 
260 rem fifteen times
270 goto 10000
280 i = 280: HOME
290 print "sound #6": print : list 300, 330
300 no = -16336
310 for loop =1 to 100
320 x = peek(no) - peek(no) + peek (no) - peek (no) + peek(no) - peek(no) + peek(no)
330 NEXT
10000 poke - 16368,0:vtab 20:htab 1:call - 958: print "'R' for repeat, 'c' to continue ";: get a$
10010 if a$ < > "R" and a$ < > "C" then 10000
10020 if a$ = "c" then 10100
10030 if i = 10 then 30
10040 if i = 50 then 70
10050 if i = 110 then x = peek (-16336): goto 130
10070 if i = 150 then 170
10080 if i = 220 then 240
10090 if i = 280 then 300
10100 if i = 10 then 50
10110 if i = 50 then 110
10120 if i = 110 then 150
10130 if i = 150 then 220
10140 if i = 220 then 280
10150 text: htab 1: print "end of program #1"
