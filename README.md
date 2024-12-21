CSS keyframe animations are awesome. They're one of the most powerful, versatile tools in CSS, and we can use them for all sorts of nifty things.
But they're also often misunderstood. They're a bit quirky, and if you don't understand those quirks, using them can be quite frustrating.
The main idea with a CSS keyframe animation is that it'll interpolate between different chunks of CSS.
For example, here we define a keyframe animation that will smoothly ramp an element's horizontal position from -100% to 0%:
@keyframes slide-in {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0%);
  }
}
Each @keyframes statement needs a name! In this case, we've chosen to name it slide-in. You can think of this like a global variable.*
Keyframe animations are meant to be general and reusable. We can apply them to specific selectors with the animation property.
