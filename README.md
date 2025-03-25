**owc_witnesses**  
*A lightweight witness system for RedM*

**owc_witnesses** is a modular witness system that alerts specific jobs when an event is witnessed. It creates a blip on the map after a configurable delay, allowing for immersive law enforcement reactions or other roleplay opportunities.

### 🔧 Features:
- Alerts specific jobs (configurable).
- Creates a map blip at the reported location.
- Configurable delay before the info and blip are broadcast.
- Optional chance system to control how likely a witness is to report an event.
- Easy integration into your existing scripts.

### ⚙️ Config Options:
- Delay time before sending the alert.
- List of jobs to be notified.
- Chance-based trigger to add realism.

### 🔗 How to use in your client-side scripts:
To trigger a witness alert from your script, simply use:

```lua
TriggerServerEvent("owc-witnesses:CheckJob", GetPlayers(), GetEntityCoords(witness))
```

This will notify configured jobs with a blip at the given coordinates after the defined delay.
