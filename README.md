# PassGate_STA-Net_Pitch_Deck


# GatePass

> *Because "he said he was from Swiggy" is not a security system.*

GatePass is a low-cost entry-access system for housing societies. Today, anyone who gets past the main gate can wander around the society for as long as they like: a wrong house, a "quick look" at the bicycles, a long chat with the plants. GatePass keeps track of every visitor after the gate.

## Try it (no install, no sign-up, no OTP to your own phone)

** https://aryanbcrazy-prog.github.io/PassGate_STA-Net_Pitch_Deck/**

Open the link and you're in. It runs entirely in your browser. A laptop works best, and there's a **Phone** button in the top bar if you want to see the mobile layout.

## How to explore

The top bar has two tabs.

**1. Guard interface**
- Pick a visitor type: delivery, essential services, an unknown visitor, or a relative.
- Enter a phone number, pick a wing, floor and house (or search by family name), and confirm.
- You land on the dashboard:
  - **Emergency messages** flash red when something is wrong.
  - **Sensors** show which ones are alive. "Check all sensors" pings each one.
  - **Guests inside** lists everyone's last checkpoint and OTP, with a red flag to revoke it.
  - **Residents waiting approval** shows who is waiting for permission.
- Then wait about 30 seconds and watch things go wrong on purpose.

**2. Sample entry**
- Pick a guest and a sensor, and walk up to a keypad like a visitor would.
- **Enter OTP** only works if the code is right. **Speak OTP** always opens the gate.
- Watch the little glass gate open, or refuse. If the sensor has been declared dead, it won't accept anything.

## ⚙️ How the system works

- **Sensors** are small, cheap devices at the main gate and at each wing. Visitors enter their OTP at every one, so the system knows where they are.
- Sensors report in with *alive* / *no reply* / *stop*, and guards see plain-English messages instead of signals.
- Guards can **revoke an OTP** the moment someone looks suspicious.
- Everything (OTPs, guests, alerts) is simulated in the browser and resets when you reload, so you can't break anything. Please try anyway.

## How was this built?

Every prompt used to build this project is in [`prompts.txt`](./prompts.txt). It goes from the first system brief to the last bug fix, in order. It shows how the system grew, one very specific request at a time.

## Thank you

A big thank you to the organisers of **CSI TechVision** for putting this event together and giving this idea a reason to exist. Without you it would still be a notebook doodle titled "gate thing??".

## Fine print

This is a demo. The OTPs are not actually sent as SMS, and no real society was harmed (or secured) in the making of this project.
