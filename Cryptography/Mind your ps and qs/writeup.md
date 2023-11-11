# Mind your Ps and Qs
## Description
In RSA, a small e value can be problematic, but what about N? Can you decrypt this? values
## Hint
Bits are expensive, I used only a little bit over 100 to save money
![Screenshot 2023-11-11 111603](https://github.com/MahikaWakankar/Cryptonite_taskphase/assets/148598677/030929cf-3da1-4079-a271-3ffaaa60b518)
## Solution
Decrypt my super sick RSA:
c: 964354128913912393938480857590969826308054462950561875638492039363373779803642185
n: 1584586296183412107468474423529992275940096154074798537916936609523894209759157543
e: 65537
from RSA we know that n is product of 2 large prime numbers(p,q), using factordb.com [factordb](http://factordb.com/index.php?query=1584586296183412107468474423529992275940096154074798537916936609523894209759157543) I found the 
needed numbers.
![Screenshot 2023-11-11 112457](https://github.com/MahikaWakankar/Cryptonite_taskphase/assets/148598677/69606fbd-baeb-4a66-82f9-a4d9f51a421c)
p= 2434792384523484381583634042478415057961
q=650809615742055581459820253356987396346063
using rsa decoder dcode.fr [dCode](https://www.dcode.fr/rsa-cipher)
![Screenshot 2023-11-11 113011](https://github.com/MahikaWakankar/Cryptonite_taskphase/assets/148598677/c17373e2-b29b-4e2a-aee4-90ba6f4c3a2f)
hence flag is picoCTF{sma11_N_n0_g0od_73918962}
