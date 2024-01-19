---
layout: project
type: project
image: img/c++.png
title: "C++ Database"
date: 2023
published: true
labels:
  - C
  - C++
  - GitHub
summary: "A database which allows records to be created, deleted, searched for and saves the data in a txt file."
---

<img class="img-fluid" src="https://github.com/AdrielWhite/AdrielWhite.github.io/blob/main/img/Screenshot%202024-01-18%20163501.png?raw=true">

Cotton is a horror-style text-based adventure game I developed using the functions and macros built from The Wizard's Game in [Conrad Barski's Land of Lisp](http://landoflisp.com/). Slightly more interesting and convoluted! (It is not that scary.)

To give you a flavor of the game, here is an excerpt from one run:

<hr>

```
int llist::findRecord(int uaccountno)
{
    struct record * current;
    int retVal;

    #ifdef DEBUGMODE
    cout << "\n/* DEBUG ** findRecord() */";
    cout << "\n/* DEBUG ** accountno = " << uaccountno << " */\n";
    #endif

    current = this->start;
    retVal = -1;
    while (current != NULL)
    {
        if ((*current).accountno == uaccountno)
        {
            if (retVal < 0)
            {
                retVal = 1;
            }
            else
            {
                retVal++;
            }
            cout << "\naccountno: " << (*current).accountno;
            cout << "\nname: " << (*current).name;
            cout << "address: \n" << (*current).address;
        }
        current = (*current).next;
    }
    return retVal;
}
```


<hr>

Source: <a href="https://github.com/jogarces/ics-313-text-game"><i class="large github icon "></i>jogarces/ics-313-text-game</a>
