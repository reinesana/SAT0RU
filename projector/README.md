## Projector Extension

An extension of SAT0RU that projects cursed techniques onto a wall. Your laptop camera tracks your hands, and each technique appears on the wall just above your hand, so from the audience's point of view it looks like you're casting it.

## Design

* **Controller** (`projector/index.html`) runs on your laptop screen. It tracks your hands, detects the signs, and sends the technique and hand position to the projector.
* **Projector** (`projector/index.html?projector`) runs fullscreen on the projector. It only renders the particle effects, at the position the controller sends.

An initial calibration maps points in the camera image to points on the projected image, so the effect lines up with your hand as seen from the camera.

## Setup

### Running
1.  **Connect the projector** and set your display to **extend**, not mirror (macOS: System Settings → Displays).
2.  **Start the project:** right-click `projector/index.html` in VS Code and select "Open with Live Server".
3.  **Open the projector window:** click **Open Projector**, drag the new window onto the projector screen, and click it to go fullscreen.
4.  **Position the camera** so it can see both you and the projected area on the wall behind you.
5.  **Calibrate:** click **Calibrate**. Four numbered markers appear on the wall. Click the centre of each one, in order, where you see it in the camera view on your laptop.
6.  **Cast:** Red forms on your index fingertip, Hollow Purple at your pinch point, and the Domain Expansions above your hand. Use **Effect size** and **Height above hand** (domains only) to fine-tune the effect.


## Tips

* **Avoid blocking the beam.** If the projector is in front of you, your body casts a shadow on the wall. Mount it high or stand slightly to the side of the beam.
* **Keep the controller window open.** Minimising it slows down hand tracking.
