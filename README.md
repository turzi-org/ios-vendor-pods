# ios-vendor-pods

CocoaPods archives that Turzi's iOS app depends on and that are no longer
downloadable from their original host. Each is published, unchanged in content,
as an asset of a GitHub release here, and the app's own podspecs point at it.

## onnxruntime 1.15.1 (release `onnxruntime-1.15.1`)

`onnxruntime-c` and `onnxruntime-objc` 1.15.1, pinned by the Flutter plugin
`onnxruntime` 1.4.1. Microsoft's pod host for these versions
(`onnxruntimepackages.z14.web.core.windows.net`) now answers 404, and its newer
host does not serve a valid certificate, so a clean `pod install` failed.

- Rebuilt from intact CocoaPods installs of the original archives. Two
  independently downloaded copies were compared file by file and are identical.
- The original podspecs carry no checksum; ours pin the sha256 in `SHA256SUMS`.
- ONNX Runtime is © Microsoft Corporation under the MIT License
  (`LICENSE-onnxruntime`, also inside each archive). Nothing here is modified.
