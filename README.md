# chooser-lang
music lang test


Bellingham, M., Holland, S. and Mulholland, P. (2017) ‘Choosers: designing a highly expressive algorithmic music composition system for non-programmers’, 2nd Conference on Computer Simulation of Musical Creativity. 

http://oro.open.ac.uk/57761/1/Matt%20Bellingham%20PPIG%202018%20AsSUbmitted%20.pdf

Bellingham, Matt; Holland, Simon and Mulholland, Paul (2018). Choosers: The design and evaluation of a visual algorithmic music composition language for non-programmers. In: Proceedings of 29th Annual Workshop of the Psychology of Programming Interest Group - PPIG 2018.
http://oro.open.ac.uk/53946/1/Bellingham%20et%20al.%202017%20-%20Choosers%20-%20designing%20a%20highly%20expressive%20algorithmic%20music%20composition%20system%20for%20non-programmers.pdf



;; sample : sample-file-path -> audio
;; e.g. (sample "melody1.wav")

;; sequence : sample ...+ ; -> audio
(sequence (sample "melody1.wav") (sample "melody2.wav") (sample "melody1.wav"))

;; chooser : 
