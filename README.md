# AgentSwarm

A multi-agent orchestration framework for coordinating autonomous AI agents.

## Installation

```bash
pip install agentSwarm
```

## Quick Start

```python
from agentswarm import Agent, Swarm

# Define agents
agent1 = Agent(
    name="Agent1",
    instructions="You are a helpful assistant.",
    tools=[...]
)

agent2 = Agent(
    name="Agent2", 
    instructions="You specialize in data analysis.",
    tools=[...]
)

# Create swarm and run
swarm = Swarm(agents=[agent1, agent2])
response = swarm.run(
    agent=agent1,
    messages=[{"role": "user", "content": "Hello!"}]
)
```

## Features

- Multi-agent coordination
- Tool/Function calling
- Agent handoffs
- Context variables
- Streaming support

## License

MIT