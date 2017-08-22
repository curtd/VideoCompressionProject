# Data Features
- all integer values are positive unless otherwise noted
- all features are included in the model unless otherwise noted

## Index
- Description: itemization of each measurement - unique for each test batch
- Type: Numeric (Integral)
- Included: No

## CameraName
- Description: code to distinguish different cameras
- Type: Categorical (Unordered)
- Values: D30, D24, D16, A8, A5, F6, F12, A3

## PrimaryResolution
- Description: Width x Height in pixels
- Type: Numeric (Integral)

## SecondaryResolution
- Description: Width x Height in pixels of secondary stream
- Type: Numeric (Integral)

## TertiaryResolution
- Description: Width x Height in pixels of tertiary stream
- Type: Numeric (Integral)

## Flicker
- Description: Camera cuts out light flicker, depending on the region
- Type: Categorical (Ordered)
- Values: 50Hz or 60Hz

## Keyframe
- Description: number of P/B-frames between I-frames (minus 1)
- Type: Numeric (Integral)

## ImageRate
- Description: frames per second
- Type: Numeric (Integral)

## Quality
- Description: compression control, low number is best quality, highest bitrate
- Type: Numeric (Integral)

## Sharpening
- Description: edge-detection filter parameter (always 50)
- Type: Numeric (Integral)
- Included: No

## Nonlinear
- Description: single or multi-exposure frames (aka High Dynamic Range)
- Type: Categorical (Unordered)
- Values: 1 - HDR on, 0 HDR off

## Mode
- Description: High performance or standard modes
- Type: Categorical (Unordered)
- Values: 1 - high performance, 0 - standard performance
- Included: No

## Compression
- Description: Additional compression mode - lowers quality for still parts of the scene
- Type: Categorical (Unordered)
- Values: 'Off' or 'On'

## KbpsLimit
- Description: (kilobits per second) - user set maximum bitrate
- Type: Numerical (Integral)

## WaitSeconds
- Description: Time between measurements
- Type: Numerical (Integral)

## CollectSeconds
- Description: Time of data collection
- Type: Numerical (Integral)

## TotalBytes
- Description: Number of bytes transmitted from camera to network
- Type: Numerical (Integral)

## PrimaryBitsPerSecond
- Description: Mean bitrate over measurement interval accounted for by primary stream
- Type: Numerical (Real)
- Predictor

## SecondaryBitsPerSecond
- Description: Mean bitrate over measurement interval accounted for by secondary stream
- Type: Numerical (Real)
- Predictor

## TertiaryBitsPerSecond
- Description: Mean bitrate over measurement interval accounted for by tertiary stream
- Type: Numerical (Real)
- Predictor

## Status
- Description: Measurement success, warning, or failure
- Type: String

## Message
- Description: More information on warning or failure
- Type: String

## Test
- Description: Type of test - correlation with camera parameter fields
- Type: Categorical (Unordered)
- Values: Base, Idle, Compression

## Detail
- Description: Low detail - easy to compress, lower bitrate
- Type: Categorical (Ordered)
- Values: low, medium, high


## Motion
- Description: Low motion - easy to compress, lower bitrate
- Type: Categorical (Ordered)
- Values: none, low, high 
