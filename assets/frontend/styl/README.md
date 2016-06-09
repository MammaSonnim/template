// Rupture HINT

+above(measure) +from-width(measure) When the screen size is above the provided measure, the styles in the block will take effect. Styles take effect from the provided measure and above.

+below(measure) +to-width(measure) When the screen size is below the provided measure, the styles in the block will take effect. Styles take effect from zero up to the provided measure.

+between(measure, measure) When the screen size is between the two provided measure, the styles in the block will take effect.

+at(measure)  Intended for use with scale measures, when the screen size is between the provided scale measure and the one below it, the styles in the block will take effect. For example, if your scale was something like rupture.scale = 0 400px 600px, and you used the mixin like +at(2), it would kick in between 400 and 600px (remember, scale is zero indexed, so 2 is the third value, and one less is the second). If you use this with a value, it will not have much effect, as it will be at one specific pixel value rather than a range like you want.

+mobile() When the screen size is 320px (defined by rupture.mobile-cutoff) or less, the styles in the block will take effect.

+tablet() When the screen size is between 960px (defined by rupture.desktop-cutoff) and 320px (defined by mobile-cutoff), the styles in the block will take effect.

+desktop() When the screen size is 960px (defined by rupture.desktop-cutoff) or more, the styles in the block will take effect.

+hd() When the screen size is 1220px (defined by rupture.hd-cutoff) or more, the styles in the block will take effect.

+density(value) When the device has a pixel density of at least the given value, the styles in the block will take effect. The value should be a unitless pixel ratio number such as 1, 1.5, or 2. The value can also be retina, in which case the rupture.retina-density variable will be used.

+retina() When the device has a pixel density of over rupture.retina-density (defaults to 1.5), the styles in the block will take effect.
