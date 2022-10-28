# Public Works Basic Template

A basic HTML + Javascript template for generative works for the public works platform.

## Usage
Clone or use this project as a template `https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template`

Modify `index.js` to create your rendering logic using a prng from `createPrng()`

Press space bar or touch to create a new hash.

## Work Requirements
* A work must be reproducible. If a work is given the same hash, it must produce the exact same image.
* Save attributes with `setProperties(myAttributes, myOptionalTraits)` before your rendering is complete.
* Call `setPreviewReady()` when the preview is complete. Otherwise, a snapshot will be taken after 60 seconds.
* Attributes and traits must be a javascript object where keys are the attribute names and values one of `string`, `number` or `boolean`. Any other type will be serialized with `.toString()`.
* Your work must be self-contained-- any external calls will be blocked during the preview rendering pipeline.
