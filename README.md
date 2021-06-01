# Whitepaper

Curation Markets is a model that allows groups to more effectively coordinate & earn from value they co-create around shared goals.

Readings:
1. [Designing Bond Curves](https://medium.com/thoughtchains/on-single-bonding-curves-for-continuous-token-models-a167f5ffef89)
1. [Curation Markets Whitepaper](https://docs.google.com/document/d/1VNkBjjGhcZUV9CyC0ccWYbqeOoVKT2maqX0rK3yXB20/edit)
1. [Thought piece of bonding curve cryptoeconomics](https://blog.cosmos.network/distribution-curves-a-thought-piece-on-cryptoeconomics-246b43a3a5ee)
1. [Making it profitable to protect the commons](https://medium.com/@simondlr/saving-the-planet-making-it-profitable-to-protect-the-commons-50393906fe22)

## Economic Design

To enter Eden, you must first purchase Eden tokens using an AMM functioning on an exponential bonding curve. My vision is `y = (x/1000000)^(z), 3/2 ≤ z ≤ 2`.  The upper bound of 2 was inspired by BitClout and Metcalfe's law. This will be deposited into the Vault contract.

With the launch of ETH 2.0, this ETH will be staked to earn a yield. The yield will be used to purchase Eden tokens from the AMM as support. In the meantime, time-permitting, we will explore yield-generating strategies like yearn.finance.

Eden tokens can be used to purchase project tokens. Project tokens are purchased through an AMM operating on a logarithmic curve that transitions to a linear function to encourage experimentative speculation in the near term and stability as the project matures. 

The amount of Eden tokens held by the project token contract represents its claim on a proportional amount of ETH held by the Vault. This ETH is available for use as collateral for projects to take out DeFi loans. (Maybe the Eden token can be used as collateral?) The collected interest will purchase Eden tokens that are automatically reinvested into the project's own token, to encourage the project to use the source of capital.
