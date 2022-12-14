# Diary Method Design Recipe

## 1. Describe the Problem

As a user
So that I can keep track of my tasks
I want to check if a text includes the string #TODO

## 2. Design the Method Signature

_Include the name of the method, its parameters, return value, and side effects._

```ruby
includes_todo = check_todo(text)

# text is a string with words in it
# includes_todo is a boolean
```

## 3. Create Examples as Tests

_Make a list of examples of what the method will take and return._

```ruby
check_todo("") => Fail "No text entered"
check_todo(ANYTHING_THAT_ISNT_A_STRING) => Fail "Input is not a string"
check_todo("A string with #TODO") => true
check_todo("A string without todo") => false
```

_Encode each example as a test. You can add to the above list as you go._

## 4. Implement the Behaviour

_After each test you write, follow the test-driving process of red, green, refactor to implement the behaviour._
