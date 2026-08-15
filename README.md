# Smiffy's Github

Python, "grown up" AI, embedded, IoT.

## What to look at

Anything you like :-p Ordered by what is likely to be most useful.  These are working bits and bods 
from systems I have built/run, put here in case they may be useful to someone. Not necessarily active projects.

## Agent infrastructure

- **[state-mcp](https://github.com/smiffy-online/state-mcp)** — PostgreSQL-backed state management via MCP.
Persistent memory and coordination across conversations and across agents. Context loss is what makes agents 
unreliable over long-running work; this is what is working for me.
  - **[state-mcp-extension](https://github.com/smiffy-online/state-mcp-extension)** — Claude Desktop extension (MCPB)
  - **[state-mcp-proxy](https://github.com/smiffy-online/state-mcp-proxy)** — REST proxy for iOS and web access 
DEPRECATED, Anthropic finally has this covered, to a degree.
- **[dasmodel](https://github.com/smiffy-online/dasmodel)** — experimental agent interface for Ollama models, 
local or cloud, with MCP tool integration, shell access, and a training feedback loop. Now deprecated; 
it was a useful investigative exercise, now integrating/modifying Hermes Agent.
- **[filesystem_supertool2](https://github.com/smiffy-online/filesystem_supertool2)** — filesystem and 
code-navigation tooling over MCP. **Active development**
- **[mcp-browser-client](https://github.com/smiffy-online/mcp-browser-client)** — zero-dependency JavaScript
MCP client for browsers. Streamable HTTP transport. See what your models are talking about, behind your back!
- **[mcp-icloud-calendar](https://github.com/smiffy-online/mcp-icloud-calendar)** — iCloud calendar access over MCP.
Because *of course* Apple doesn't just have a nice API for this. 

## Misti

- **[misti](https://github.com/smiffy-online/misti)** — architecture, design rationale and search DSL for the 
multi-agent platform the tooling above was built for. External memory and concierge services, for humans and LLMs.
Seriously, there is a LOT going on here, one day I hope to have the leisure to write it up, and share more of it.

## IoT

- **[UPD](https://github.com/smiffy-online/upd)** — Universal Payload Decoder. Parametric 
decoding for LoRaWAN sensors, replacing per-device decoders with one configurable implementation. PoC
at the moment, but it works. Could be integrated into an agentic flow, to cut out all the boring bits,
but I am not currently engaged in that area, so feel free to adopt, adapt, improve.

## Micropython

- **[micropython-timezone](https://github.com/smiffy-online/micropython-timezone)** — timezone handling for MicroPython, emulating Python's `zoneinfo`.
- **[micropython-firmware-builder](https://github.com/smiffy-online/micropython-firmware-builder)** — custom firmware builds. WIP, contributions welcome.

## Network

- **[network-scan](https://github.com/smiffy-online/network-scan)** — cross-platform (Linux/Darwin) network discovery. Active ARP scanning combined with ARP cache analysis.

## How this was built

The code in these repositories was partly developed through my Claude framework, I thrash out the specs 
with Opus on desktop, create tasks as State MCP threads, then I manually transfer a handoff note to Claude Code,
Either Sonnet, or Opus, depending on the task. Where I watch closesly, and with saintly patience.

## Contact

**Email:** dev@smiffy.online · **LinkedIn:** [linkedin.com/in/smiffy](https://linkedin.com/in/smiffy)

## License

All repositories MIT unless otherwise noted.
