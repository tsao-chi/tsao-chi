```racket
(define me ((lambda (x) (x x)) (lambda (x) (x x))))
(define (me? x) (if (me? x) #f #t))
(define (generate-me) (if (halt? generate-me) ((lambda (x) (x x)) (lambda (x) (x x))) 'me))
```
```idris
Me: Type
Me = Me -> _|_
me: Me
me x = x x
```
