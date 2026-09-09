# Site index · format 2
Structure and the names of what each page offers. Values that change often — prices, hours, phone,
address — and body copy are deliberately not recorded here; read the page itself for those.

## index.html → /
title: Rainbow Thai – Authentic Thai Food, Pad Thai, Curries & Roti in Westport, CT
purpose: The whole site — a one-page restaurant site carrying both menus, hours, gallery, reviews and FAQ.
sections:
- `#home` "Rainbow Thai - Authentic Thai Cuisine, Pad Thai, Curries, Roti" — hero with the tagline and the Explore Menu and Order Online calls to action
- `#about` "About Rainbow Thai" — the restaurant's description and its Fresh Ingredients and Traditional Recipes points
- `#menu` "Authentic Thai Cuisine" — the menu, presented as two tabbed panels named All Day Menu and Lunch Menu
- `#dinner-menu-btn` — the tab button that shows the All Day menu
- `#lunch-menu-btn` — the tab button that shows the Lunch menu
- `#dinner-menu-content` "Dinner Pricing" — the All Day panel, a price table by protein followed by 85 dishes grouped under Appetizer, Soup, Salad, Chef Special, Noodle & Rice, From the Wok, Curries, Noodle Soup, Side Dishes and Dessert: Vegetable Spring Roll, Edamame, Chicken Cashew Wrap, Roti Canai, Crab Rangoon, Curry Puff, Po Pia Sod, Shrimp Summer Roll, Tao Hoo Tord, Chicken Satay, Chicken Wing, Lime Chili Shrimp, Crispy Calamari, Mee Grob, Kong Tod, Tom Yum Goong, Tom Kha Gai, Sweet Corn Soup, Vegetable Soup, Thai Salad, Somtum, Nua Nam Tok, Duck Salad, Yum Woon Sen, Sizzling Pancake, Seafood Delight, Pla Rad Prik, Pla Sam Rod, Salmon Mango Curry, Steamed Ginger Fish, Pineapple Duck Curry, Duck Choo Chee, Duck Ga Prow, Peanut Shrimp Curry, Laksa Shrimp, Pra Raam Chicken, Shaking Beef, Garlic Eggplant Asparagus, Pad Thai, Drunken Noodles, Pad See Ew, Pad Woon Sen, Mee Goreng, House Fried Rice, Spicy Fried Rice, Pineapple Fried Rice, Basil, Cashew Nut, Ginger, Garlic, Sambal, Sweet and Sour, Broccoli, Pad Ped, Mango Curry, Yellow Curry, Masaman Curry, Jungle Curry, Pineapple Curry, Rendang, Red Curry, Green Curry, Penang Curry, Noodle Soup, Tom Yum Noodle Soup, Duck Noodle Soup, Jasmine rice, Brown rice, Thai Sticky Rice, Steamed Vegetable, Add Tofu, Peanut Sauce, Prik Nam Pla, Hot Sauce, Mango Sticky Rice, Coconut Pudding, Fried Banana, Fried Ice Cream, Ice Cream
- `#lunch-menu-content` "Lunch Pricing" — the Lunch panel, a price table by protein followed by 27 dishes grouped under Noodle & Rice, From the Wok, Curries and Noodle Soup: Pad Thai, Drunken Noodles, Pad See Ew, Pad Woon Sen, Mee Goreng, House Fried Rice, Spicy Fried Rice, Pineapple Fried Rice, Basil, Cashew Nut, Ginger, Garlic, Sambal, Sweet and Sour, Broccoli, Pad Ped, Mango Curry, Yellow Curry, Masaman Curry, Jungle Curry, Pineapple Curry, Rendang, Red Curry, Green Curry, Penang Curry, Noodle Soup, Tom Yum Noodle Soup
- `#visit` "Hours" — the weekly opening hours, one row per day, with the address and directions
- `#gallery` "The Rainbow Thai Experience" — photographs of the room and the dishes
- `#reviews` "What Our Customers Say" — customer review quotes
- `#faq` "Frequently Asked Questions" — an accordion covering: reservations, vegetarian or vegan options, parking
also: Every one of the 27 lunch dishes is written a second time in the All Day panel, so renaming a dish means finding it in both panels. Nothing on screen shows the two disagreeing, because only one panel is visible at a time.
also: The two menu panels are shown and hidden by script through the tab buttons above them, so only one is visible at a time and a change made to the visible panel is easy to believe is the only one needed.
also: The dish rows repeat the same markup per dish, so a change to one row's structure has to be made to every row in that panel.

## support files
Files that are not pages. A line marked [content] holds words or data a visitor reads, so a
change to the site's content can land there; the rest only make the site work or look right.
- `robots.txt` — crawler rules and the sitemap link — derived from the site by the deploy, not written by hand
- `sitemap.xml` — the list of page URLs — derived from the site by the deploy, not written by hand

## shared (every page)
The header, navigation, mobile menu and footer are propagated from index.html to every other page by
`shell_propagation`. A change to any of them is made on index.html alone and copied automatically.
