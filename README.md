# TextOverPlayer

TextOverPlayer is a Minecraft plugin that displays chat messages above a player's head using Armor Stands. It supports HEX colors, custom particle effects, and configurable message display times.

## Features

- Display chat messages above a player's head.
- Support for HEX color codes in messages.
- Customizable particle effects.
- Configurable message display duration.
- Commands to reload configuration and change settings.

## Commands

- `/textoverplayer reload`: Reload the plugin configuration.
- `/textoverplayer max-line-length [number]`: Set the maximum line length for messages.
- `/textoverplayer max-lines [number]`: Set the maximum number of lines for messages.
- `/textoverplayer initial-display-time [number]`: Set the initial display time for messages.
- `/textoverplayer additional-time-per-line [number]`: Set the additional display time per line.
- `/textoverplayer particle-type [type]`: Set the particle type for effects.
- `/textoverplayer particle-count [number]`: Set the particle count for effects.
- `/textoverplayer particle-enabled [true/false]`: Enable or disable particle effects.
- `/textoverplayer chat-line-enabled [true/false]`: Enable or disable chat messages above the player's head.

## Permissions

- `textoverplayer.use`

## Configuration

The `config.yml` file contains the following settings:

```yaml
max-line-length: 30
max-lines: 5
particle-type: VILLAGER_HAPPY
particle-count: 10
particle-enabled: true
chat-line-enabled: true
initial-display-time: 5
additional-time-per-line: 2
messages:
  reload: "&aConfiguration reloaded!"
  set_max_line_length: "&aMax line length set to {length}! &ePlease use /textoverplayer reload to apply changes."
  set_max_lines: "&aMax lines set to {lines}! &ePlease use /textoverplayer reload to apply changes."
  set_particle_type: "&aParticle type set to {type}! &ePlease use /textoverplayer reload to apply changes."
  set_particle_count: "&aParticle count set to {count}! &ePlease use /textoverplayer reload to apply changes."
  set_particle_enabled: "&aParticle enabled set to {enabled}!"
  set_chat_line_enabled: "&aChat line enabled set to {enabled}!"
  set_initial_display_time: "&aInitial display time set to {time} seconds!"
  set_additional_time_per_line: "&aAdditional time per line set to {time} seconds!"
  invalid_number: "&cInvalid number!"
  invalid_particle: "&cInvalid particle type!"
  invalid_boolean: "&cInvalid value! Use true или false."
