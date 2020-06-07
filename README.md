## AAL(AN) - **A**n **A**wful **L**anguage **A**midst **N**ot bad ones
AALAN, AAL for short, is a hypothetical, for now, language designed by a lowly JavaScript developer and a C purist.


## Little Bit Of Reading

### General Premise:
Take some of the nice things about JavaScript (easy async, non-dependent function arguments)
whilst keeping more traditional stance on typing and other far superiour parts of your average lang.
All this whilst keeping it beginner (not just human) readable, once again on the level of js, we aren't
stooping to Python... yet.

### Basics:
**Variables:**

Creating variables is well, the same as everywhere else, just with ':' as the operator. 
E.g: ` int age: 12; `. The ':' works well, as if you were writing a list, whilst also 
providing separation in symbols to the equals operator '='; 

**Arrays:**

Something I quite dislike about Java is it's myriad of Array like data types.
Arrays, Lists, ArrayLists, it's just a mess. In AAL, we're hoping for one, or at least
as few array types as we can get away with, more like JS.

## A sample:

```

const rand: import(random); #No quotes because of course

fn main(string[] args) {

    ##
    Le settings
    ##

    # You don't need to provide the 'string[] args' unless you plan on using them.

    string token: ""; # String's are implimented by default, as with numbers.

    int length: 10;
    bool uppercase: true; # Unlike cring java you use bool, not boolean. 

    string[] alphabet = "abcdefghijklmnopqrstuvwxyz1234567890".split("");

    ##
    Le program 
    ##

    if(uppercase) alphabet += alphabet.matches("[A-z]").join("").toUpperCase().split("");

    for(int i: 0; i < length; i++) {

        token += alphabet[rand.range(0, alphabet.length + 1)]; # Using += to concat arrays!

    }

}
```
