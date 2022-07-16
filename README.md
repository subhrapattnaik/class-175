# class-175
AR CHEMICAL COMPOUNDS



https://curriculum.whitehatjr.com/PRO+Asset/PRO+175+Output+Ref-AR+Chemistry.mp4




Now we will take two arrays (A & B) for
compounds which can be formed with
just two elements (like NaCl, KCl):
● One with elements that can lose
electrons to form compounds that
are elements like Na (Sodium), K
(Potassium), Li (Lithium) and H
(Hydrogen).



● And another one with elements
that need electrons to form
compounds that are elements like
F (Fluorine), Cl (Chlorine), Br
(Bromine) and I (Iodine).


we can
now calculate the distance.
For this we are going to use the Three.js
method distanceTo().
For example elA.distanceTo(elB) will
give distance between elA and elB,
where elA and elB are position vectors
as Three.js objects.



Now we will call this
function(getDistance()) to get the
distance between two barcode markers:
If it can be formed then we’ll show the
compound using all
If the compound cannot be formed then
we'll show the text
message-”Compound will not form…”
Can you tell how we should write this?
To do this we will write inside the .tick()
function of the component. The .tick()
functions is called continuously:
● Check if elementsArray length is
greater than zero.
● Select “message-text” entity.
● Call getCompund()



● If elementsArray length is equal
to two:
○ Find distance between two
markers using
getDistance() function.
○ If distance is less than
1.25:
■ Check if the
compound is
defined and call
showCompund(),
which sets the
visible attribute for
compounds to true
and for elements to
false.
○ Else show message-text.
