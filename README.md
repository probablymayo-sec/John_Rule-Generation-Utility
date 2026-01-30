# John_Rule-Generation-Utility

This utility will generate a very long list of rules for JohnTheRipper. These are meant to be thrown into the John configuration file (normally: `john.conf`)

The rule outputs can be redirected to a rule file in the following fashion: 
- ```python3 John_Rule-Generation-Utility.py > johnRules.txt```

These rules are sorted by length or "complexity" 

It should be noted that the `:` rule among others like `c` and `a` should be added to your ruleset as this rule generation leaves them out (except for `l`)

Generally, I find that copying the `john.conf` file and adding the ruleset to the new copy is the best way to maintain the defualt configuration of John should you want to return back to it. With this method, use the `sudo` command to allow you to edit the 2nd configuration file. From here, you can tell john to use that config file instead of the default config file with `john --config=/path/to/your/config.conf`

