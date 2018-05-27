# Affine-Crypto-System-Sage

How affine crypto system works:
The form of the affine cipher is E(x) = [a.x + b]mod(m). Here, a and b are
integers (keys); x is the plaintext number to be encrypted. m is 26, because of the use
of a 26 character alphabet in English Alphabet.
Similarly , the decryption form is D(y) = [a -1 .(y-b)]mod(m). a -1 is the inverse of a.

For instance, let us encrypt the plain text “EMRE OVUNC”, using the key a=3,
b=8.
A=AffineCryptosystem(AlphabeticStrings())
P=A.encoding("EmreOVUNC")
a,b=(3,8)
C=A.enciphering(a,b,P)
A.deciphering(a,b,C)==P
print C
