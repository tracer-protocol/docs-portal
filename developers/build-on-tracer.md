# Build on Tracer

Tracer is a composable piece of infrastructure that can be integrated into any application. In addition to providing a set of audited contracts tested in practice, Tracer provides help with aspects such as market making, co-marketing, data availability, and parameter optimisation.

> With Tracer, you are not alone. Develop using Tracer's contracts and we'll support you throughout your journey.

The Tracer product suite currently consists of the Perpetual Pools template. The table below helps you determine whether Perpetual Pools are the right contract for your application.

| Property                          | Perpetual Pools v2                                                                                                      |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Data sources                      | Any standardised Tracer Data Feed (e.g. any Chainlink feed)                                                             |
| Data source manipulations         | Any wrapper available in Tracer Data Factory (e.g. arithmetic, smooth moving average)                                   |
| Fees                              | Configurable; annual management, mint, and burn fees available. Can be split between two recipients at different rates. |
| Funding rate                      | In-kind, value is determined by other parameters                                                                        |
| Leverage                          | Positive integers (IEEE754 bytes16)                                                                                     |
| Leverage function                 | Sigmoidal                                                                                                               |
| Liqudation mechanism              | None, positions are fully funded                                                                                        |
| Margin requirement                | None, positions are fully funded                                                                                        |
| Settlement asset                  | Any non-rebasing, non-deflationary ERC-20 token                                                                         |
| Tokenised position representation | Yes; separate ERC-20 for long and short positions                                                                       |
| Transferable ownership            | Yes; position represented by a token                                                                                    |
| Volatility decay                  | Yes; impact is dependent on data source, leverage, and mint & burn fees                                                 |

## Development Guides

* [Perpetual Pools](https://app.gitbook.com/s/kfN6trJwMTrtfGeIe8lX/developer-resources/development-guide)

{% hint style="info" %}
Questions? Head over to the #developers channel on our [Discord](https://discord.gg/TracerDAO) for help!
{% endhint %}
