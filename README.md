# Expo Camera Aspect Ratio Bug

This repository demonstrates a bug in Expo's Camera component related to aspect ratio distortion when custom styling is applied. The bug occurs when styling the Camera component in a way that alters its aspect ratio, resulting in distorted image captures.

The `bug.js` file reproduces the issue, while `bugSolution.js` provides a solution using the `Camera.Constants.Aspect` prop for better aspect ratio management.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`.
4. Observe the distorted preview and captured images in `bug.js`.
5. Compare with the corrected preview and captured images in `bugSolution.js`.

## Solution

The solution involves using `Camera.Constants.Aspect` prop to explicitly set the aspect ratio, rather than relying on direct width and height styling.  This ensures consistent and undistorted image capture across different devices and screen sizes.  See `bugSolution.js` for implementation details.