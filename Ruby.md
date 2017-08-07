# Ruby Questions

## Which of the expressions listed below will result in "false"?
```ruby
true    ? "true" : "false"  n
false   ? "true" : "false"  y
nil     ? "true" : "false"  n
1       ? "true" : "false"  n
0       ? "true" : "false"  y
"false" ? "true" : "false"  y
""      ? "true" : "false"  n
[]      ? "true" : "false"  n
```
## I want to write some code that takes an array of numbers, multiplies each item in the array by 3, and returns a new array with the new values. know I should use #map, #each, or #select, but I’m not sure which one is best -- teach me.

```ruby
def foo(array)
  array.each do |num|
    p num * 3
  end
end
```

## What are the common controller actions?

index, new, create, show, edit, update, destroy

## Which of the following is not a benefit of Object-Oriented Programming?

a) Reduces side effects of functions  x
b) Enables code reuse
c) Encapsulates functionality
d) Allows the developer to make certain methods/variables inaccessible to other classes

## Consider the following two methods:
```ruby
def times_two(arg1);
  puts arg1 * 2;
end

def sum(arg1, arg2);
  puts arg1 + arg2;
end
```
What will be the result of each of the following lines of code:
```ruby
times_two 5   nil
times_two(5)  10
times_two (5) 10
sum 1, 2      nil
sum(1, 2)     3
sum (1, 2)    3
```

## What is missing? M_____/View/Controller

  app

## What is the most beneficial aspect of TDD?

  For TDD you can check the logic, make sure it would all work, and see what is acting up before writting the code for the app.

## Write a function that accepts an array of numbers and a second number. Beginning at index 0, total up the sum of the values of the array until you've met or surpassed the second argument. Return the number of elements required to fulfill the goal. If the goal can't be reached, return 0.

```ruby
  def foo(arr, num)
    sum = 0
    arr.each_with_index do |number, index|
      if sum < num
         sum + number
      else 
        index
      end
    return index
    end
  end
  ```
      
  
    

## Make a copy of http://jsbin.com/beyape/1/edit complete the task described in the comments and attach the link

http://jsbin.com/qurihopumo/edit?html,js,output
(function(time){
  // Based on the current time, using JS and jQuery, 
  // make the following pronouncements:
  // Between 9AM and Noon: We come in peace.
  // Between Noon and Midnight: We are the borg. Resistance is futile.
  // Any other time: All your base are belong to us. You have no chance to survive make your time.
  $("#myMessageToEarth").append("We come in peace.<br>")
    $("#myMessageToEarth").append("For now...")
    }
  else if (time >=12 && time <24)
    $("#myMessageToEarth").html("We are the borg. Resistance is futile.")
  else
    $("#myMessageToEarth").html("All your base are belong to us. You have no chance to survive make your time.")
})()
