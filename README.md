# GOKZ Rank Kicker

This plugin kicks players who are not high enough Global API rank, so you can create a server that only accepts skilled
enough players. The players score is checked based on the servers default GOKZ mode.

Configure the minimum required rank or score amount by using the following cvars:

* `grk_minimum_allowed_skillgroup`
  This skillgroup and higher will not be kicked from the server.
* `grk_minimum_allowed_score`
  This score and higher will not be kicked from the server.

In addition to this, you can also specify immunity from the kicker based on Sourcemod admin flags and command access.
By default players with the Reserved slot access are immune (`a` flag). You can configure this by using SourceMod
overrides. To change the immunity to admins only for example, use overrides like this:

```text
Overrides
{
    "grk_kicker_immunity" "b"
}
```
