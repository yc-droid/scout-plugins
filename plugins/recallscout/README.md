# RecallScout

RecallScout connects Claude to official US government safety recall data: NHTSA vehicle recalls, owner complaints and crash-test ratings, NHTSA child car seat recalls, CPSC consumer product recalls and FDA food recalls.

## What's included

- **RecallScout connector**: the remote MCP server at `https://recallscout.salesup.workers.dev/mcp`. No account, sign-in or API key needed.
- **used-car-safety-check**: Run a complete safety check on a car someone owns or is about to buy.
- **household-recall-sweep**: Check a list of things someone owns for recalls: child car seats, baby gear, appliances, toys, other household products or food in the kitchen.

## Use it

Ask Claude to check a VIN, a used car you're considering, your child's car seat, a product at home or a food recall. The bundled skills run a complete used-car safety check or a recall sweep across a list of items you own.

## Data

RecallScout sends the VIN, vehicle make/model/year, car seat brand or model, or product and food search terms you ask about to the RecallScout server (recallscout.salesup.workers.dev), which looks them up in public US government databases (NHTSA, CPSC and openFDA). It stores nothing about you. See the privacy policy at https://recallscout.salesup.workers.dev/privacy and the terms at https://recallscout.salesup.workers.dev/terms.

## Support

Email yc@salesup.club or visit https://recallscout.salesup.workers.dev/support. RecallScout is an independent tool by Yash Chowdhury and isn't affiliated with the data providers it uses.
