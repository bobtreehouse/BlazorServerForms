# BlazorServerForms
test work using Blazor Server and specifically the Edit Form "@Model" versus "@EditContext" Validation 

This is the index page of a test BlazorServer project used to provide a sign-up form. 
The EditForm uses the "@model" for validation. The custom validation messages will display for individual field 
errors however the entire form will NOT submit unless it is field in by the user with no errors and in the first attempt. 
It might require some kind of "State Has Changed" method for the form to refresh as an incorrect entry also throws an error 
on the whole page.


The "indexEditContext" razor page uses the "EditForm EditContext" approach which seems to better handle an InValid Submit 
however it Blocks ALL Submits from passing to the database. 
