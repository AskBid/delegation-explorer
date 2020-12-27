# Delegation Explorer Backend

Delegation Explorer is a Rails App API Backend that interfaces with a Javascript Frontend with no framework.

The backend populates its postgresQL database by raketasks that query a GraphQL API mainteined from a `[cardano-graphql`](https://github.com/input-output-hk/cardano-graphql). Look in the [backend submodule](https://github.com/AskBid/delegations-explorer-backend) for more information.

Delegation Explorer allows User of the [Cardano Blockchain ](https://cardano.org/) who own a stake address to track that address rewards and compare the rewards they would have achieved by delegating instead to different Pools that they want to follow.

The backend repo has a `seed.rb` file that populates the database with two epochs worth of data that allows teh use of the web app without the need to build the Cardano nodes and GraphQL API.


# About Cardano delegations

Every Cardano Coin (₳) holder can delegate their holdings to a Pool. Each delegation worth is represented from the StakeAddress amount.
Each Pool participate to a lottery to produce blocks, the more delegations a Pool have, the more likely it is to be assigned blocks to produce. Pool performance also contributes to how many blocks the pool will produce.
For each block produced the Pool will get ₳ rewards that will be split proportionally between all the Delegators.
Delegations and Rewards distribution is organised in Epochs, every 5 days new delegations can be assigned and old rewards are delivered.

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/AskBid/delegations-explorer. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the [Contributor Covenant](contributor-covenant.org) code of conduct.

## License

The repository is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT)