# pokemon-to-calculator

A plain HTML calculator for planning a VGC tournament. It works out the time, judge pay and prize pot for an event.

Live page: https://pizzacatz.github.io/pokemon-to-calculator/

## Using it

Every box can be edited. Changing one box updates the others, both forwards and backwards.

- **players** sets the Swiss rounds, top cut rounds and Bo1/Bo3 times, using the player brackets from the original spreadsheet.
- **judge compensation per entry × players** = total payout. Total payout divided by the event's hours gives pay per hour.
- **pot contribution per entry × players** = total pot. Prizes are 50% for 1st, 25% for 2nd and 12.5% each for 3rd and 4th.
- **house cut × players** = house total cut.
- **entry cost** = judge compensation + pot contribution + house cut.
- **working backwards changes** decides what changes when you type into a total, a prize or an hourly rate: the per-entry amount, or the number of players.

Boxes show `N/A` with fewer than 4 players, and `ERROR` when no value works.

## Files

- `index.html`: the whole app. It has no CSS and no dependencies.

To update the live page, edit `index.html`, then commit and push to `main`. GitHub Pages redeploys it.
