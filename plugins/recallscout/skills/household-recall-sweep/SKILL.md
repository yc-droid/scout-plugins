---
name: household-recall-sweep
description: Check a list of things someone owns for recalls: child car seats, baby gear, appliances, toys, other household products or food in the kitchen. Use when the user lists items, says they have a new baby, or asks whether anything they own has been recalled.
---

To sweep a list of items for recalls:

1. Sort each item into one bucket: child car seat or booster → `search_car_seat_recalls` with the brand and model; food or drink → `search_food_recalls`; any other consumer product → `search_product_recalls` with the brand and product type.
2. Run one search per item. Use the brand plus a short product word, for example "Graco stroller" or "space heater".
3. Report a table with columns Item | Status (Recalled / Possible match / No recall found) | What to do. "Possible match" means the brand and product type match but the model or dates need checking.
4. For each match, give the hazard, the remedy and the official link, and tell the user what to compare: the model number and date of manufacture on the label for car seats and products, or the lot codes and package size for food.
5. Put anything with a risk of serious injury, a child hazard or an FDA Class I food recall first.

Coverage is the United States only. Meat, poultry and egg recalls come from the USDA and aren't included.
