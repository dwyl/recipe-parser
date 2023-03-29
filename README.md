<div align="center">

# `Recipe Parser` 🍲 🥗 🌮 😋

**Parse recipes** from your favorite websites, 
blogs or social posts <br />
to `extract` and `enhance` 
the ingredients and instructions 
for your **meal planning**.

</div>

# Why?

There are many good recipes online
but there isn't a good way 
to import them 
into your favorite meal planning system.

So we end up storing them as links
and then have to click into page
(which can take several seconds to load)
read through the whole
recipe each time.
This is an inefficient use of time.

We want to 
**solve our _own_ nutrition 
and meal planning problem**
from first principals.

The starting point: recipes. 


# What?

This project will eventually parse _any_ recipe
from _any_ website using Machine Learning (ML).
But for now we are doing the parsing _manually_
by hand-crafting a parser for each website
that we want to extract a recipe from.

This is an example of 
["do things that don't scale"](http://paulgraham.com/ds.html).
We are not going to spend hundreds (thousands?) of hours/dollars
building ML models to parse recipes
when what we _really_ want to do
is build the _interface_ for meal-planning.
Rather we are going to create parsers
for the top 10 (ish) recipe websites
so that we get started as quickly as possible.

## Which Sites?

We want to build up a bank of parsers
that will parse recipe data from 
_any_ website.
This alphabetical list is our "roadmap":

+ [ ] https://www.allrecipes.com
+ [ ] https://www.bbcgoodfood.com
+ [ ] https://www.delish.com
+ [ ] https://www.epicurious.com
+ [ ] https://www.recipetineats.com
+ [ ] https://www.simplyrecipes.com

**Please `add`** to this **list** by opening an issue: 
[dwyl/recipe-parser/issues](https://github.com/dwyl/recipe-parser/issues)

> **Note**: the order listed 
> is not necessarily the order we will create the parsers
> rather they will be created on an adhoc basis
> as required or voted on by the `people` needing the parser.

# Who?

This project is "by us for us". 
We are _using_ the parser to import recipes
so that we have a starting point for our meal planning system.

If you find this useful 
you can use it
by following the instructions below.


## Contributing

There are _many_ ways you can contribute.
1. Use the parser and give feedback!
2. Vote on the list of recipe websites we should parse next!
3. Add to the list of recipe websites
4. Improve the documentation so that the project is useful to more people
5. Write a parser! 

# How?

Coming soon! 

<br />
<br />

# Research

## Precedents

Before creating this library
we exhaustively looked at other
instances of recipe parsers online,
e.g: 
[github.com/forbesg/bbc-good-food-recipe-scraper](https://github.com/forbesg/bbc-good-food-recipe-scraper)

There's nothing new about creating a recipe parser. 
What's new in this library:
1. **_Extensive_ Tests** - with automated tests and sample data
2. **_Actively_ Maintained** - if spot anything not working with the parser, please open an issue. 🙏
3. **Contributions 

# Roadmap

_Before_ embarking on this project,
we tried using `GPT` to parse recipes. 
The results were inconsistent (non-deterministic)
even with `GPT-4`. 
So we are hand-crafting parser
and will collect as much _human_ feedback
as possible on the quality/consistency of the parser(s).
We _may_ end up using `AI` (`ML`/`LLMs`) 
to _enhance_ our parser in the future.
Especially once we have parsed 20+ websites
(and a few thousand recipes)
and can consistently extract valid 
_training_ data for an ML model to reference.

## Extracting Recipe Data from _Images_

We want to be able to take a photo of a recipe
in a book and have the ingredients, 
instructions and picture extracted. 
This will require some ML/OCR work.
If you would like to contribute to this,
please leave a comment
on this issue: 
[dwyl/recipe-parser/**issues/5**](https://github.com/dwyl/recipe-parser/issues/5)