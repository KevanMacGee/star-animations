# Animation 1 — Staggered & Glow

Reproduce the **“Staggered & Glow”** star animation from my reference exactly.

Apply the effect to a row of five stars. Do not redesign the surrounding component, card, typography, spacing, or layout. The task is specifically to recreate the star entrance animation.

### Starting state

Each star should begin with:

- `opacity: 0`
- `transform: scale(0.5)`
- Gold color: `#d4af37`
- Transition duration: `0.6s`
- Transition easing: `cubic-bezier(0.34, 1.56, 0.64, 1)`

### Visible state

When the animation is triggered, each star should transition to:

- `opacity: 1`
- `transform: scale(1)`
- `text-shadow: 0 0 15px rgba(212, 175, 55, 0.6)`

The effect should feel like each star **gently pops into existence with a soft gold glow**.

### Stagger timing

The stars must appear one after another from left to right using these exact delays:

1. Star 1: `0.1s`
2. Star 2: `0.2s`
3. Star 3: `0.3s`
4. Star 4: `0.4s`
5. Star 5: `0.5s`

Do not substitute a different stagger interval.

### Trigger behavior

Trigger the animation when approximately **50% of the star container enters the viewport**.

The animation must run **only once**. Once triggered, the stars remain fully visible and glowing. Scrolling away and back should not replay it.

Do not turn this into a continuously pulsing animation.

The goal is to reproduce the original motion and timing as precisely as possible rather than creating an animation merely inspired by it.

---

# Animation 2 — Fly-in & Spin

Reproduce the **“Fly-in & Spin”** star animation from my reference exactly.

Apply the animation to five stars without changing the rest of the component's design.

### Starting state

Each star should begin:

- `opacity: 0`
- `transform: translateY(20px) rotate(-45deg)`

Use this transition:

- Duration: `0.6s`
- Easing: `cubic-bezier(0.34, 1.56, 0.64, 1)`

### Visible state

Each star transitions to:

- `opacity: 1`
- `transform: translateY(0) rotate(0deg) scale(1)`

The star should therefore appear to **rise approximately 20px into position while rotating 45 degrees into alignment**.

It is a relatively quick, clean entrance rather than a long spin.

### Stagger timing

Use these exact delays:

1. Star 1: `0.10s`
2. Star 2: `0.15s`
3. Star 3: `0.20s`
4. Star 4: `0.25s`
5. Star 5: `0.30s`

Notice that this stagger is considerably tighter than the Staggered & Glow version. Preserve that difference.

### Trigger behavior

Start the sequence when approximately **50% of the star container becomes visible in the viewport**.

Run it once only.

After each star has arrived, it remains completely static in its finished position.

Do not add looping motion, bouncing, additional rotations, or glow unless it already exists elsewhere in the design.

The objective is exact reproduction of the described movement, timing, and easing.

---

# Animation 3 — Pulse Wave

Reproduce the **“Pulse Wave”** star animation exactly.

This is a **one-time sequential pulse**, not a continuously pulsing star rating.

Each of the five stars should perform the same animation one after another from left to right.

### Exact keyframe sequence

Animate each star over:

`0.8s ease-out`

Use these exact stages:

**0%**

- `transform: scale(0.5)`
- `opacity: 0`
- `filter: brightness(1)`

**50%**

- `transform: scale(1.5)`
- `opacity: 1`
- `filter: brightness(1.8)`

**100%**

- `transform: scale(1)`
- `opacity: 1`
- `filter: brightness(1)`

The visual effect should be:

**small/invisible → dramatically expands and brightens → settles to normal size**

The expansion to `1.5` scale is intentional. Do not tone it down.

### Stagger timing

Use exactly:

1. Star 1: `0.1s`
2. Star 2: `0.2s`
3. Star 3: `0.3s`
4. Star 4: `0.4s`
5. Star 5: `0.5s`

This creates a pulse that visually travels from left to right across the five stars.

### Trigger behavior

Trigger when approximately **50% of the stars' container enters the viewport**.

Run the animation once.

Once a star completes its pulse, it should remain:

- visible
- normal size
- normal brightness
- static

Do not make the stars continue breathing, shimmering, glowing, or pulsing.

Preserve these exact values rather than approximating the animation with a generic “pop” effect.

---

# Animation 4 — Staggered Pulse Pop

Reproduce the **“Staggered Pulse Pop”** animation exactly.

This effect combines the entrance, oversize pulse, brightness increase, and gold glow into one animation.

Do not simplify this into a normal scale animation or generic glow.

### Animation duration and easing

Each star uses:

`0.7s cubic-bezier(0.25, 0.46, 0.45, 0.94)`

and retains its final state after completion.

### Exact keyframes

**0%**

- `transform: scale(0.2)`
- `opacity: 0`
- `text-shadow: 0 0 0px rgba(212, 175, 55, 0)`

The star begins extremely small and invisible.

**50%**

- `transform: scale(1.6)`
- `opacity: 1`
- `text-shadow: 0 0 30px rgba(212, 175, 55, 1)`
- `filter: brightness(1.5)`

At the midpoint, the star should dramatically overshoot its normal size while producing a strong gold glow.

**100%**

- `transform: scale(1)`
- `opacity: 1`
- `text-shadow: 0 0 10px rgba(212, 175, 55, 0.4)`
- `filter: brightness(1)`

The star then settles to normal size while retaining a subtle residual glow.

### Stagger timing

Animate the five stars left-to-right with:

1. Star 1: `0.1s`
2. Star 2: `0.2s`
3. Star 3: `0.3s`
4. Star 4: `0.4s`
5. Star 5: `0.5s`

### Trigger behavior

Trigger once approximately when **50% of the star container enters the viewport**.

Do not replay the animation when the element leaves and re-enters the viewport.

After the sequence completes, every star should remain visible, normal-sized, and subtly glowing.

The large `1.6` scale and strong `30px` midpoint glow are deliberate parts of the design. Do not reduce them in an attempt to make the effect more subtle.

---

# Animation 5 — Falling Spin / Wobble Settle

Reproduce the **“Falling Spin — Wobble Settle with Glow Wave”** star animation exactly.

This animation is intentionally much more elaborate than the simpler star reveals.

Each star should appear to **fall from above while spinning rapidly, reach its destination, then wobble from side to side as its golden glow peaks and gradually disappears**.

Do not replace this with a generic drop, bounce, spring, or rotate animation.

### Starting state

Before triggering, each star should have:

- `opacity: 0`
- `transform: translateY(-80px) rotate(-720deg) scale(0.7)`
- `text-shadow: 0 0 0px rgba(212, 175, 55, 0)`

### Duration and easing

Use:

`1.5s cubic-bezier(0.22, 1, 0.36, 1)`

The animation must retain its final state.

### Exact keyframes

**0%**

- `opacity: 0`
- `translateY(-80px)`
- `rotate(-720deg)`
- `scale(0.7)`
- no glow
- `brightness(1)`

**45%**

- `opacity: 1`
- `translateY(0)`
- `rotate(15deg)`
- `scale(1)`
- `text-shadow: 0 0 18px rgba(212,175,55,0.7), 0 0 35px rgba(212,175,55,0.25)`
- `brightness(1.4)`

This is the initial landing.

**52%**

- `translateY(0)`
- `rotate(-14deg)`
- `scale(1)`
- `text-shadow: 0 0 24px rgba(212,175,55,1), 0 0 50px rgba(212,175,55,0.35)`
- `brightness(1.6)`

This is the strongest opposite-direction wobble and brightest moment.

**59%**

- `rotate(8deg)`
- `scale(1)`
- glow returns to:\
  `0 0 18px rgba(212,175,55,0.7), 0 0 35px rgba(212,175,55,0.25)`
- `brightness(1.3)`

**65%**

- `rotate(-5deg)`
- `scale(1)`
- `text-shadow: 0 0 10px rgba(212,175,55,0.4)`
- `brightness(1.1)`

**72%**

- `rotate(2deg)`
- `scale(1)`
- `text-shadow: 0 0 4px rgba(212,175,55,0.15)`
- `brightness(1.05)`

**78%**

- `rotate(0deg)`
- `scale(1)`
- no glow
- `brightness(1)`

**100%**

- `opacity: 1`
- `translateY(0)`
- `rotate(0deg)`
- `scale(1)`
- no glow
- `brightness(1)`

The remaining time after 78% intentionally lets the final settled state breathe.

### Stagger timing

Use these exact delays:

1. Star 1: `0.10s`
2. Star 2: `0.22s`
3. Star 3: `0.34s`
4. Star 4: `0.46s`
5. Star 5: `0.58s`

### Important visual character

The motion should read as:

**fall + rapid two-turn spin → land slightly crooked → wobble left/right with decreasing rotation → settle perfectly straight**

The glow should peak during the wobble and then completely disappear.

### Trigger behavior

Trigger once when approximately 50% of the container enters the viewport.

Do not replay on subsequent scrolling.

Once complete, all stars remain completely static.

Do not alter, shorten, “smooth out,” or simplify the intermediate wobble keyframes. Their asymmetry is what creates the intended physical settling effect.

---

# Animation 6 — Falling Spin / Magnetic Snap

Reproduce the **“Falling Spin — Magnetic Snap”** animation exactly.

This begins similarly to the Falling Spin / Wobble version, but its landing behavior is intentionally different.

The star should **fall and spin into the area, slightly overshoot its final position, pull backward briefly, and then appear to magnetically snap into perfect alignment with a sudden strong gold flash**.

Do not turn this into a wobble animation. The defining feature is the decisive snap.

### Starting state

Before triggering:

- `opacity: 0`
- `transform: translateY(-80px) rotate(-720deg) scale(0.7)`
- `text-shadow: 0 0 0px rgba(212, 175, 55, 0)`
- `filter: brightness(1)`

### Duration and easing

Use exactly:

`1.5s cubic-bezier(0.22, 1, 0.36, 1)`

Retain the finished state.

### Exact keyframes

**0%**

- `opacity: 0`
- `translateY(-80px)`
- `rotate(-720deg)`
- `scale(0.7)`
- no glow
- `brightness(1)`

**60%**

- `opacity: 1`
- `translateY(6px)`
- `rotate(10deg)`
- `scale(1.05)`
- no glow
- `brightness(1)`

The star has slightly overshot its destination.

**72%**

- `translateY(-2px)`
- `rotate(-3deg)`
- `scale(0.97)`
- `text-shadow: 0 0 30px rgba(212,175,55,1), 0 0 60px rgba(212,175,55,0.4)`
- `brightness(1.7)`

The star is briefly pulled slightly past its resting point in the opposite direction and begins glowing dramatically.

**78%**

- `translateY(0)`
- `rotate(0deg)`
- `scale(1.02)`
- `text-shadow: 0 0 35px rgba(212,175,55,1), 0 0 70px rgba(212,175,55,0.45)`
- `brightness(1.8)`

This is the key **magnetic snap** moment.

The star reaches exact rotational alignment while becoming slightly oversized and producing its strongest glow.

**84%**

- `translateY(0)`
- `rotate(0deg)`
- `scale(1)`
- `text-shadow: 0 0 15px rgba(212,175,55,0.4), 0 0 35px rgba(212,175,55,0.15)`
- `brightness(1.15)`

The flash quickly dissipates.

**100%**

- `opacity: 1`
- `translateY(0)`
- `rotate(0deg)`
- `scale(1)`
- no glow
- `brightness(1)`

### Stagger timing

Use exactly:

1. Star 1: `0.10s`
2. Star 2: `0.22s`
3. Star 3: `0.34s`
4. Star 4: `0.46s`
5. Star 5: `0.58s`

### Important visual character

The intended sequence is:

**fall while spinning → overshoot downward → pull slightly upward/back → SNAP into exact position with a bright golden flash → rapidly settle**

The 72–84% portion is critical.

Do not replace it with a conventional bounce.

Do not gradually introduce the glow across the whole fall. The strongest glow belongs specifically around the magnetic snap at 72–78%.

### Trigger behavior

Trigger once when approximately **50% of the star container is visible**.

Do not replay when scrolling back to it.

At completion, the stars should be completely static with:

- no glow
- no rotation
- normal brightness
- normal scale
