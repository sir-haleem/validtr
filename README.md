# validtr
A simple form field validation plugin with jQuery support

Initialized with _v or validtr

var regForm = _v("#regForm");

_v object takes a parameter is which the form id attribute to be validated.

The overloaded version of the _v object takes an object as an additional parameter.

var regForm = _v("#regForm", {
                 "textfield",
                 "password",
                 " email",
                 "checkbox",
                 " radiobutton",
                 "terms"
             });

You can also call the addFields method and pass in the object same as above.

regForm.addFields({
                 "textfield",
                 "password",
                 " email",
                 "checkbox",
                 " radiobutton",
                 "terms"
                });

What the above does is to tell validtr the fields that you are working with for this very instantiation.

To see what happens :

console.log(regForm);

Before and after adding fields.

It will log arrays corresponding to the parameters you've passed and the arrays will contain jQuery objects of the Dom elements of the fields that are in the form id that you've passed earlier.

You can have more than one checkbox and radiobuttoj

Now validating text fields:

regForm.validateTextfield();
