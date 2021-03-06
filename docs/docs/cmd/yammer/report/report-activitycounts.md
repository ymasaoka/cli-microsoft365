# yammer report activitycounts

Gets the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked

## Usage

```sh
yammer report activitycounts [options]
```

## Options

Option|Description
------|-----------
`--help`|output usage information
`-p, --period <period>`|The length of time over which the report is aggregated. Supported values `D7,D30,D90,D180`
`--query [query]`|JMESPath query string. See [http://jmespath.org/](http://jmespath.org/) for more information and examples
`-o, --output [output]`|Output type. `text,json`. Default `text`
`--verbose`|Runs command with verbose logging
`--debug`|Runs command with debug logging

## Examples

Gets the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked for the last week

```sh
yammer report activitycounts --period D7
```

Gets the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked for the last week and exports the report data in the specified path in text format

```sh
yammer report activitycounts --period D7 --output text > "activitycounts.txt"
```

Gets the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked for the last week and exports the report data in the specified path in json format

```sh
yammer report activitycounts --period D7 --output json > "activitycounts.json"
```
