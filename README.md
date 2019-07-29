# BugsAndTheirSolutions
I will be collect here bugs from android apps and write solutions for them!

# View
Problem with recyclerView and editText
Then editText have focuse and we are delete it(or update) 
We may catch exception 
@ IllegalArgumentException: parameter must be a descendant of this view @

Bad solution,
but very populare is set adjustPan in manifest

Good solution 
View.descendantFocusability = ViewGroup.FOCUS_BEFORE_DESCENDANTS
