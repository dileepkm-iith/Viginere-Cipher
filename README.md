# Viginere-Cipher

## CIPHER TEXT: 
yvrwxrvmeegfdxgfzywtxzlvlqccbgnpptlqcttwvfadgukginvvgcwkrgcmqrqdogicxzpjmrbccghmuvajecibtfqtppmktptiwsjxvcebihuvajkgkmpenzrhvkkgoxpjhjlvzatlqtgpegtmchozapgfgmabvzapenzztkvpmumjfsvavvvekgjqxhpscabgwdpbvyycwyfphakgcfnccgirqwqitvlqpgffddirfpinpzrntpurditfkdmgrkdgikftfccjukckcggkkwplulpxgikftwkxlxmafdiagzlsbxzbjtnrlsmjvscbvpycwkertztzrnhhkftgckgdgkemjkeflhmkkstgvrqhxosjnmjzqipgernlkorwwcpmugqmcbugilxggkctghfpirpzltwqycgxdpyshrkcctekycwizttmqfsglgcttlvyghvqeqibvlrxhp.

## DECIPHERED TEXT:
we the people of india having solemnly resolved to constitute india into a sovereign socialist secular democratic republic and to secure to all its citizens justice social economic and political liberty of thought expression belief faith and worship equality of status and of opportunity and to promote among them all fraternity assuring the dignity of the individual and the unity and integrity of the nation in our constituent assembly this twenty sixth day of november nineteen forty nine do here by adopt enact and give to ourselves this constitution.

KEY: CRYPT

# PROCEDURE:

**1. Finding Key Length by Friedman Test(Uses the index of coincidence)
2. Finding Key by Chi-squared statistic.
3. Finding Plain text by founded key.**

## 1.Finding Key Length by Friedman Test(Uses the index of coincidence):
*The Index of Coincidence is a statistical technique that gives an indication of how English-like a piece of text is. Generally if text is similar to English, we will have index of coincidence around 0.06. So we will find the index of coincidence considering the different lengths.*

Let us consider example of length 3 of given cipher text

• Divide the cipher text into 3 sequeces where each sequence is encrypted by same letter(Sequence 0 has characters of indexes 0, 3, 6, 9 ..........length of cipher, Sequence 1 has characters of indexes 1, 4, 7, 10 ..........length of cipher, Sequence 2 has characters of indexes 2, 5, 8, 11 ..........length of cipher.

• Now we find the index of coincidence of each sequence by using where f is frequency of correspoding letters and N is length of corresponding sequence

• Now we computer average of index of coincidence of this sequences and if we found the index of coincdence near 0.06 we found the key length

The implementation of above made in python which is available in code file.

by executing it we get length of key 
## LENGTH OF THE KEY IS 5

*For the given cipher text it is found key length as 5.*

## 2.Finding Key by Chi-squared statistic.

Chi-square gives how similar two categorical probability distributions are, if identical chi-squared statistic is 0. If different some higher number will be the result.

• As we found the key length, divide into sets which are encryted by same letter correspondingly, store this in list.

• For each list item now see the chi-square value with deciphering by each  letter (a, b, c............................z)
where E is for normal english text of N letter, how many times corresponding letter occurs C is for orginal text of Nletters, how many times corresponding letter occurs.

• The chi-square with minimum value will be corresponding shift letter for corresponding set. The implementation available in code file.

**KEY IS : crypt**

## 3.Finding Plain Text:

Now decipher the cipher text by using crypt keyword. The implementation available in code file.
