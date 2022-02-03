# CryptoAnalysis of a Vigenere cipher
**Paolo Marcoccia<sup>1</sup>**

<sub>1. University of Stavanger, Institutt for Matematikk og Fysikk, Kjølv Egelands hus, 5.etg, E-blokk, 4021 Stavanger, Norway </sub> 

## Introduction ##

In this [notebook](https://github.com/KuZa91/CryptoAnalysis_of_a_Vigenere_cypher/blob/main/VigenereCypherCryptoanalysis.ipynb), we are gonna decypher a message that we know was encrypted by using a [Vigenere cipher](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher). The message that are going to consider is as follows : \
\
_"TUIRDSFOGKYLBVLOORXXRVDPL \
  SHRSBPOCBTTLQPGAOMHMSVONM \
  HDHDNTRTCXRYCJLNHGHTBRIIM \
  HHQWBNHGTIERDAXBHWCZIQGEB \
  RHRQRTKSGXVRZJMIRBXGBXQWT \
  RHGIUELXXGGDIIAOUWIBEVAPR \
  DHQXWEWCTQTHBSFAUHXTLOOLN \
  NWWAMHHOHBAQUPFEVGRAEGIAX \
  DICGLESHTFBHFGXMRJXGGPOGM \
  IDZATWZCJEDESPLIJBPEAGWEE \
  OPOILALREXOSZTPOXZSMANSXM \
  TRATTNWVPMWKOIAASDTGEGPTY \
  OUSRHUORHMAUHJIAJOXGIQOHM \
  AWSRHUQQXEMHSIBNJCCPEGBTL \
  DDMBKLLRTYEQRTWBHWYBNJGJL \
  ERTBBLLHPKYICGVEWCRKAFYSH \
  WQCCMHHGINDHBIFOYSBXNWHWX \
  CUIHAIQUDYTKSRHUQHTKRHJDE"_ \
\  
We are gonna start our analysis by trying to find the lenght of the key, which is probably the most important step in order to properly solve a Vigenere Cipher.
Knowing the lenght of the key, allow us to decompose the original encoded text in a subset of $n$ messages encoded trough a common [Caesar Cipher](https://en.wikipedia.org/wiki/Caesar_cipher), where $n$ is equal to the lenght of the key. 
