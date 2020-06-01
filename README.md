# Additive Shader - Weather

> Under construction

This mod extends Additive Shader with some weather-dependent visibility toggles.

The following tags are supported:

|tag                  |Description                       |Game Property         |
|:---                 |:---                              |:---                  |
|`on-during-rain`     |Visible when it's raining/snowing.|`m_currentRain`       |
|`off-during-rain`    |Hidden ^^                         |                      |
|`on-during-fog`      |Visible when it's foggy           |`m_currentFog`        |
|`off-during-fog`     |Hidden ^^                         |                      |
|`on-during-cloud`    |Visible when it's cloudy          |`m_currentCloud`      |
|`off-during-cloud`   |Hidden ^^                         |                      |
|`on-during-freezing` |Visible when temperature < 0°C    |`m_currentTemperature`|
|`off-during-freezing`|Hidden ^^                         |                      |

TODO: User can set thresholds in the mod settings screen.

Example of an `m_mesh.name` that is on when raining, but not when freezing, with fade of `10` and light intensity of `1`:

```
AdditiveShader RemoteControl 10 1 on-during-rain off-during-snow
```

You could maybe use these for highway LED signs or something like that?
