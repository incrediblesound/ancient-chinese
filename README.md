Ancient Chinese
===============
I thought I might share my knowledge of Ancient Chinese with the git world for two reasons:    
1) Github is a vast, awesome repository of knowledge full of amazing people    
2) Ancient Chines is a vast, awesome repository of knowledge full of amazing people    

Given these two highly distinct factors in combination with my desire to not waste an expensive master's degree the decision to act was easily made. As I started to work I realized how wasteful it is to write a highly organized book without any markup whatsoever. Thusly I decided to distinguish the various parts of the book using xml, and to use JavaScript to format the content. Seeing the result I was greatly pleased, and wondered why anyone would ever write a book without using markup to make it computer readable.   

##Section reference
Each book is contained in its own file and is wrapped in a "book" tag.    
Each book and each section/chapter of each book has a "title" tag.
Each section has a "cn" original chinese, "each" word for word translation, "en" english translation, and "notes" commentary.

##Important Note
The word for word translation of each line is stored in an array of JS objects. The "notes" section for each line is an array of strings each of which references an index of that array, thusly "(1) This is my favorite character" refers to the second item in the word for word translation. I will occasionally reference other things like "(en) My translation is really bad" references the english translation for that line.
