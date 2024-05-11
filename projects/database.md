---
layout: project
type: project
image: img/c-image.png
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

In ICS 212 I programmed a C++ database. The database is built upon a linked-list framework. This database contains many functions which allow the adding, removal, searching, and printing of records.  Upon termination of the program, the project will save the remaining records into a txt file. This allows the records to be saved and accessed when the program is launched again. The project also contains a dynamic text-based user interface which can handle a variety of proper and improper inputs and allow the user to input and access data.

This project showcases my ability to facilitate basic back-end database functionality. I also employed careful planning to properly execute the proper storage and access of the records. Since the linked-list structure is coded in C, I did not have a library of pre-built data structures to work with. This meant it was easy to cause segmentation faults if the data was allocated improperly.

The concept of this database is from the ICS 212 instructor and material. However, all code was planned and coded by me. Here is a snippet of code that implements the findRecord function which searches through the database looking for records that have user-specified account number:

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

Source: <a href="https://github.com/AdrielWhite/c-project-database"><i class="large github icon "></i>C++ Database on github</a>
