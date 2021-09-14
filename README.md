# circlceci-dynamic-config-sandbox
My CircleCI dynamic config sandbox

# Merge config.yml
If you want to check merged config.yml locally, execute these commands.

## `circleci config pack`
`circleci config pack .circleci/config_pack`

## `yq`
`yq ea '. as $item ireduce ({}; . * $item )' .circleci/config_yq/config_*`