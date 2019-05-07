## Secure communications before computers

From the early days until radio was invented, people had few options to send a message privately:
- use postal service and hope for the best that your envelope won't be open 
- send a person with your message and hope he won't be intercepted nor he will defect you
- use dove post

So if you sent plain text, there were chances the contents of your private message would be known to an adversary.
As a result, alphabetical ciphers were invented, for example
- Ceasar cipher of ROT13
- Vigenere cipher

It seems Vigenere cipher was robust enough for its epoch. Much later an algorithm was found that breaks it 
after observing a long enough cipher text. Both the plain text and the key are found.

In 1917 it was proven that to have perfect secrecy (adversay learns nothing from cipher text) the private key knows to 
the sender and the receiver must be at least as long as the message itself. To send the next message, you use the next 
part of the key and nevr reuse it.
So, if you calculate cipher text = plain text text *xor* key
(addition modulo 2 for binary values) you cipher is perfectly secure. That is a One Time Pad or Vernam cipher.

Later on, as radio was invented, another crypto marvel was designed: 
- the Enigma machine.

Its versions were used by Germans in WWII. It is an electromechanical typewriter with a complex algo in it and a key schedule
(list of keys).
The ciphertext was transmitted via radio as Morse code.
The allies failed to break it until they captured the machine itself. 
Around that time the first prototype of a computer was built for this very purpose. Adam Turing took part in that project.

The latest version of Enigma and long key schedules were used on submarines as they operated in the sea for a long time. 
If the Germans found out the machine was captured they changed the key schedule. 

Enigma and the key schedule was so precious for the Allies that at least once an English warship defeated a German submarine, it surfaced, 
officers covertly grabbed Enigma and the key schedule from it and subsequently the warship sank the submarine with all its crew taking no 
prisoners of war. 
Noboby had to know that Enigma and the key schedue were stolen. 
As a resut this key schedule was in use for a while and the messages were succesfully decripted.

Closer to the end of the WWII after significant efforts the Allies managed to break the cipher having obtained just the latest 
version of Enigma.
 
