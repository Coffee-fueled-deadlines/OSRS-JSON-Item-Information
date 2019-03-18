# OSRS-JSON-Item-Information

  The OSRS Market API is a bit poorly designed (in my opinion) as it requires you to iterate
  through item IDs to get the name of the item.  This means that, in some applications, you
  have to iterate through every item ID to check the name of the item if you're looking for
  information on a specific item.

  This list is a fix for that.  It displays some basic information of items in OSRS (including
  current market information based off of RSBuddy's API) and is updated regularly by one of my
  discord bots.  That means that, for the most part, this information will contain up to date
  information.  Most importantly, however, the keys in this JSON list are based off of the
  item's NAME instead of it's id.

  Prior, to get the Store Price of an item (without knowing it's item ID prior), you had to do
  this:

  	for i in ITEMS:
  		if ITEMS[i]['name'] == "Rune Dagger":
  			itemPrice = ITEMS[i]['sp']

  However, now with this new list, looking up a specific item is as easy as this:

  	itemPrice = ITEMS['rune dagger']['store_price']

  This saves your application time and thus resources while searching for user supplied item
  information.

  Hope it helps!
  
### Back-link to Patreon with other information

  https://www.patreon.com/Coffee_Fueled_Deadlines
    Link above links to patreon page with information on Discord Bots and other applications.
