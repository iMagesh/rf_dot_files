## Installation

```
gem install rubocop
```

## Configuration

The RuboCop behavior can be controlled in the .rubocop.yml file in the root path where you want to execute it. In this file, you can enable/disable certain cops (rules) or change their behavior.

## Usage

To use the RuboCop you just need to navigate to the directory where you want to run the linter, and execute:

```
rubocop
rubocop --out result.txt
rubocop lib/file.rb
rubocop app/ spec/ lib/file.rb
```


## Autocorrecting

```
rubocop --auto-correct or rubocop -a
```
