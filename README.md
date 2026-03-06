<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="logo/telescope-full-dark.svg">
    <source media="(prefers-color-scheme: light)" srcset="logo/telescope-full.svg">
    <img alt="Telescope" src="logo/telescope-full.svg" height="80">
  </picture>
</p>

<p align="center">
  Documentation site for <a href="https://github.com/eduardoslonski/telescope">Telescope</a> — a framework for post-training LLMs with reinforcement learning for reasoning and agents.
</p>

# Telescope Docs

Deployed at [docs.telescope.training](https://docs.telescope.training).

## Repositories

| Repository | Description |
|------------|-------------|
| [telescope](https://github.com/eduardoslonski/telescope) | Training engine — orchestrator, vLLM inference, FSDP/Megatron trainer on Ray |
| [telescope-ui](https://github.com/eduardoslonski/telescope-ui) | Visualization dashboard — real-time metrics, rollout inspection, GPU timeline |

## Structure

```
training/           # Training engine docs
  installation      # Docker & source install
  examples          # Example configs (countdown, math, wordle, code)
  features          # Feature overview
  architecture      # Orchestrator, inference, trainer
  async-training    # Async rollout generation
  algorithms        # GRPO, RLOO, REINFORCE++, DR-GRPO, CISPO, GSPO, SAPO
  environments      # Single-turn, multi-turn, custom environments
  reward-design     # Multi-component rewards, normalization
  data-preparation  # Dataset format and loading
  tool-calling      # Agentic training with sandbox execution
  checkpointing     # Save, resume, HuggingFace conversion
  multi-node        # Ray cluster setup, placement strategies
  evals             # Periodic and standalone evaluation
  visualization     # Connecting to telescope-ui
  performance       # Sequence packing, prefetch, sample lanes
  config            # Three-layer config system
  troubleshooting   # Common issues

visualization/      # UI dashboard docs
  installation      # pip install telescope-ui
  how-it-works      # W&B sync, DuckDB storage
  overview          # Landing page and progress
  metrics           # Charts, custom dashboards, EMA smoothing
  rollouts          # Sample browser, multi-turn, render toggles
  timeline          # Gantt chart, event breakdown
  infra             # GPU/CPU metrics, topology, model viewer
  evals             # Eval results and pass@k
  runs              # Run management and discovery
  database          # Storage, compression
```
