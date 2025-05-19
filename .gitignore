NearestPoint – Advanced Explanation

Vireal

Projects the hit position into the part's local space, clamps it within the local bounding box, and returns the corresponding point in world space. Fully respects part orientation.

Quantis

Performs clamping in world space using the part's center and half-size. Ignores rotation — best used only on axis-aligned, unrotated parts.

Full

Converts to local space, but restricts the clamping to a tighter 50% region of the part’s size. This results in points that remain closer to the part's center.

Primor

Similar to `Vireal`, this method clamps the local-space hit position within the full bounds of the part, then transforms the result back into world space.

Point

Calculates the hit direction relative to the part’s center, then snaps to the furthest face in that direction. Slightly offsets the point outward to ensure it's just outside the part surface.

Method Summary

| Type       | Uses Local Space? | Clamps To     | Description                                |
| ---------- | ----------------- | ------------- | ------------------------------------------ |
| `Quantis`  | ❌ No              | World AABB    | World-based clamping, not rotation-safe    |
| `Vireal`   | ✅ Yes             | Local Box     | Accurate clamping on rotated parts         |
| `Full`     | ✅ Yes             | 50% Local Box | Restricts position toward center           |
| `Primor`   | ✅ Yes             | Local Box     | Alias of `Vireal`                          |
| `Fractaln` | ✅ Yes             | Local Box     | Duplicate of `Primor`                      |
| `Point`    | ✅ Yes             | Surface Face  | Snaps to outward face and offsets slightly |
