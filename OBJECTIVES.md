Custom Shift Cipher Module

Go through the process of setting up a blank Drupal site. Once you've built a development environment create a custom module which encrypts user input using a Shift Cipher.

Requirements:

    It should present a custom form with 3 text inputs. We want you to use text inputs rather than radio buttons or menus so that you can practice validation.
    One input should be a shift value, one should be a direction, and the third should be the phrase to be encrypted.
    Then you should redirect to a second page to show the result - the encoded phrase. Here are a couple examples of input and output.

1. Input:
Shift value = 3
Shift direction = right
Phrase = "hello"

Output:
"khoor"

2. Input:
Shift value = 1
Shift direction = left
Phrase = "hi there!"

Output:
"gh sgdqd!"

    The shift value is the number of places to shift each letter over.
    If the shift direction is "right" then you will add the shift value. For example: "a" with a shift value of 1 and a direction of right would become "b". A shift direction of "left" with a shift value of 1 would turn "b" into "a".
    If the shift amount takes you over the bounds of the alphabet then cycle back to the beginning. For example: a shift value of 3 with the direction of right would turn "z" into "c".
    Any spaces or punctuation in the input phrase should be ignored and reproduced in the final result without being shifted.
    Your final result should be in all lowercase.

Be sure to validate all input before calculating the result. Here are the validation rules:

    The shift value must be a positive integer
    The shift direction must be either "left" or "right".
    The only special characters that should be allowed in your input phrase are spaces and punctuation.

Objectives

Here are the objectives the teacher will use to review your code with you:

    Does your module present a form with the correct fields?
    Are you performing all necessary user input validation?
    Is the input phrase correctly encrypted and displayed on the final page?
    Did you submit a project repository containing the cipher module, regularly make Git commits and include a clear and tidy readme?
    Is the code clear and easy to follow, with clean indentation and descriptive variable names?
    Does the project demonstrate an understanding of this week's concepts? If prompted, can you discuss your code with an instructor using the correct terminology?
    Is the project in a polished, portfolio-quality state?
    Was the required functionality in place before the 5:00pm Friday deadline?
