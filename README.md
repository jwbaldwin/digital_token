# Digital Token

[ISO 24165](https://www.iso.org/standard/80601.html) introduces a common language for digital currencies. Up until now, digital currencies ("crypto") have been an uncomfortable fit into the world of currencies which are governed by [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217).

`ISO 4217` does allow for private use currencies, however in common use several crypto currencies use unnoficial `ISO 4217` codes that clash with the standard.

The introduction of `ISO 24165` (and is relationship to [ISO 20022](https://www.iso20022.org)) creates a framework for the identification and standardisation of digital tokens.

In addition, the [Digital Token Identification Foundation (DTIF)](https://dtif.org) has been formed to operate a [registry](https://dtif.org/token-registry-search/) of tokens with [downloadable data](https://dtif.org/download-dti-registry/) making it easy to access and integrate the data into applications.

This library provides a means to download and access the digital token registry. One application is the upcoming integration of `digital_token` into [ex_money](https://github.com/kipcole9/money) providing money operations on both ISO 4217 currencies and ISO 24165 digital tokens.

### Non-ISO 4217 cryptocurrency codes

The following are examples of commonly-used but non-compliant `ISO 4217` currency codes. This, plus the inherent flux in the number of digital currencies gave rise to `ISO 24165`.


Unofficial code | Digits | Currency | Notes
---------- | --- | ------------- | ---------
ADA       | 6 | Ada	        | ADA conflicts with ISO 4217, because AD stands for Andorra.
BNB       | 8 | Binance	BNB | BNB conflicts with ISO 4217, because BN stands for Brunei Darussalam.
BSV       | 8 | Bitcoin SV	| BSV conflicts with ISO 4217, because BS stands for Bahamas.
BTC, XBT  | 8 |	Bitcoin     |	XBT conflicts with ISO 4217, because BT stands for Bhutan.
DAS       |	8	| Dash	      | DASH is of non-standard length.
DOGE      |	4 |	Dogecoin	  | DOGE is of non-standard length.
ETH       | 18|	Ethereum	  | ETH conflicts with ISO 4217, because ET stands for Ethiopia.
LTC       | 8 |	Litecoin	  | LTC conflicts with ISO 4217, because LT stands for Lithuania.

### Installation

The package can be installed by adding `digital_token` to your list of dependencies in `mix.exs`:

```elixir
def deps do
  [
    {:digital_token, "~> 0.1.0"}
  ]
end
```

The docs can be found at <https://hexdocs.pm/digital_token>.

