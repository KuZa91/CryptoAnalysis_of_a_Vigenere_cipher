# CryptoAnalysis of a Vigenere cipher
**Paolo Marcoccia<sup>1</sup>**

<sub>1. University of Stavanger, Institutt for Matematikk og Fysikk, Kjølv Egelands hus, 5.etg, E-blokk, 4021 Stavanger, Norway </sub> 

## Introduction ##

In this [notebook](https://github.com/KuZa91/CryptoAnalysis_of_a_Vigenere_cipher/blob/main/VigenereCipherCryptoanalysis.ipynb), we are gonna decipher a message that we know was encrypted by using a [Vigenere cipher](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher). The message that are going to consider is as follows : \
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
The Caesar ciphers, can be easily decrypted trough [brute force](https://en.wikipedia.org/wiki/Brute-force_attack), as each subset would only have 26 possible values for the key value, however, in our analysis we are gonna implement a [frequentist analysis](https://en.wikipedia.org/wiki/Frequentist_inference) in order to properly estimate the value of the key for the various subsets.
The [notebook](https://github.com/KuZa91/CryptoAnalysis_of_a_Vigenere_cipher/blob/main/VigenereCipherCryptoanalysis.ipynb) procedure, can be easily used to decrypt any other message encrypted trough use of a Vigenere cipher, however, as some of the conjectures used in this approach can lead to misleading results, human supervision through the steps of the analysis is still greatly suggested in spite of considering the [notebook](https://github.com/KuZa91/CryptoAnalysis_of_a_Vigenere_cipher/blob/main/VigenereCipherCryptoanalysis.ipynb) as an automatic solver !

## Analysis Details ##
