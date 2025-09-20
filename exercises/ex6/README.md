# Exercise 5 - Exercise 6 Description

In this exercise, you will ship a new version of the app instantly after making changes using different techniques.

## Exercise 6.1 Navigate to Main.Page

1. Click here.
<br>![](/exercises/ex5/images/05_01_0010.png)

2.	Insert this line of code.
```abap
response->set_text( |Hello ABAP World! | ). 
```

## Exercise 6.2 Use Visual Editor to make changes

After completing these steps you will have...

1.	Enter this code.
```abap
DATA(lt_params) = request->get_form_fields(  ).
READ TABLE lt_params REFERENCE INTO DATA(lr_params) WITH KEY name = 'cmd'.
  IF sy-subrc = 0.
    response->set_status( i_code = 200
                     i_reason = 'Everything is fine').
    RETURN.
  ENDIF.

```

## Exercise 6.3 Use Text Editor to make changes

## Exercise 6.3 Use Joule Editor to make changes

## Exercise 6.4 Deploy & Test

## Summary

You've now ...

Continue to - [Exercise 5 - Exercise 5 Description](../ex5/README.md) //TODO