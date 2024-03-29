# chooser-lang
music lang test


Bellingham, M., Holland, S. and Mulholland, P. (2017) Choosers: designing a highly expressive algorithmic music composition system for non-programmers. 2nd Conference on Computer Simulation of Musical Creativity – 11th to 13th September 2017, The Open University, Milton Keynes, UK. http://hdl.handle.net/2436/621151.  http://oro.open.ac.uk/57761/1/Matt%20Bellingham%20PPIG%202018%20AsSUbmitted%20.pdf

Bellingham, Matt; Holland, Simon and Mulholland, Paul (2018). Choosers: The design and evaluation of a visual algorithmic music composition language for non-programmers. In: Proceedings of 29th Annual Workshop of the Psychology of Programming Interest Group - PPIG 2018.
http://oro.open.ac.uk/53946/1/Bellingham%20et%20al.%202017%20-%20Choosers%20-%20designing%20a%20highly%20expressive%20algorithmic%20music%20composition%20system%20for%20non-programmers.pdf


```
;; sample : sample-file-path -> audio
;; e.g. (sample "melody1.wav")

;; sequence : sample ...+ ; -> audio

(sequence (sample "melody1.wav") (sample "melody2.wav") (sample "melody1.wav"))

(define m1 (sample "melody1.wav"))
(define m2 (sample "melody2.wav"))
(define m3 (sequence m1 m2 m1))

 -> audio
(lane sample weight status)

;; chooser : number-of-lanes-to-play lane ...+  [time bars stop-type; -> audio 
;; number-of-lanes-to-play ; natural-number
;; lane : sample weight status 
;; weight : (or number #t)
;; status : (or 'once '↺' repeat 
;; stop-type ; (or '>' hard-stop 'X>' soft-stop)

(define melody
 (chooser 2 
  (m1  1   #t)
  (m2  1   #t)
  (m3  1   #t)
  (time 16bars > )
  ))
  



```
