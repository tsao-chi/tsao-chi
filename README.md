```racket
(define me ((lambda (x) (x x)) (lambda (x) (x x))))
(define (me? x) (if (me? x) #f #t))
(define (generate-me) (if (halt? generate-me) ((lambda (x) (x x)) (lambda (x) (x x))) 'me))
```
