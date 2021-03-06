# home-assistant_OctopusAgile rates card
Octopus Agile custom card to display future rates in Home Assistant

## Referral code
Feel free to use my referral code and get £50 credit to your account (as well as mine): https://share.octopus.energy/lilac-bison-793

## Installation
1. Download [agile-rates-card.js](https://raw.githubusercontent.com/markgdev/home-assistant_OctopusAgile/master/custom_cards/agile-rates-card.js)
2. Place file in config/www directory. - Create this directory and restart home assistant if this doesn't exist.
3. Add the resource to lovelace in configuration -> Lovelace dashboards -> Resources 
    * Enable advanced mode and put lovelace into edit mode first
    * Url: /local/agile-rates-card.js
    * Resource Type: Javascript module
4. Add card to dashboard
```
entity: octopusagile.rates
type: 'custom:agile-rates-card'
// The below are optional.
cols: 4
mediumlimit: 9
highlimit: 15
```

### Example
![Image of Card](https://raw.githubusercontent.com/markgdev/home-assistant_OctopusAgile/master/custom_cards/agile-rates-card-screenshot.png)


This card was created with the help of the [Lovelace attributes card](https://community.home-assistant.io/t/lovelace-attributes-card-entity-row/59122) and the Home assistant custom card guide.
