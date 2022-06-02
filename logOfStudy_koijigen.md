

## 2206022230

Passed first test "sumOfSquares".
It was done by following :

1. create Lecture1.hs.bak from copying Lecture1.hs.
2. edit Lecture1.hs's function "sumOfSquares" to pass test.
3. execute command : `cabal run exercises-test --enable-tests -- -m "sumOfSquares"`

## 2206022200

I did things bellow:

1. Falked this repository and opened it by gitpod.
2. on gitpod, install some extension suggested by gitpod IDE.
3. edit gitpod permission at "https://gitpod.io/integrations". the steps is following : click "GitHub" row's pulldown (it seems to see "・・・"), and click "Edit Permissions" from pulldown, and check "public_repo" and push "Update Permissions" button.
4. create file named "testpush" on gitpod IDE.
5. Open "Source Control", and commit change and push "Sync" button on gitpod IDE.
6. git push is successed. it is verified by to see remote repository on github.com.

---

And I followed this repository README.md's section "### Cabal".
In particular, It's following (the all following steps did on terminal at gitpod IDE) : 

1. execute following command : `make build` . 
2. execute following command : `make test-lecture1` .
3. execute following command : `cabal run exercises-test --enable-tests -- -m "strSum"` .

step 3's output is following (and it was right responce) :

```output

Resolving dependencies...
Build profile: -w ghc-8.10.7 -O1
In order, the following will be built (use -v for more details):
 - exercises-0.0.0.0 (lib) (file src/Lecture1.hs changed)
 - exercises-0.0.0.0 (test:exercises-test) (dependency rebuilt)
Preprocessing library for exercises-0.0.0.0..
Building library for exercises-0.0.0.0..
[4 of 4] Compiling Lecture1

src/Lecture1.hs:43:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature:
      makeSnippet :: Int -> [Char] -> [Char]
   |
43 | makeSnippet limit text = take limit ("Description: " ++ text) ++ "..."
   | ^^^^^^^^^^^

src/Lecture1.hs:58:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature:
      sumOfSquares :: Double -> Double -> Double
   |
58 | sumOfSquares x y = (powerDouble x 2) + (powerDouble y 2)
   | ^^^^^^^^^^^^

src/Lecture1.hs:70:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature: lastDigit :: p -> a
   |
70 | lastDigit n = error "lastDigit: Not implemented!"
   | ^^^^^^^^^

src/Lecture1.hs:70:11: warning: [-Wunused-matches]
    Defined but not used: ‘n’
   |
70 | lastDigit n = error "lastDigit: Not implemented!"
   |           ^

src/Lecture1.hs:84:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature:
      minmax :: p1 -> p2 -> p3 -> a
   |
84 | minmax x y z = error "TODO"
   | ^^^^^^

src/Lecture1.hs:84:8: warning: [-Wunused-matches]
    Defined but not used: ‘x’
   |
84 | minmax x y z = error "TODO"
   |        ^

src/Lecture1.hs:84:10: warning: [-Wunused-matches]
    Defined but not used: ‘y’
   |
84 | minmax x y z = error "TODO"
   |          ^

src/Lecture1.hs:84:12: warning: [-Wunused-matches]
    Defined but not used: ‘z’
   |
84 | minmax x y z = error "TODO"
   |            ^

src/Lecture1.hs:101:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature:
      subString :: p1 -> p2 -> p3 -> a
    |
101 | subString start end str = error "TODO"
    | ^^^^^^^^^

src/Lecture1.hs:101:11: warning: [-Wunused-matches]
    Defined but not used: ‘start’
    |
101 | subString start end str = error "TODO"
    |           ^^^^^

src/Lecture1.hs:101:17: warning: [-Wunused-matches]
    Defined but not used: ‘end’
    |
101 | subString start end str = error "TODO"
    |                 ^^^

src/Lecture1.hs:101:21: warning: [-Wunused-matches]
    Defined but not used: ‘str’
    |
101 | subString start end str = error "TODO"
    |                     ^^^

src/Lecture1.hs:111:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature: strSum :: p -> a
    |
111 | strSum str = error "TODO"
    | ^^^^^^

src/Lecture1.hs:111:8: warning: [-Wunused-matches]
    Defined but not used: ‘str’
    |
111 | strSum str = error "TODO"
    |        ^^^

src/Lecture1.hs:126:1: warning: [-Wmissing-signatures]
    Top-level binding with no type signature:
      lowerAndGreater :: p1 -> p2 -> a
    |
126 | lowerAndGreater n list = error "TODO"
    | ^^^^^^^^^^^^^^^

src/Lecture1.hs:126:17: warning: [-Wunused-matches]
    Defined but not used: ‘n’
    |
126 | lowerAndGreater n list = error "TODO"
    |                 ^

src/Lecture1.hs:126:19: warning: [-Wunused-matches]
    Defined but not used: ‘list’
    |
126 | lowerAndGreater n list = error "TODO"
    |                   ^^^^
Preprocessing test suite 'exercises-test' for exercises-0.0.0.0..
Building test suite 'exercises-test' for exercises-0.0.0.0..
[1 of 5] Compiling Test.Lecture1 [Lecture1 changed]
[5 of 5] Compiling Main [Test.Lecture1 changed]
Linking /workspace/exercises/dist-newstyle/build/x86_64-linux/ghc-8.10.7/exercises-0.0.0.0/t/exercises-test/build/exercises-test/exercises-test ...

Tests
  Lecture 1
    strSum
      Empty string [✘]
      Single positive number [✘]
      Single negative number [✘]
      Spaced number [✘]
      Only positive [✘]
      Only negative [✘]
      Mix [✘]

Failures:

  src/Lecture1.hs:111:14: 
  1) Tests, Lecture 1, strSum, Empty string
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Empty string/"

  src/Lecture1.hs:111:14: 
  2) Tests, Lecture 1, strSum, Single positive number
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Single positive number/"

  src/Lecture1.hs:111:14: 
  3) Tests, Lecture 1, strSum, Single negative number
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Single negative number/"

  src/Lecture1.hs:111:14: 
  4) Tests, Lecture 1, strSum, Spaced number
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Spaced number/"

  src/Lecture1.hs:111:14: 
  5) Tests, Lecture 1, strSum, Only positive
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Only positive/"

  src/Lecture1.hs:111:14: 
  6) Tests, Lecture 1, strSum, Only negative
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Only negative/"

  src/Lecture1.hs:111:14: 
  7) Tests, Lecture 1, strSum, Mix
       uncaught exception: ErrorCall
       TODO
       CallStack (from HasCallStack):
         error, called at src/Lecture1.hs:111:14 in exercises-0.0.0.0-inplace:Lecture1

  To rerun use: --match "/Tests/Lecture 1/strSum/Mix/"

Randomized with seed 1311969434

Finished in 0.0037 seconds
7 examples, 7 failures

```

---

So, I finished ready to start to study my first haskell lectures "exercise". 
