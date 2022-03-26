- :smiling_face_with_three_hearts: Working on [`The Aya Prover`](https://github.com/aya-prover/aya-dev).
- :fire: Trying to build a new projection on social media.
- Legacy projection: https://github.com/zaoqi

Pronouns: She/Her

```racket
(define me ((lambda (x) (x x)) (lambda (x) (x x))))
(define (me? x) (if (me? x) #f #t))
(define (generate-me) (if (halt? generate-me) ((lambda (x) (x x)) (lambda (x) (x x))) 'me))
```
```idris
Me: Type
Me = Me -> Void
me: Me
me x = x x
```
```haskell
import Data.Void
data Me = Me (Me -> Void)
me = Me (\me -> case me of (Me x) -> x me)
```
