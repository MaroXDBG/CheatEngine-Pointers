# CheatEngine-Pointers

The Other Challenges were quite easy because they are the same concept of scanning the value in memory and applying changes.


But the challenge is how to deal with a programme or a game that is constantly changing the adresse upon runtime 

Or an Application which uses ASLR (Address space layout randomization)

That when cheat engine offers Pointer Scanning

Which is the concept of finding the pointer that holds the adress of the value we want to find so that even if the adress is changed 

the pointer finds it back

# Here's the challenge :

![enter image description here](https://github.com/MaroXDBG/CheatEngine-Pointers/blob/main/screens/main.PNG)


# I will leave this Challenge to My Colleague **@NassimMs** to Explain downwords 

----------------------------------------------------------------------------------------------------------------------------------

>> *NassimMS* : So if we approach the challenge the usual way like the tutorial covered by MaroXDBG in finding values we find 

our first adress which is : 

![screen](https://github.com/NassimMs/CheatEngine-Pointers/blob/main/screens/2.PNG)

But it is only a normal adress which will get change after the program exit so we need to find the pointer holding the adress

We can do that the manual way or by using Cheat Engine Pointer Scanning Function.

I will use the manual way to Explain how it works.

So if we right click the adress and check what instructions ( Assembly instruction ) that access the adress for Reading/Writing

![screen](https://github.com/NassimMs/CheatEngine-Pointers/blob/main/screens/3.PNG)

There is this interessting instruction that i highlighted which shows that [edx] which is a register but when it is between brackets it means

that it is an adress.. perhaps it is the one pointing to the already found adress ?

# Examining the EDX Register 

![screen](https://github.com/NassimMs/CheatEngine-Pointers/blob/main/screens/4.PNG)

if we search for that adress in cheat engine to find the pointer holding that adress 

![screen](https://github.com/NassimMs/CheatEngine-Pointers/blob/main/screens/5.PNG)

We can see in the highlighted area that we found a base adress which start by the ***Process name / Module Name***


Thanks to MaroXDBG for the invitation




