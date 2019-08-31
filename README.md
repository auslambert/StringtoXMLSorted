# StringtoXMLSorted
A remake of String to XML that stores data pairs, with optional sorting by description.

Creates an Xml file with data pairs that are editable with a standard XML editor such as Notepad for XML i na location of your choice.
Each data pair contains a description/data element.

in the SIMPL folder is an example program that contains example SIMP code plus the required S+ module.
The module defines 25 data pairs but the S# doesn't care, only writing those elements that have data in either the description
or data fields. You can change the number of elements by altering the line in the S+ file:
#DEFINE_CONSTANT ASIZE 25 and recompiling.

the example program is a cut down version form a live project that also stored Phone number pairs.
All you need to do is copy the folders 'Tuner Favorites' and 'Tuner recall' and F9 rename 'tuner' to 'ATC' and add a couple of
signals to OR's in the common popup logic to have any number of XML files.

The example program also contains a couple of utility modules that do handy things like a timed popup and an SMV filter that
reacts to any change except a predefined 'do nothing' value, like 0.
And a module that pulses digits (like IR files) when given a text string like a phone or channel number.

Enjoy!
