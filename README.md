# moltbot

### Primary and other model check on terminal

`clawdbot config get agents.defaults.model`

`clawdbot config get agents.defaults.models`

`clawdbot config set agents.defaults.model '{"primary": "openrouter/nvidia/nemotron-3-nano-30b-a3b:free"}'`

### Restart

`clawdbot gateway restart`

### Adding clawdbot user to docker 

`journalctl --user -u clawdbot-gateway.service -n 20 --no-pager` : if `clawdbot tui` not working inside ssh

`ssh clawdbot@72.60.29.216`

`sudo usermod -aG docker clawdbot`

