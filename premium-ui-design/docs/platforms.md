# Platforms（平台自动切换）

## Web
自动加载：Responsive、Typography、Layout、Conversion UX、Motion、Accessibility
输出重点：
- CTA 与信息层级
- 表单/设置/空状态/错误恢复
- 可读性与对比度

## iOS
自动加载：Apple HIG、SwiftUI、Native Navigation、SF Symbols、Dynamic Type、Accessibility、Haptics、Motion、Liquid Glass（适用时）
强制原则：
> 不要把 Web UI 搬进 iPhone。

## macOS
单独处理（不要与 iOS 混用）：
Toolbar、Sidebar、Inspector、Menu Bar、Window、Sheet、Popover、Keyboard Shortcut、Context Menu、Drag & Drop、Multi-window
强制原则：
> Mac App 像 Mac App。

## Android
自动加载：Material 3、Jetpack Compose、Android Navigation、Adaptive Layout、Dynamic Color、Android Interaction
强制原则：
> iOS ≠ Android。

## Flutter / React Native
跨平台核心一致 + 平台差异化适配：
navigation/back/sheet/dialog/picker/typography/spacing/motion 分别按平台调整。

