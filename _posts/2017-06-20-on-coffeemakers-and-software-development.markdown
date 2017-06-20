---
layout: post
title:  "On Coffeemakers and Software Development"
date:   2017-06-20 07:00:00 -0400
categories: development
---
Anyone who has worked with me has probably noted my strong affinity for coffee in all its varieties. Depending on my mood, I might enjoy breaking up the day with a cappuccino, mocha, latte, flat white, macchiato, espresso, kalita, Turkish or French press coffee. To service ~~addicts~~ afficianados like me, coffee shops might install a machine such as the [Nuova Simonelli Aurelia II](http://www.espressooutlet.net/nuova-simonelli-aurelia-ii-3-group-volumetric-commercial-espresso-machine/?gclid=CjwKEAjwgtTJBRDRmd6ZtLrGyxwSJAA7Fy-hbcwuCgwe5SXEYga9gK-2UDlptcv1Wvdx5ZIqP72axhoCQEvw_wcB) which has every possible feature enabling it to make any kind of coffee beverage imaginable. 

The functions of such a device are impressive but a far more popular coffeemaker for personal use is the [Bialetti Moka Express](http://www.bialetti.com/coffee/stovetop/moka-express-c-1_7_22.html). Its [simple, mass-producible design](https://en.wikipedia.org/wiki/Moka_pot#Brewing_coffee_with_a_moka_pot), consisting of three parts that can be individually disassembled, replaced, and washed has gone largely unchanged since it was first conceived in 1933. While the Bialetti cannot on its own make the range of drinks of other machines, its reasonable price, ease of use, and low maintenance have led to its widespread adoption and today a Moka Express can be found in nearly every Italian kitchen.

Which machine has the better design? Of course, the answer depends on the use case. 

The Aurelia II is extremely capable but is far more expensive, requires training to use, and is harder to clean and maintain. For a coffee shop with diverse customer tastes, sufficient capital, and knowledgeable baristas these are reasonable tradeoffs to make. 

The moka pot merely makes coffee but is far more affordable, requires no training to use, and is trivial to clean and maintain. These are attractive qualities for the average family that wants to make a straightforward, good cup of coffee.

Suppose that family also wants to make, let’s say, a cappuccino? They might separately purchase a milk steamer to go along with their Bialetti. In addition, those who wish to control how finely their beans are ground can buy their own coffee grinder. So while the use cases of the Bialetti by itself are limited, additional features may be added separately that, when combined, still allow for a wide range of beverages to be crafted.

Suppose a new product manager at Bialetti surveys the market and finds that tastes in coffee are incredibly varied. They might ask for a machine such as the Aurelia II to be produced and they would not be wrong. Nevertheless, a mature engineer would still inform them of the tradeoffs they might not know they are making when encouraging a more complicated product to be built.

Developers face a similar set of choices when we consider how to build our applications. Software is certainly more complex than coffee and there is every temptation to construct programs that handle all known and possible future use cases. We should still pause and think about what value provide with the products we build.

People do not derive value from using coffeemakers; they derive value from drinking coffee.

People do not derive value from using software; they derive value from a job done well.

The need to reliably deliver working software within finite schedules and budgets requires us to approach our development in a manner that accounts for the most common use case first and is extremely replicable. We should explore options to treat orthogonal concerns separately: opting to build the coffeemaker apart from the milk steamer so that we can deliver and maintain each independently. In addition to lowering production costs, we might find that after building the former we have less need for the latter after all. If we do eventually learn that our customers truly want a more complex product, we will be in a far better position to create one if we already have several working components.

As an industry, I believe we can improve in our ability to focus on the highest value item among many. Let’s strive to choose simple solutions that compose well together so that we can do more with less.