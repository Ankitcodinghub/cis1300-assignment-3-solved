# cis1300-assignment-3-solved
**TO GET THIS SOLUTION VISIT:** [CIS1300 Assignment 3 Solved](https://www.ankitcodinghub.com/product/cis1300-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115304&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CIS1300 Assignment 3  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Introduction

Welcome to Part 2 of Assignment 3. The challenge in this part of the assignment (worth 15% of the total grade) is to use 2 data sets at the same time to do some comparisons.

Program 2: babiesQuery.c

Source Code Files

Your program will have the name babiesQuery.c and you will also use the header file babies.h. In babies.h, you will find the definitions that you will need for your program. It has the following contents:

/* Defines */

#define MAXLENGTH 20 #define ROWS 200

/* Struct definitions */ struct pNames { int year; int rank[ROWS];

char maleName[ROWS][MAXLENGTH]; int maleNumber[ROWS]; char femaleName[ROWS][MAXLENGTH]; int femaleNumber[ROWS];

};

/* Function definitions */

int removeCommas ( char * );

Functionality

The program will accomplish the following tasks:

• Read in all the information about multiple decades that the user requests, e.g. if the user wants to compare the 1880’s to the 1980’s then you must read in the file

1880Names.txt and 1980Names.txt.

o You can also decide to load all of the Names files into your program before you ask the user which decades they want.

• As before you will store this information in the structure given to you in the header file babies.h.

o Once again you have a choice – you can create two structures, for example

struct pNames decade1; struct pNames decade2;

o Or you can store the Names data in an array of type struct pNames struct pNames decades[num] where num is from 2 to 14.

• You will then ask your user questions that will allow you to find the following types of information: o For a given rank, what is the (male, female, both) name , e.g. in the 1880’s and the 1980’s, the female name of rank 1 is Mary in 1880 and Jessica for 1980. o The top 10 names (male and female) for the given decades that are the same.

o Given a name (female, male or both), find the rank for the given decades.

Question Script

The questioning of the user must follow the following script:

$ ./babiesQuery

What 2 decades do you want to look at? [1880 to 2010]: 1880 1980

Would you like to see a rank, search for a name, or see the top 10? [rank, search, top]: rank Now there are three different paths for questioning:

Path 1: rank

What rank do you wish to see? [1-200]: 2

Would you like to see the male (0), female (1), or both (2) name(s)? [0-2]: 2

Rank 2: 1880: Male: William (84881) and Female: Anna (38159)

1980: Male: Christopher (554984) and Female: Jennifer (440871) if response is 2

Rank 2: 1880 Male: William (84881)

1980 Male: Christopher (554984) if response is 0

Rank 2: 1880: Female: Anna (38159)

1980: Female: Jennifer (440871) if response is 1 Path 2: search

What name do you want to search for? [case sensitive]: Emily

Do you wish to search male (0), female (1), or both (2) name? [0-2]: 1

In 1880, the female name Emily is ranked 91 with a count of 3368 and

In 1980, the female name Emily is ranked 25 with a count of 131755. if response is 1

In 1880, the male name Emily is not ranked and

In 1980, the male name Emily is not ranked. if response is 0 and the name is not found In 1880, the female name Emily is ranked 91 with a count of 3368 and the male name Emily is not ranked

And in 1980, the female name Emily is ranked 25 with a count of 131755 and the male name

Emily is not ranked. if response is 2 – the female name will always go first even if it is not found Path 3: top

Male names that appear in both 1880 and 1980 Top Tens: John, James, Joseph, Robert

Female names that appear in both1880 and 1980 Top Tens: Elizabeth

After the answer has been presented to the user the following questions will be asked:

Do you want to ask another question about 1880 and 1980? [Y or N]: Y

If the response is Y then return to the question “Would you like to see a rank, search for a name, or see the top 10? [rank, search, top]: ”.

If the response is N then ask the following:

Would you like to select other decades? [Y or N]: Y

If the response is Y then return to the question “What 2 decades do you want to look at? [1880 to 2010]: “.

If the response is N then terminate the program with the message: Thank you for using babiesQuery.

Error Checking

Error checking is extremely important when users are giving information to the program. For all of the questions asked of the user, you must check that the input is exactly what was asked for. Let us examine the various responses requested from the user:

• What 2 decades do you want to look at? [1880 to 2010]:

o The response must be two of 1880, 1890, 1900, 1910, 1920, 1930, 1940, 1950, 1960, 1970, 1980, 1990, 2000, or 2010, separated by at least one space. No other numbers are acceptable. Both numbers cannot be the same.

• Would you like to see a rank, search for a name, or see the top 10? [rank, search, top]:

o The user must type in rank or search or top – all lower case and all spelled correctly and in full.

• What rank do you wish to see? [1-200]:

o Only numbers between 1 and 200 are acceptable.

• Would you like to see the male (0), female (1), or both (2) name(s)? [0-2]:

o Only the numbers 0, 1, or 2 are acceptable.

• What name do you want to search for? [case sensitive]:

o The requested string is to be treated as case sensitive (names in the files have the first letter in upper case and the rest in lower case). If they enter a name that does not follow this format, the string is to be accepted as input but the program is to do nothing to “fix” the case and thus the request will fail.

• Do you wish to search male (0), female (1), or both (2) name? [0-2]: o Only the numbers 0, 1, or 2 are acceptable.

• Do you want to ask another question about 1880 and 1980? [Y or N]:

o The user is to respond with a single letter, either Y or N but it is to be treated in a case insensitive manner; i.e. y and n are acceptable.

• Would you like to select other decades? [Y or N]:

o The user is to respond with a single letter, either Y or N but it is to be treated in a case insensitive manner; i.e. y and n are acceptable.

If the user makes an error, the program is to give an error message and then repeat the question. The following are the error messages that are to be given:

• What 2 decades do you want to look at? [1880 to 2010]:

o Acceptable decades are 1880, 1890, 1900, 1910, 1920, 1930, 1940, 1950, 1960, 1970, 1980, 1990, 2000, or 2010. No other numbers are acceptable. You must enter 2 acceptable decades separated by a least one space.

• Would you like to see a rank, search for a name, or see the top 10? [rank, search, top]:

o Please type in rank, search, or top exactly as requested.

• What rank do you wish to see? [1-200]:

o Only numbers between 1 and 200 are acceptable.

• Would you like to see the male (0), female (1), or both (2) name(s)? [0-2]:

o Only the numbers 0, 1, or 2 are acceptable.

• What name do you want to search for? [case sensitive]:

o No error message is needed for this question.

• Do you wish to search male (0), female (1), or both (2) name? [0-2]: o Only the numbers 0, 1, or 2 are acceptable.

• Do you want to ask another question about 1880 and 1980? [Y or N]:

o Only the single characters Y or N are acceptable. • Would you like to select other decades? [Y or N]:

o Only the single characters Y or N are acceptable.
