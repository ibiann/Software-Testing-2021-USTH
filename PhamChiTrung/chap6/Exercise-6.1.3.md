# Answer the following questions:

![image](https://raw.githubusercontent.com/ibiann/Software-Testing-2021-USTH/main/PhamChiTrung/Img%206.1.3.PNG)
```
a. “Location of element in list” fails the disjointness property: 
    - If the element is first entry in list, Block 1 and Block 2 will be jointed.
b. “Location of element in list” fails the completeness property:
    - If the element is last entry, it can either be null or not in the list.
c. Supply one or more new partitions that capture the intent of “Location of element in list” 
but do not suffer from completeness or disjointness problems:
    - Block1: element is not null but it still in the list.
    - Block2: element is either not null or not in the list.
    - Block3: element is null.
    
```
