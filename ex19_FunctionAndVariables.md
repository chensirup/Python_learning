# Function And Variables

### New ex19.py

- **Writed the new :**

```
def cheese_and_crackers(cheese_count,boxes_of_crackers):
    print("You have %d cheese!"%cheese_count)
    print("You have %d boxes of crackers!"%boxes_of_crackers)
    print("Man that's enough for a party!")
    print("Get a blanket.\n")


print("We can just the function numbers directly:")
cheese_and_crackers(20,30)



print("OR, we can use variables from our script:")
amount_of_cheese=10
amount_of_crackers=50

cheese_and_crackers(amount_of_cheese,amount_of_crackers)


print("We can even do math inside too:")
cheese_and_crackers(10+20,5+6)


print("And we can combine the two,variables and math:")
cheese_and_crackers(amount_of_cheese+100,amount_of_crackers+1000)

```

- **Runed it :**

```
PS F:\mystuff> python ex19.py
We can just the function numbers directly:
You have 20 cheese!
You have 30 boxes of crackers!
Man that's enough for a party!
Get a blanket.

OR, we can use variables from our script:
You have 10 cheese!
You have 50 boxes of crackers!
Man that's enough for a party!
Get a blanket.

We can even do math inside too:
You have 30 cheese!
You have 11 boxes of crackers!
Man that's enough for a party!
Get a blanket.

And we can combine the two,variables and math:
You have 110 cheese!
You have 1050 boxes of crackers!
Man that's enough for a party!
Get a blanket.
```

That's a error in the first run :

```
PS F:\mystuff> python ex19.py
We can just the function numbers directly:
Traceback (most recent call last):
  File "ex19.py", line 9, in <module>
    cheeses_and_crackers(20,30)
NameError: name 'cheeses_and_crackers' is not defined
```

The variable is `cheese`, no `cheeses`.

***
### Thinking

- **Write a new function by myself in `ex19_1.py` :**

```
def my_family(male_count,female_count,amount):
    print("My family have %d male."%male_count)
    print("My family have %d female."%female_count)
    print("This is my family %d peoples.\n"%amount)

print("We can just the function numbers directly:")
my_family(3,2,5)

print("Variables from script:")
amount_of_male=5
amount_of_female=5
amount_of_family=10

my_family(amount_of_male,amount_of_female,amount_of_family)

print("do math:")
my_family(3+2,2+3,5+5)

print("math and variables:")
my_family(amount_of_male+1,amount_of_female+2,amount_of_family+3)

print("math and variables too:")
my_family(amount_of_male,amount_of_female,amount_of_male+amount_of_female)

```


- **Runed it :**

```
PS F:\mystuff> python ex19_1.py
We can just the function numbers directly:
My family have 3 male.
My family have 2 female.
This is my family 5 peoples.

Variables from script:
My family have 5 male.
My family have 5 female.
This is my family 10 peoples.

do math:
My family have 5 male.
My family have 5 female.
This is my family 10 peoples.

math and variables:
My family have 6 male.
My family have 7 female.
This is my family 13 peoples.

math and variables too:
My family have 5 male.
My family have 5 female.
This is my family 10 peoples.
```

I did it .

***
- Changelog
- 2017-02-22 12:02:26 ©陈sir
