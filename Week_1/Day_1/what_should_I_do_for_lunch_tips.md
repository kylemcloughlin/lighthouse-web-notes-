### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces.

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.
```
 function whatToDoForLunch(hungry, availableTime) {


 //If we're not hungry, we want to tell ourselves to get back to work.
  if (hungry === false) {
    return "Get back to work.";
  }

  //Otherwise,
  else {

    //we want to pick something up and eat it in the lab when we've got less than 20 minutes
    if (availableTime < 20) {
      return "Pick something up and eat it in the lab.";
    }

    //try a place nearby if we've got between 20 and 30 minutes
    else if (availableTime >= 20 && availableTime <= 30) {
      return "Try a place nearby.";
    }

    //If we have any more time than 30 mins
    //we want to remind ourselves that we're in a bootcamp and that we
    //should reconsider how much time we actually have to spare.
    else {      return "You're in bootcamp, reconsider how much time you have to spare.";
    }

  }
}


/*
 * This is some test runner code that's simply calling our whatToDoForLunch function
 * defined above to verify we're making the right decisions. Do not modify it!
 */

//console.log("I don't know what to do!");

```





