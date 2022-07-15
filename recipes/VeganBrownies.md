~~~ markdown-script
include '../../hobbs-family-cookbook/markdownBookRecipe.mds'
recipeMenu()
~~~

# Vegan Brownies

~~~ markdown-script
recipeHeader()
~~~

  [9x9-inch baking dish](#var.vCategory='Desserts'&var.vScale=0.67)

  [9x13-inch baking dish](#var.vCategory='Desserts'&var.vScale=1)

Stir the dry ingredients together in a large bowl.

~~~ markdown-script
recipeIngredients( \
    '2 C all-purpose flour', \
    '2 C white sugar', \
    '3/4 C unsweetened cocoa powder', \
    '1 tsp baking powder', \
    '1 tsp salt' \
)
~~~

Add the liquid ingredients and mix until well blended.

~~~ markdown-script
recipeIngredients( \
    '1 C water', \
    '1 C vegetable oil', \
    '1 tsp vanilla extract' \
)
markdownPrint( \
    '', \
    'Pour into a 9x' + if(vScale < 0.7, '9', '13') + '-inch baking dish and bake for 25-30 minutes until the top is no longer shiny.', \
    'Let cool for 10 minutes before serving.' \
)
~~~
