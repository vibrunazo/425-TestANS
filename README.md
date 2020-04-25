Anim Notify State bug in Unreal Engine

1. Setup an Anim Montage that lasts around 1sec

2. Add an Anim Notify State that starts at 0.1sec and lasts for 0.5sec with Tick Type set to Queued. https://puu.sh/FCorN/1c098260c0.png https://puu.sh/FCosl/78271196df.png

3. Play that Montage, then play it again on Blend Out: https://puu.sh/FCoui/ff34965b78.png

The Anim Notify State will trigger once for the first Montage Play then trigger twice on the second, triggering a total of 3 times. https://puu.sh/FCowZ/02e20e594b.png

In this particular project for UE 4.25 preview 7. The ThirdPersonCharacter Blueprint calls the Montages from Begin Play. 