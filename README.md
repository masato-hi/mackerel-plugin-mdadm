# mackerel-plugin-thermal
Add metrics of mdadm's RAID device information to mackerel.

## Installation
#### Place mackerel-plugin-mdadm and make it executable.
```
curl -o /usr/local/bin/mackerel-mdadm https://raw.githubusercontent.com/masato-hi/mackerel-plugin-mdadm/master/mackerel-plugin-mdadm
chmod +x /usr/local/bin/mackerel-plugin-mdadm
```

#### Please add the following contents to /etc/mackerel-agent/mackerel-agent.conf
```
[plugin.metrics.mdadm]
command = "mackerel-plugin-mdadm"
```

#### Please reload mackerel-agent.
```
service mackerel-agent reload
```


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/masato-hi/mackerel-plugin-mdadm.


## License

The script is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

