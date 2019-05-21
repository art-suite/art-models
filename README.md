# Art.Models

Successor to Art.Flux

Goal: Composability:

* models should not be accessed through a global namespace
* fluxStore becomes part of each model
* ApplictionState has a custom store that works "just like a headless component"

All models
* have epoched-state-update-queues
* are subscription-sources

But stores may vary. ApplicationState persists its state values even
when there are no subscribers.

But others use the old FluxStore, transient model that releases state when
no subscribers.

### Install

```coffeescript
npm install art-models
```